<h1 id="6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $M$ bound the [operator norm](../../../../../../operator-norm.md) of $D^2F$; the bound on individual second derivatives supplies such an $M$ depending also on dimension. The [Taylor theorem](../../../../../../taylor-theorem.md) with integral remainder gives

$$
F(p)=F(0)+DF(0)\cdot p+\int_0^1(1-t)\,p^TD^2F(tp)p\,dt.
$$

Thus [quadratic growth from a bounded Hessian](../../../../../../quadratic-growth-from-a-bounded-hessian.md) gives

$$
|F(p)|\leq|F(0)|+|DF(0)||p|+\frac M2|p|^2\leq C(1+|p|^2).
$$

Since $\Omega$ is bounded it has finite measure, and a function in the [Sobolev space](../../../../../../sobolev-space-split.md) $H^1(\Omega)$ has $Du\in L^2(\Omega)$. The given lower bound also implies that the integrand is nonnegative. Consequently

$$
\boxed{0\leq\mathcal F(u)=\int_\Omega F(Du)\leq C\left(|\Omega|+\|Du\|_2^2\right)<\infty.}
$$

For later use the same [Hessian](../../../../../../hessian-matrix.md) bound yields $|DF(p)|\leq|DF(0)|+M|p|$, hence $DF(Du)\in L^2(\Omega)$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6](../../6.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
