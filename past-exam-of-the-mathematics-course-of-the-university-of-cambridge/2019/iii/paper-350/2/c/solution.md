<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the shape-rate convention for the [Gamma distribution](../../../../../../gamma-distribution.md). Define

$$
B=A^TA,\qquad u_* = B^{-1}A^Tm,\qquad
r=m-Au_*,\qquad
a=\alpha+\frac k2,\qquad
b(u)=\beta+\frac12\|m-Au\|^2.
$$

The zero [null space](../../../../../../kernel-of-a-linear-map.md) assumption makes $B$ a [positive-definite matrix](../../../../../../positive-definite-matrix.md), and $u_*$ is the unique [ordinary least squares](../../../../../../ordinary-least-squares.md) solution. The [Gaussian likelihood](../../../../../../gaussian-likelihood.md) contributes $\gamma^{k/2}$, which must be retained because $\gamma$ is unknown. Multiplying it by the [improper prior](../../../../../../improper-prior.md) and the [Gamma distribution](../../../../../../gamma-distribution.md) gives the [normal-gamma posterior with a flat prior](../../../../../../normal-gamma-posterior-with-a-flat-prior.md):

$$
\boxed{\pi^m(u,\gamma)=\frac1{\mathcal Z}\gamma^{a-1}e^{-\gamma b(u)},\qquad u\in\mathbb R^d,\quad\gamma>0.}
$$

Here the constant density of the [improper prior](../../../../../../improper-prior.md) cancels on normalization. Put

$$
b_0=\beta+\tfrac12\|r\|^2>0,\qquad
s=a-\tfrac d2=\alpha+\tfrac{k-d}{2}>0.
$$

The [normal equation](../../../../../../normal-equation.md) $A^Tr=0$ makes the residual orthogonal to the range of $A$. The [orthogonal decomposition by a closed subspace](../../../../../../orthogonal-decomposition-by-a-closed-subspace.md) into that range and its [orthogonal complement](../../../../../../orthogonal-complement.md) gives

$$
b(u)=b_0+\tfrac12(u-u_*)^TB(u-u_*).
$$

Integration over $u$ by the [Gaussian integral](../../../../../../gaussian-integral.md), followed by integration over $\gamma$ using the [Gamma distribution](../../../../../../gamma-distribution.md), yields

$$
\mathcal Z=\frac{(2\pi)^{d/2}}{\sqrt{\det B}}\frac{\Gamma(s)}{b_0^s}<\infty.
$$

Thus the [posterior distribution](../../../../../../bayesian-posterior.md) is proper, despite the [improper prior](../../../../../../improper-prior.md); here $k\geq d$ follows from the zero [null space](../../../../../../kernel-of-a-linear-map.md) assumption.

[Completing the square](../../../../../../completing-the-square.md) in $u$ and collecting the powers of $\gamma$ give the two [conditional distributions](../../../../../../conditional-distribution.md):

$$
\boxed{u\mid\gamma,m\sim\mathcal N(u_*,\gamma^{-1}B^{-1}),\qquad
\gamma\mid u,m\sim\operatorname{Gamma}(a,b(u)).}
$$

Explicitly their [probability density functions](../../../../../../probability-density-function.md) are

$$
\pi(u\mid\gamma,m)=\frac{\gamma^{d/2}\sqrt{\det B}}{(2\pi)^{d/2}}
e^{-\frac\gamma2(u-u_*)^TB(u-u_*)},\qquad
\pi(\gamma\mid u,m)=\frac{b(u)^a}{\Gamma(a)}\gamma^{a-1}e^{-b(u)\gamma}.
$$

For a joint [maximum a posteriori estimate](../../../../../../maximum-a-posteriori-estimate.md) relative to $du\,d\gamma$, first fix $\gamma>0$. The unique maximizing $u$ is $u_*$. The remaining log density is $(a-1)\log\gamma-b_0\gamma$ plus a constant. Consequently, if $a>1$,

$$
\boxed{\widehat u_{\mathrm{MAP}}=u_*,\qquad
\widehat\gamma_{\mathrm{MAP}}=\frac{\alpha+k/2-1}{\beta+\|r\|^2/2}.}
$$

The stated assumptions do not always imply $a>1$. If $a=1$, the supremum occurs as $\gamma\downarrow0$ but is not attained on $\gamma>0$; if $a<1$, the density is unbounded there. In either case there is no joint [maximum a posteriori estimate](../../../../../../maximum-a-posteriori-estimate.md) in the stated parameter space. Calling zero a boundary mode does not make it an admissible positive precision.

If “MAP estimators” instead means separate modes of the [marginal distributions](../../../../../../marginal-distribution.md), integration gives

$$
\pi(u\mid m)\propto\left[b_0+\tfrac12(u-u_*)^TB(u-u_*)\right]^{-a},\qquad
\gamma\mid m\sim\operatorname{Gamma}(s,b_0).
$$

Thus the marginal [maximum a posteriori estimate](../../../../../../maximum-a-posteriori-estimate.md) of $u$ is always $u_*$, and that of $\gamma$ is $(s-1)/b_0$ when $s>1$, with the same nonattainment at zero when $s\leq1$. Joint and marginal maximization are different operations; the usual joint interpretation gives the preceding boxed pair.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 350](../../../paper-350-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
