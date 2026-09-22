<h1 id="1/d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

In IF, fetch `PREFETCH` normally. In ID, recognize its opcode, read the base [processor register](../../../../../../processor-register.md) and immediate offset, and set controls selecting a prefetch request rather than a [load instruction](../../../../../../load-instruction.md) or [store instruction](../../../../../../store-instruction.md). Ordinary [register forwarding](../../../../../../register-forwarding.md) and [data hazard](../../../../../../data-hazard.md) interlocks still apply to that base [processor register](../../../../../../processor-register.md). In EX, use the [arithmetic logic unit](../../../../../../arithmetic-logic-unit.md) to form the effective [memory address](../../../../../../memory-address.md).

Latch that [memory address](../../../../../../memory-address.md) and a prefetch-valid control into EX/MEM. In MEM, put the [memory address](../../../../../../memory-address.md) and any hint information on the dedicated request [computer bus](../../../../../../computer-bus.md), or enqueue them in a small prefetch-request queue. The [cache prefetching](../../../../../../cache-prefetching.md) engine handles lookup, allocation and the later [cache line](../../../../../../cache-line.md) return independently. Do not wait for the fill or select the returned data as a [register file](../../../../../../register-file.md) input. In WB, disable architectural [processor register](../../../../../../processor-register.md) and [processor condition flag](../../../../../../processor-condition-flag.md) writes; the instruction simply leaves the [in-order pipeline](../../../../../../in-order-pipeline.md).

If the request path is busy, dropping the hint is compatible with the contract in part (ii), and preserves its nonblocking purpose. A design that instead stalls until queue space exists can still be correct but reduces the performance benefit. A [memory management unit](../../../../../../memory-management-unit.md) must not turn a speculative hint into an ordinary protection fault: discard an invalid target, or use an appropriately checked nonfaulting translation path. Suppress device transactions for [memory-mapped input-output](../../../../../../memory-mapped-input-output.md) and avoid speculative writes. **Use the existing address-generation datapath, add a prefetch request/control path, and disable demand-load waiting and writeback.**

$$
\boxed{\text{EX forms the address; MEM queues the hint; WB writes nothing.}}
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [Computer architecture](../../../../computer-architecture-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
