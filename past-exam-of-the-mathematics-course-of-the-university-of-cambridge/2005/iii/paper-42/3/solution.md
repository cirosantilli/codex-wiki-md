<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Put $S_1=\sum_iY_i$, $S_2=\sum_iY_i^2$ and $R=\sqrt{S_2}$. Apart from a data-only constant, the [log-likelihood](../../../../../log-likelihood.md) is

$$
\ell(\mu)=-n\log\mu-\frac{S_2}{2\mu^2}+\frac{S_1}{\mu}-\frac n2.
$$

The natural parameters in the ambient two-parameter [exponential family](../../../../../exponential-family-split.md) of [normal distributions](../../../../../normal-distribution.md) are $\eta_1=1/\mu$ and $\eta_2=-1/(2\mu^2)$, restricted to the nonaffine curve $\eta_2=-\eta_1^2/2$, $\eta_1>0$. Its parametrization has rank one. Thus this is a one-dimensional [curved exponential family](../../../../../curved-exponential-family.md) inside a two-dimensional full family.

The [Fisher-Neyman factorization theorem](../../../../../fisher-neyman-factorization-theorem.md) makes $(S_1,S_2)$ sufficient. For two samples $y,z$, the parameter-dependent part of their log density ratio is $\Delta S_1/\mu-\Delta S_2/(2\mu^2)$. A polynomial in $1/\mu$ is constant on $(0,\infty)$ only if both nonconstant coefficients vanish. The [likelihood-ratio criterion for minimal sufficiency](../../../../../likelihood-ratio-criterion-for-minimal-sufficiency.md) therefore proves **$(S_1,S_2)$ is minimal sufficient**.

Write $Y_i=\mu Z_i$ with [independent](../../../../../independent-random-variables.md) $Z_i\sim N(1,1)$. Since $\mu>0$, $a=\sqrt n\sqrt{\sum_iZ_i^2}/\sum_iZ_i$ has a [probability distribution](../../../../../probability-distribution.md) [independent](../../../../../independent-random-variables.md) of $\mu$: it is an [ancillary statistic](../../../../../ancillary-statistic.md). The denominator is nonzero almost surely. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $|a|\geq1$; on the requested positive branch, $S_1>0$ and $a\geq1$.

The [likelihood](../../../../../likelihood-function.md) equation is $n\mu^2+S_1\mu-S_2=0$. Its positive root is

$$
\widehat\mu=\frac{\sqrt{S_1^2+4nS_2}-S_1}{2n}
=\frac R{q\sqrt n},\qquad q=\frac{\sqrt{1+4a^2}+1}{2a}.
$$

There is exactly one positive root. The sign of the [score function](../../../../../informant-function.md) changes from positive to negative there, and $\ell\to-\infty$ at both ends of $(0,\infty)$ when $S_2>0$, so it is the unique [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md). The useful identities are

$$
q^2-q/a-1=0,\qquad S_2=nq^2\widehat\mu^2,\qquad S_1=nq\widehat\mu/a.
$$

Substitution yields, dropping the constant $-n/2$,

$$
\boxed{\ell(\mu;v,a)=-n\log\mu-\frac{nq^2v^2}{2\mu^2}+\frac{nqv}{a\mu},\qquad v=\widehat\mu.}
$$

Differentiating twice and using $q/a=q^2-1$ at the fitted value gives the [observed information](../../../../../observed-fisher-information.md)

$$
j(v;v,a)=-\ell_{\mu\mu}(v;v,a)=\frac{n(1+q^2)}{v^2}.
$$

The scalar [P-star approximation](../../../../../p-star-approximation.md) uses $\sqrt{j(v)}\exp\{\ell(\mu;v,a)-\ell(v;v,a)\}$. Consequently, with its normalizing factor explicitly retained,

$$
\boxed{p^*(v\mid a;\mu)=\frac{C_n(a)}{v}\sqrt{\frac{n(1+q^2)}{2\pi}}
\exp\left\{n\log\frac v\mu-\frac{nq^2}{2}\left(\frac{v^2}{\mu^2}-1\right)+\frac{nq}{a}\left(\frac v\mu-1\right)\right\},\quad v>0.}
$$

Here $C_n(a)$ is chosen to make the density integrate to one, and is [independent](../../../../../independent-random-variables.md) of $\mu$. To see this without assuming an approximate normalizer, define

$$
J_n(a)=\int_0^\infty z^{n-1}\exp\left(-\frac{nq^2z^2}{2}+\frac{nqz}{a}\right)dz.
$$

The integral is finite and positive, and normalized $p^*$ is exactly

$$
p^*(v\mid a;\mu)=\frac{(v/\mu)^{n-1}}{\mu J_n(a)}\exp\left[-\frac{nq^2}{2}(v/\mu)^2+\frac{nq}{a}(v/\mu)\right].
$$

Indeed $C_n(a)=\{\sqrt{n(1+q^2)/(2\pi)}\exp[nq^2/2-nq/a]J_n(a)\}^{-1}$.

There is a direct check of this [conditional scale density in a curved Gaussian family](../../../../../conditional-scale-density-in-a-curved-gaussian-family.md). In [polar coordinates](../../../../../polar-coordinates.md) $y=Ru$, the sample density times volume element is proportional to $\mu^{-n}R^{n-1}\exp[-R^2/(2\mu^2)+R\sum_i u_i/\mu]dR\,d\omega(u)$. Conditioning on $a$ fixes $\sum_i u_i=\sqrt n/a$. The remaining angular factor is [independent](../../../../../independent-random-variables.md) of $R,\mu$, while $R=q\sqrt n\,v$. Thus the exact conditional radial density has the same normalized form. For $n=1$ the positive ancillary branch fixes the positive sign and the same one-dimensional radial calculation applies. **In this scale model the normalized $p^*$ expression equals the exact conditional density**, not merely its leading approximation.

For $t>0$, compute its conditional distribution by one-dimensional quadrature:

$$
\boxed{\mathbb P_\mu(\widehat\mu\leq t\mid a)\approx
\frac{\displaystyle\int_0^{t/\mu}z^{n-1}e^{-nq^2z^2/2+nqz/a}\,dz}{J_n(a)}.}
$$

It is zero for $t\leq0$; with the conditional-density calculation just given, this normalized formula is exact for almost every admissible $a$. Numerically, subtract the maximum log integrand before exponentiating to avoid overflow. The sampling probability still depends on the stipulated true $\mu$; replacing it by a fitted value would be a separate plug-in inference step.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
