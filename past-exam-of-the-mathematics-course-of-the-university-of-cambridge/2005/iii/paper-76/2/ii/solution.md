<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take zero mean flow locally and incompressible fluctuations. Subtracting the averaged induction equation gives

$$
(\partial_t-\eta\nabla^2)\mathbf b=\nabla\times(\mathbf u\times\overline{\mathbf B})+\nabla\times(\mathbf u\times\mathbf b-\langle\mathbf u\times\mathbf b\rangle).
$$

The [first-order smoothing approximation](../../../../../../first-order-smoothing-approximation.md) omits the second term on the right when solving for $\mathbf b$, but retains $\langle\mathbf u\times\mathbf b\rangle$ in the mean equation. For a locally uniform, slowly changing mean [magnetic field](../../../../../../magnetic-field.md) the forcing becomes $(\overline{\mathbf B}\cdot\nabla)\mathbf u$.

There are two controlled ways to make the omitted fluctuation term small. At small eddy [magnetic Reynolds number](../../../../../../magnetic-reynolds-number.md) $R_m=u_{\mathrm{rms}}\ell/\eta$, diffusion gives $b/B\sim R_m$, so the omitted $ub/\ell$ is smaller than the retained $uB/\ell$ by $R_m$. Alternatively, if $u_{\mathrm{rms}}\tau/\ell\ll1$ for the fluctuation response time $\tau$, then $b/B\sim u_{\mathrm{rms}}\tau/\ell$ and the short-memory response is perturbative. Mean-field scale separation is additionally required. Merely calling the [turbulence](../../../../../../turbulence-split.md) weak or assuming that the mean [magnetic field](../../../../../../magnetic-field.md) is small does not justify the omission.

With homogeneous initial transients removed, the causal linear solution is

$$
b_i(t)=\overline B_j\int_0^\infty e^{\eta\tau\nabla^2}\partial_j u_i(t-\tau)\,d\tau.
$$

Insert this into the electromotive correlation. [Isotropy](../../../../../../isotropy.md) gives $\alpha_{ij}=\alpha\delta_{ij}$, so taking the [trace](../../../../../../matrix-trace.md) yields the [helicity formula for isotropic first-order smoothing](../../../../../../helicity-formula-for-isotropic-first-order-smoothing.md):

$$
3\alpha=\int_0^\infty\epsilon_{imn}\left\langle u_m(t)\partial_i e^{\eta\tau\nabla^2}u_n(t-\tau)\right\rangle d\tau.
$$

Using the alternating-tensor sign gives

$$
\boxed{\alpha=-\frac13\int_0^\infty\left\langle\mathbf u(t)\cdot\nabla\times e^{\eta\tau\nabla^2}\mathbf u(t-\tau)\right\rangle d\tau.}
$$

The minus sign follows from $\epsilon_{imn}=-\epsilon_{min}$. This derivation specifies the diffusion and correlation weighting, rather than asserting that alpha is proportional to instantaneous helicity for arbitrary [turbulence](../../../../../../turbulence-split.md).

If $\eta\tau/\ell^2\ll1$, diffusion over a [correlation time](../../../../../../correlation-time.md) is negligible. Define the helicity [correlation time](../../../../../../correlation-time.md) by

$$
\tau_H\langle\mathbf u\cdot\boldsymbol\varpi\rangle=\int_0^\infty\langle\mathbf u(t)\cdot\boldsymbol\varpi(t-\tau)\rangle d\tau,\qquad\boldsymbol\varpi=\nabla\times\mathbf u.
$$

For an ordinary decaying correlation with nonzero mean [kinetic helicity](../../../../../../hydrodynamical-helicity.md), this gives the familiar estimate

$$
\boxed{\alpha=-\frac{\tau_H}{3}\langle\mathbf u\cdot\boldsymbol\varpi\rangle.}
$$

It is the [kinetic helicity](../../../../../../hydrodynamical-helicity.md), not [magnetic helicity](../../../../../../magnetic-helicity.md). Opposite flow handedness reverses the [alpha effect](../../../../../../alpha-effect.md). The time-integral formula remains meaningful if the equal-time helicity vanishes or its correlation changes sign, when replacing it by a single positive [correlation time](../../../../../../correlation-time.md) may fail. In the same weak-diffusion short-memory approximation the gradient forcing $-(\mathbf u\cdot\nabla)\overline{\mathbf B}$ gives $\beta=\frac13\int_0^\infty\langle\mathbf u(t)\cdot\mathbf u(t-\tau)\rangle d\tau\simeq\tau_Uu_{\mathrm{rms}}^2/3$; the two [correlation times](../../../../../../correlation-time.md) need not be equal.

In the small-$R_m$, slowly varying quasistatic regime, diffusion is instead essential. The response gives

$$
\alpha=-\frac1{3\eta}\left\langle\mathbf u\cdot(-\nabla^2)^{-1}\boldsymbol\varpi\right\rangle.
$$

For velocity concentrated at wavenumber $k_0$, this becomes $\alpha=-\langle\mathbf u\cdot\boldsymbol\varpi\rangle/(3\eta k_0^2)$. Its effective memory is the [magnetic diffusion](../../../../../../magnetic-diffusion.md) time on the eddy scale. The controlled low-$R_m$ setting is developed in [Moffatt's analysis of turbulent dynamo action](https://www.damtp.cam.ac.uk/user/hkm2/PDFs/Moffatt_1970_JFM_41_435.pdf); the causal-response calculation above also covers short-memory [turbulence](../../../../../../turbulence-split.md) without assuming that diffusion is always negligible.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
