<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $R^2=\sum_ix_i^2$ and impose tracelessness by a [Lagrange multiplier](../../../../lagrange-multiplier.md) $\zeta$. Differentiating $V-\zeta\sum_i x_i$ gives

$$
\boxed{4b x_i^3+(4aR^2-2m^2)x_i-\zeta=0\qquad(i=1,\ldots,5).}
$$

For $b\ne0$, each [eigenvalue](../../../../eigenvalue.md) is a real root of the same nonzero cubic [polynomial](../../../../polynomial-split.md), so at most three distinct values occur at any stationary point, in particular at any existing minimum. If the multiplicities are $n_1,\ldots,n_k$, the unbroken subgroup is the block centralizer

$$
\boxed{S\bigl(U(n_1)\times\cdots\times U(n_k)\bigr),\qquad
k\le3,\quad\sum_\alpha n_\alpha=5.}
$$

Its connected Lie algebra is $\bigoplus_\alpha\mathfrak{su}(n_\alpha)\oplus\mathfrak u(1)^{k-1}$. The partitions allowed by this upper bound are $5$, $4+1$, $3+2$, $3+1+1$, and $2+2+1$. These are candidate patterns, not a proof that every one is a stable minimum for given couplings. For three distinct roots, the absent quadratic coefficient also implies that their unweighted sum is zero; tracelessness imposes an additional multiplicity-weighted relation.

**The unrestricted printed claim has an exception.** If $b=0$, $a>0$ and $m>0$, every traceless matrix with $R^2=m^2/(2a)$ is a global minimum. For example

$$
\Phi_d=\frac{m}{\sqrt{20a}}\operatorname{diag}(-2,-1,0,1,2)
$$

has five distinct [eigenvalues](../../../../eigenvalue.md) and attains that minimum. Its unbroken subgroup is the maximal torus $U(1)^4$. The cubic argument therefore requires a nonzero $b$, or another condition excluding the identically vanishing stationarity polynomial. Couplings for which the potential is unbounded below have no global minimum to classify.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
