<h1 id="a/3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Substitute $y=\sum_{k\geq0}a_kx^k$ and compare the coefficient of $x^k$. The two [derivative](../../../../../derivative.md) terms give $(k+1)^2a_{k+1}$, while the remaining terms give $(n-k)a_k$. Thus

$$
\boxed{a_{k+1}=\frac{k-n}{(k+1)^2}a_k,\qquad a_0=1.}
$$

Iterating the recurrence gives

$$
\boxed{a_k=\frac{(-1)^kn!}{(n-k)!(k!)^2}=\frac{(-1)^k}{k!}\binom nk\quad(0\leq k\leq n),\qquad a_k=0\quad(k>n).}
$$

Indeed the recurrence first vanishes at $k=n$ and then remains zero. Consequently the [Laguerre polynomial](../../../../../laguerre-polynomial.md) is

$$
\boxed{L_n(x)=\sum_{k=0}^n\frac{(-1)^k}{k!}\binom nk x^k,}
$$

with exact degree $n$ and leading coefficient $(-1)^n/n!$. This is the regular power-series branch normalized at zero; the second branch at the repeated [indicial root](../../../../../indicial-root.md) is not an additional [analytic](../../../../../holomorphic-function-split.md) solution with this normalization.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the differential equations and applications course of the University of Oxford](../../../../split.md)
6. [Differential equations and applications course of the University of Oxford](../../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
