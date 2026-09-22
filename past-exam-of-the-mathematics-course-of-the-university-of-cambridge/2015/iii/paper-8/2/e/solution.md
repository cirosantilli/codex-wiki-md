<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Work in the [Banach space](../../../../../../banach-space-split.md) $\mathcal B_T$ of bounded strongly measurable maps $[0,T]\to L^2_{x,v}$, with norm $\|g\|_{\mathcal B_T}=\sup_{0\leq t\leq T}\|g(t)\|_2$. Keeping actual representatives at every time matches the pointwise-in-time mild formulation. The [Boltzmann Volterra operator](../../../../../../boltzmann-volterra-operator.md) is bounded on this space, and the [factorial bound for a Volterra iterate](../../../../../../factorial-bound-for-a-volterra-iterate.md) gives

$$
\|\tau^n\|_{\mathcal B_T\to\mathcal B_T}\leq\frac{(CT)^n}{n!}.
$$

Thus the [Volterra series for the linear Boltzmann equation](../../../../../../volterra-series-for-the-linear-boltzmann-equation.md) converges in [operator norm](../../../../../../operator-norm.md) for every finite $T$, even when $CT\geq1$. Set

$$
\boxed{f=\sum_{n=0}^\infty\tau^nF(f_0,a).}
$$

For its partial sums, $(I-\tau)\sum_{n=0}^N\tau^nF=F-\tau^{N+1}F$. The remainder tends to zero by the factorial estimate. Hence $(I-\tau)f=F$, precisely the required characteristic integral equation.

The norm bound in (b) gives **an explicit choice of the existence constant**:

$$
\boxed{\sup_{0\leq t\leq T}\|f(t)\|_2
\leq e^{CT}\|f_0\|_2,\qquad C_T=e^{CT}.}
$$

Also $f(0)=f_0$, since every term with $n\geq1$ vanishes at zero and the damping interval has length zero. This proves existence in the paper's weak, characteristic-integral sense. With merely measurable nonnegative $a$, that sense does not itself require a continuous initial trace; that trace follows under the additional local characteristic-integrability condition described in (b).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
