<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Keep successive timestamps in raw unsigned ticks, and convert their modular difference to milliseconds only after subtraction. The first pulse establishes a timestamp; it does not create a fictitious interval from startup. Store valid intervals in a five-element [ring buffer](../../../../../circular-buffer.md). During startup, average the one to four intervals actually available; return zero until there is at least one valid interval. Here zero is explicitly an unavailable-data sentinel.

The following [C programming language](../../../../../c-programming-language.md) code uses the supplied register names through an abstract [memory-mapped input-output](../../../../../memory-mapped-input-output.md) register interface. The board port supplies the actual register mapping and interrupt vector; no undocumented addresses are assumed. The two interrupt-mask hooks have the exact semantics described below and are interface requirements, not names asserted to exist in an unspecified device library.

```
#include <stdint.h>
#include <stdbool.h>

struct gpio_registers { volatile uint32_t EVENT; };
struct timer_registers { volatile uint32_t COUNT; };
extern struct gpio_registers GPIO;
extern struct timer_registers TIMER;

uint32_t irq_save_disable(void);
void irq_restore(uint32_t old_mask);

static volatile uint32_t interval_ms[5];
static volatile uint32_t next_slot = 0;
static volatile uint32_t valid = 0;
static volatile uint32_t previous_tick = 0;
static volatile bool have_previous = false;

void gpio_handler(void)
{
    if (GPIO.EVENT == 0)
        return;
    uint32_t now = TIMER.COUNT;
    GPIO.EVENT = 0;                 /* acknowledge with the specified write */
    if (have_previous) {
        uint32_t ticks = now - previous_tick;
        interval_ms[next_slot] = ticks / UINT32_C(16000);
        next_slot = (next_slot + 1) % 5;
        if (valid < 5)
            ++valid;
    } else {
        have_previous = true;
    }
    previous_tick = now;
}

uint32_t get_pulse(void)
{
    uint32_t local[5];
    uint32_t mask = irq_save_disable();
    uint32_t n = valid;
    for (uint32_t i = 0; i < n; ++i)
        local[i] = interval_ms[i];
    irq_restore(mask);             /* restore the earlier mask, not just enable */

    if (n == 0)
        return 0;
    uint64_t total = 0;
    for (uint32_t i = 0; i < n; ++i)
        total += local[i];
    if (total == 0)
        return 0;
    /* Mean duration is total/n milliseconds; round bpm to nearest integer. */
    return (uint32_t)((UINT64_C(60000) * n + total / 2) / total);
}
```

Before the buffer fills, its valid entries occupy positions $0,\ldots,n-1$. Once full, all five positions are valid, so their order is irrelevant to their sum. The conversion uses 16,000 ticks per millisecond. Truncating each interval introduces less than one millisecond of error per interval. The desired conversion is **$60000n/\sum_i\Delta_i$ beats per minute**, the reciprocal of the mean interval; averaging the individual values $60000/\Delta_i$ is generally different.

`irq_save_disable` saves the previous interrupt mask and prevents the GPIO handler from running until `irq_restore` restores that mask. Both hooks must include compiler memory barriers. On an appropriate privileged Cortex-M target, the implementation can use `MRS PRIMASK`, `CPSID i` and `MSR PRIMASK`, with a compiler memory clobber. These target operations implement [interrupt masking](../../../../../interrupt-masking.md); they are not expressible as portable ISO C alone. One concrete GCC/Clang-compatible privileged Cortex-M port for those hooks is:

```
uint32_t irq_save_disable(void)
{
    uint32_t old_mask;
    __asm__ volatile ("mrs %0, primask\n\tcpsid i"
                      : "=r" (old_mask) : : "memory");
    return old_mask;
}

void irq_restore(uint32_t old_mask)
{
    __asm__ volatile ("msr primask, %0"
                      : : "r" (old_mask) : "memory");
}
```

The compiler memory clobbers prevent access motion across the mask changes. Saving and restoring the entire prior mask is intentional; an unconditional enable would break an enclosing [critical section](../../../../../critical-section.md).[PRIMASK, \_\_get\_PRIMASK, \_\_disable\_irq and \_\_set\_PRIMASK](../../../../../cmsis-core-register-access-documentation-by-arm.md)

All state is initialized before enabling the peripheral interrupt. Assume the timer read is coherent, the handler is not reentered, and the device follows the stated write-zero acknowledgment semantics.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [Digital systems, linear algebra, introduction to formal proof resit](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
