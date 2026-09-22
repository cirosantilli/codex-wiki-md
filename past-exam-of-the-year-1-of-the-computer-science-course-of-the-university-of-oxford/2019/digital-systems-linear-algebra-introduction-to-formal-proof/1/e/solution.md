<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**Use four working [processor registers](../../../../../processor-register.md) by packing the growing [quotient](../../../../../quotient.md) into the vacated low [bits](../../../../../bit.md) of the shifting dividend.** The following is A32 [assembly language](../../../../../assembly-language.md) with conditional execution, an allowed instance of the question's general 32-bit [Reduced instruction set computer](../../../../../reduced-instruction-set-computer.md). It is not restricted to the sixteen-bit encodings in the supplied [Thumb instruction set](../../../../../thumb-instruction-set.md) table. On entry `r0` is the dividend and `r1` the positive divisor; `r2` becomes the high [remainder](../../../../../remainder.md) [machine word](../../../../../machine-word.md) and `r3` counts iterations. The [quotient](../../../../../quotient.md) is returned in `r0` and the ordinary [remainder](../../../../../remainder.md) remains in `r2`.

```
mov   r2, #0
mov   r3, #32
loop:
adds  r0, r0, r0
adcs  r2, r2, r2
cmp   r2, r1
subcs r2, r2, r1
adc   r0, r0, #0
subs  r3, r3, #1
bne   loop
bx    lr
```

Here `subcs` means conditional `sub` when [arithmetic carry](../../../../../carry-arithmetic.md) is set, **without** the flag-setting suffix. `adc` also preserves flags. Consequently the [arithmetic carry](../../../../../carry-arithmetic.md) from `cmp` survives until it is inserted as the next [quotient](../../../../../quotient.md) [bit](../../../../../bit.md). The loop has seven instructions, one of them conditional, and no data-dependent branch. Its sole branch is the backwards loop branch, taken 31 times. It uses no separate [quotient](../../../../../quotient.md) [processor register](../../../../../processor-register.md), zero [processor register](../../../../../processor-register.md), temporary comparison [processor register](../../../../../processor-register.md) or saved [arithmetic carry](../../../../../carry-arithmetic.md) [processor register](../../../../../processor-register.md). A [Thumb instruction set](../../../../../thumb-instruction-set.md) rendering using conditional execution would need an explicit conditional-execution encoding such as `it cs`; that is an additional encoded instruction, not an unexplained free operation.

The [packed restoring division](../../../../../packed-restoring-division.md) [loop invariant](../../../../../loop-invariant.md) relates it to the displayed algorithm. Specifically, let $M=2^{32}$, let $a$ retain its original mathematical value, and let $k$ be the number of completed iterations. Define the processed prefix $p_k=\lfloor a/2^{32-k}\rfloor$, its [quotient](../../../../../quotient.md) $Q_k=\lfloor p_k/b\rfloor$ and [remainder](../../../../../remainder.md) $R_k=p_k-bQ_k$. The [processor register](../../../../../processor-register.md) [loop invariant](../../../../../loop-invariant.md) is

$$
\text{high}=R_k,\qquad \text{low}=(a2^k\bmod M)+Q_k,\qquad 0\le Q_k<2^k.
$$

The two terms in the low [machine word](../../../../../machine-word.md) occupy disjoint [bit](../../../../../bit.md) positions. Its next outgoing [arithmetic carry](../../../../../carry-arithmetic.md) is therefore the next _original dividend [bit](../../../../../bit.md)_, not a [quotient](../../../../../quotient.md) [bit](../../../../../bit.md). `adds` shifts the low [machine word](../../../../../machine-word.md); `adcs` doubles the high [remainder](../../../../../remainder.md) and incorporates that dividend [bit](../../../../../bit.md). `cmp` decides whether this trial [remainder](../../../../../remainder.md) is at least the divisor; `subcs` performs the conditional subtraction, and `adc` appends its decision to the shifted [quotient](../../../../../quotient.md). This is exactly the doubling, compare/subtract and quotient-bit update, with the counter maintained separately. Before processing [bit](../../../../../bit.md) $k\le32$, the trial [remainder](../../../../../remainder.md) is at most $p_k<2^k\le M$, so the high-word addition does not require a hidden 33rd [remainder](../../../../../remainder.md) [bit](../../../../../bit.md) for this 32-bit dividend problem. After 32 iterations the residual dividend portion is zero, giving the stated outputs.

There is a **printed source error** in the auxiliary bound. At the initial state, choosing valid inputs $a=b=1$ makes the printed strict inequality $r2^j<b2^{32}$ false. The algorithm instead preserves $0\le r<b2^{32}$ for its _unpacked 64-bit_ variable, together with its printed equality [loop invariant](../../../../../loop-invariant.md). Doubling and subtracting $b2^{32}$ when necessary preserves that corrected bound. At termination the equality becomes $a2^{32}=qb2^{32}+r$; since $r$ is then divisible by $2^{32}$, it gives $0\le a-qb<b$. This source error does not invalidate the algorithm or the packed implementation. The figure is mathematical pseudocode: its `2^32` denotes exponentiation, rather than C's XOR operator.

The displayed A32 routine assembled successfully with Clang and was disassembled to check the conditional and non-flag-setting forms. Its [carry flag](../../../../../carry-flag.md) model was checked exhaustively at an eight-bit [machine word](../../../../../machine-word.md) size and against boundary and randomized 32-bit divisions. No native [ARM architecture family](../../../../../arm-architecture-family.md) execution is claimed.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
