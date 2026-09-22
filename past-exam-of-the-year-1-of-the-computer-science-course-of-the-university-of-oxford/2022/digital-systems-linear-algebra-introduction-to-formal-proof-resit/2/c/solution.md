<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A 32-bit free-running timer operates modulo $M=2^{32}$. If its previous reading is $p$, and the actual elapsed count is $d$ with $0\leq d<M$, the new reading is $(p+d)\bmod M$. The [modulo-counter elapsed-time identity](../../../../../modulo-counter-elapsed-time-identity.md) therefore gives

$$
\boxed{(\texttt{uint32\_t})(\texttt{now}-\texttt{previous\_tick})=d.}
$$

[Unsigned integer arithmetic in C](../../../../../unsigned-integer-arithmetic-in-c.md) reduces the subtraction modulo $2^{32}$, so the identity remains valid when a wrap occurs between pulses. For example, readings $2^{32}-8000$ and $8000$ give 16,000 ticks, hence one millisecond, rather than a negative interval.[Section 6.2.5 paragraph 9, unsigned arithmetic modulo one greater than the maximum representable value](../../../../../c11-committee-draft-n1570.md)

At the specified clock rate, **the true wrap period is $2^{32}/16{,}000{,}000=268.435456$ seconds**. The printed 256 seconds is inconsistent with the other two specifications. The implementation uses the stated 32-bit width and 16 MHz rate. Assuming consecutive handled pulses are less than 256 seconds apart is a sufficient conservative bound; the exact allowable bound is less than 268.435456 seconds.

This calculation requires less than one entire timer modulus of elapsed ticks between successive stored timestamps. If a whole wrap or several wraps elapse, identical register readings cannot reveal how many occurred; an overflow counter or an independent longer-range clock would be needed. Also assume pulse events are not lost and interrupt latency is constant or sufficiently small for the required accuracy: timestamps read in software measure handler-to-handler intervals, not perfect hardware capture times. Conversion to milliseconds occurs after modular subtraction, so separately rounded absolute timestamps cannot corrupt the wrap calculation.

## ↑ Ancestors (12)

1. [C](../c.md)
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
