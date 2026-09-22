<h1 id="13g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $0\le t\le1$, put $F_t=f+tg$. On the curve, $|F_t|\ge|f|-t|g|>0$, so no member of this homotopy has a boundary zero. The [argument principle](../../../../../../argument-principle.md) counts the interior zeros, with [multiplicity](../../../../../../multiplicity-mathematics.md), by its winding number $N(t)=\operatorname{wind}(F_t\circ\gamma,0)$. For a piecewise smooth curve this is

$$
N(t)=\frac1{2\pi i}\int_\gamma\frac{F_t'(z)}{F_t(z)}\,dz.
$$

There are no poles, and the null-homotopy of the Jordan curve in the domain permits this interior count. The loops $F_t\circ\gamma$ form a continuous homotopy avoiding zero, so their integer winding number stays constant. Equivalently, for a piecewise smooth curve the integral varies continuously with $t$ and is integer-valued. In particular

$$
\boxed{N(f)=N(f+g)}.
$$

This proves [Rouché's theorem](../../../../../../rouche-s-theorem.md). The counting is with [multiplicity](../../../../../../multiplicity-mathematics.md) and assumes the usual positive orientation; reversing orientation reverses both winding counts without changing the conclusion.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [13G](../../13g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
