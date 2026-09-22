<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Separate the [velocity field](../../../../../../velocity-field.md) and [magnetic field](../../../../../../magnetic-field.md) into mean and fluctuating parts,

$$
\mathbf u=\overline{\mathbf U}+\mathbf u',\qquad \mathbf B=\overline{\mathbf B}+\mathbf b',\qquad \langle\mathbf u'\rangle=\langle\mathbf b'\rangle=0.
$$

Assume the [Reynolds averaging](../../../../../../reynolds-averaging.md) operation commutes with derivatives and has the usual product rules. Averaging the [resistive induction equation](../../../../../../resistive-induction-equation.md) gives

$$
\partial_t\overline{\mathbf B}=\nabla\times(\overline{\mathbf U}\times\overline{\mathbf B}+\boldsymbol{\mathcal E})+\eta\nabla^2\overline{\mathbf B},\qquad \boldsymbol{\mathcal E}=\langle\mathbf u'\times\mathbf b'\rangle.
$$

The [mean-field electromotive force](../../../../../../mean-field-electromotive-force.md) is the contribution through which small-scale motions affect the large-scale [magnetic field](../../../../../../magnetic-field.md). If the mean field varies slowly compared with the fluctuation scales, its response can be expanded in the mean field and its spatial derivatives. With homogeneous isotropic statistics, the leading terms are

$$
\boxed{\boldsymbol{\mathcal E}=\alpha\overline{\mathbf B}-\beta\nabla\times\overline{\mathbf B}.}
$$

The [alpha effect](../../../../../../alpha-effect.md) is the term parallel to the mean field. Since an electromotive response is a polar vector whereas a [magnetic field](../../../../../../magnetic-field.md) is axial, isotropic $\alpha$ is a [pseudoscalar](../../../../../../pseudoscalar.md); reflection-symmetric statistics force it to vanish. Nonzero [kinetic helicity](../../../../../../hydrodynamical-helicity.md) supplies the required handedness. The [turbulent diffusivity](../../../../../../eddy-diffusivity.md) term transports and smooths the mean field; constant positive $\beta$ adds $\beta\nabla^2\overline{\mathbf B}$ to its evolution.

One controlled calculation is [first-order smoothing](../../../../../../first-order-smoothing-approximation.md). For negligible mean flow, omit the fluctuating nonlinear product in the fluctuation induction equation, obtaining

$$
(\partial_t-\eta\nabla^2)\mathbf b'=\nabla\times(\mathbf u'\times\overline{\mathbf B}).
$$

For [incompressible flow](../../../../../../incompressible-flow.md) this forcing is $(\overline{\mathbf B}\cdot\nabla)\mathbf u'-(\mathbf u'\cdot\nabla)\overline{\mathbf B}$. A short-memory approximation of duration $\tau$ replaces the inverse temporal response by multiplication by $\tau$. Substitution into the [mean-field electromotive force](../../../../../../mean-field-electromotive-force.md) then uses isotropy:

$$
\begin{aligned}
\epsilon_{ijk}\langle u'_j\partial_\ell u'_k\rangle&=-\frac13\langle\mathbf u'\cdot\nabla\times\mathbf u'\rangle\delta_{i\ell},\\
\langle u'_ju'_\ell\rangle&=\frac13\langle|\mathbf u'|^2\rangle\delta_{j\ell}.
\end{aligned}
$$

Consequently

$$
\boxed{\alpha\simeq-\frac\tau3\langle\mathbf u'\cdot\nabla\times\mathbf u'\rangle,\qquad \beta\simeq\frac\tau3\langle|\mathbf u'|^2\rangle.}
$$

The first sign follows by taking the trace of the alpha-response tensor: $\epsilon_{ijk}u'_j\partial_i u'_k=-\mathbf u'\cdot\nabla\times\mathbf u'$. This establishes the [helicity formula for isotropic first-order smoothing](../../../../../../helicity-formula-for-isotropic-first-order-smoothing.md). Its controlled regimes include small [magnetic Reynolds number](../../../../../../magnetic-reynolds-number.md) or sufficiently short fluctuation [correlation time](../../../../../../correlation-time.md). Outside such a closure, the coefficients involve response-weighted time correlations; an instantaneous helicity formula is not universal.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
