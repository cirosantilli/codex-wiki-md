<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

By the spectral theorem, the operator in parentheses acts at spectral value $t\in\mathbb R$ by

$$
\frac1{2\pi i}\int_a^b
\left[\frac1{t-x-i\epsilon}
-\frac1{t-x+i\epsilon}\right]dx
=\frac1\pi\int_a^b
\frac\epsilon{(t-x)^2+\epsilon^2}\,dx.
$$

The Poisson kernel converges to $1$ for $t\in(a,b)$, to $1/2$ at $t=a,b$, and to $0$ outside $[a,b]$. It is uniformly bounded, so dominated convergence in the [spectral measure of a normal operator](../../../../../../spectral-measure-of-a-normal-operator.md) gives the strong limit

$$
E((a,b))+\frac12E(\{a\})+\frac12E(\{b\})
=\boxed{\frac12[E((a,b))+E([a,b])]}.
$$

Applying this operator to $v$ proves the claimed [Stone formula](../../../../../../stone-formula.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 358](../../../paper-358-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
