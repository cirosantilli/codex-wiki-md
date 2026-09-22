<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $y=\psi_s$ and retain the [Landweber relaxation parameter](../../../../../../landweber-relaxation-parameter.md) $\tau$. The printed $\|A\|<2$ allows the fixed choice $\tau=1/2$, since then $\tau\|A\|^2<2$. It does not justify a unit step: the scalar [linear operator](../../../../../../linear-operator.md) $A=3/2$ has norm below $2$, but unit-step error is multiplied by $1-|A|^2=-5/4$ and diverges. We use $0<\tau<2/\|A\|^2$ throughout.

From the recurrence and $f_0=0$, induction yields the closed form

$$
\boxed{f_n=R_ny,\qquad R_n=\tau\sum_{k=0}^{n-1}(I-\tau A^*A)^kA^*.}
$$

For the [compact operator](../../../../../../compact-operator-split.md) in part ii, take a [singular system of a compact operator](../../../../../../singular-system-of-a-compact-operator.md) with $Av_j=\sigma_ju_j$, $A^*u_j=\sigma_jv_j$ and $\sigma_j>0$. Thus $\sigma_j^2$ are the [eigenvalues](../../../../../../eigenvalue.md) of $A^*A$; this fixes the notation implicit in the printed hint. In the singular component $j$, the recurrence is

$$
\langle f_{m+1},v_j\rangle=(1-\tau\sigma_j^2)\langle f_m,v_j\rangle+\tau\sigma_j\langle y,u_j\rangle.
$$

Summing the [geometric series](../../../../../../geometric-series.md) gives the [Landweber spectral filter](../../../../../../landweber-spectral-filter.md)

$$
\boxed{R_ny=\sum_j\frac{1-(1-\tau\sigma_j^2)^n}{\sigma_j}\langle y,u_j\rangle v_j.}
$$

There is no contribution from data in $\ker A^*$ or from $\ker A$ in the reconstruction. Starting at zero is what selects the [minimum-norm least-squares solution](../../../../../../minimum-norm-least-squares-solution.md).

For fixed $\sigma_j>0$, $|1-\tau\sigma_j^2|<1$, so the numerator tends to $1$. The assumption $y\in D(A^\dagger)$ is the [Picard criterion](../../../../../../picard-criterion.md)

$$
\sum_j\frac{|\langle y,u_j\rangle|^2}{\sigma_j^2}<\infty,
$$

with an arbitrary additional component in $\ker A^*$. The squared reconstruction error is

$$
\|R_ny-A^\dagger y\|^2=\sum_j|1-\tau\sigma_j^2|^{2n}\frac{|\langle y,u_j\rangle|^2}{\sigma_j^2}.
$$

Each term tends to zero and is bounded by a summable term from the [Picard criterion](../../../../../../picard-criterion.md). The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) therefore proves $R_ny\to A^\dagger y$, where $A^\dagger$ is the [Moore–Penrose inverse of an operator](../../../../../../moore-penrose-inverse-of-an-operator.md).

For each finite $n$, the [regularization of an inverse problem](../../../../../../regularization-of-an-inverse-problem.md) is stable. Set $t=\tau\sigma^2\in(0,2)$. The [geometric series](../../../../../../geometric-series.md) and $|1-t|\leq1$ imply

$$
|1-(1-t)^n|\leq\min(nt,2),\qquad
\left|\frac{1-(1-\tau\sigma^2)^n}{\sigma}\right|\leq\min(n\tau\sigma,2/\sigma)\leq\sqrt{2\tau n}.
$$

Consequently the [Landweber noise amplification bound](../../../../../../landweber-noise-amplification-bound.md) in this general step-size convention is $\|R_n\|\leq\sqrt{2\tau n}$. If additionally $\tau\|A\|^2\leq1$, the sharper numerator bound $\min(nt,1)$ gives $\|R_n\|\leq\sqrt{\tau n}$.

To see the [regularization parameter](../../../../../../regularization-parameter.md) directly, put $\alpha=1/(\tau n)$. Modes with $\sigma^2\ll\alpha$ have numerator approximately $n\tau\sigma^2$, so their inverse coefficient is approximately $\sigma/\alpha$ rather than $1/\sigma$. Each fixed nonzero mode is eventually restored as $\alpha\downarrow0$. Thus

$$
\boxed{\alpha=\frac1{\tau n}\quad\text{and, for fixed }\tau,\quad\alpha\propto\frac1n.}
$$

The finite iterates suppress unstable small [singular values](../../../../../../singular-value.md); infinitely many iterations remove this suppression. For noisy data $\|y^\delta-y\|\leq\delta$, the [noise-bias decomposition for linear regularization](../../../../../../noise-bias-decomposition-for-linear-regularization.md) gives

$$
\|R_ny^\delta-A^\dagger y\|\leq\sqrt{2\tau n}\,\delta+\|R_ny-A^\dagger y\|.
$$

Choosing $n(\delta)\to\infty$ and $\delta^2n(\delta)\to0$ proves noisy-data convergence. **The reciprocal iteration index is a regularization parameter, and early stopping controls noise amplification.**

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
