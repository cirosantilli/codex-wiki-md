<h1 id="d/d1/solution">Solution</h1>

↑ **Parent:** [D1](../d1.md)

For $x>0$ the geometric ratio $e^{-2x}$ has modulus less than one, and

$$
\sum_{m\geq0}(1-e^{-x})e^{-(2m+1)x}
=\frac{(1-e^{-x})e^{-x}}{1-e^{-2x}}=\frac1{e^x+1}.
$$

Every summand is nonnegative. The [monotone convergence theorem](../../../../monotone-convergence-theorem.md) therefore permits integration of the sum:

$$
\int_0^\infty\frac{dx}{e^x+1}
=\sum_{m\geq0}\left(\frac1{2m+1}-\frac1{2m+2}\right).
$$

The [integral](../../../../integral-split.md) is finite because its integrand is bounded above by $e^{-x}$, whose [integral](../../../../integral-split.md) is one. The displayed paired sums are the even partial sums of the [alternating harmonic series](../../../../alternating-harmonic-series.md); its odd partial sums differ by a term tending to zero. Thus the required equality holds with the usual series ordering. One can additionally evaluate it by $t=e^{-x}$:

$$
\boxed{\int_0^\infty\frac{dx}{e^x+1}=\int_0^1\frac{dt}{1+t}=\log2
=\sum_{n=1}^\infty\frac{(-1)^{n+1}}n.}
$$

Grouping into nonnegative pairs supplies the justified interchange; [absolute convergence](../../../../absolute-convergence.md) of the ungrouped integrated alternating series is not needed and would be false.

## ↑ Ancestors (12)

1. [D1](../d1.md)
2. [D](../../d.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
