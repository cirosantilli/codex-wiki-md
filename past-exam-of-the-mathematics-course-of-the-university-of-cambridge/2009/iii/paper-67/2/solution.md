<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $m_0=\mu_0\rho$ and treat the imposed mean [magnetic field](../../../../../magnetic-field.md) as uniform on the forcing scale. In [first-order smoothing](../../../../../first-order-smoothing-approximation.md), retain terms linear in the fluctuating fields in their equations, while keeping their quadratic correlation when calculating the [mean-field electromotive force](../../../../../mean-field-electromotive-force.md). The inertial fluctuation, nonlinear induction term and quadratic fluctuating [Lorentz force density](../../../../../lorentz-force-density.md) are neglected in the steady response. The linear magnetic force is

$$
\frac1{m_0}(\nabla\times\mathbf b)\times\mathbf B
=\frac1{m_0}(\mathbf B\cdot\nabla)\mathbf b-\nabla\frac{\mathbf B\cdot\mathbf b}{m_0}.
$$

Absorb the gradient into the total pressure. The resulting equations are

$$
0=-\rho^{-1}\nabla P+m_0^{-1}(\mathbf B\cdot\nabla)\mathbf b+\nu\nabla^2\mathbf u+\mathbf f,
\qquad
0=(\mathbf B\cdot\nabla)\mathbf u+\eta\nabla^2\mathbf b+\mathbf g,
$$

with $\nabla\cdot\mathbf u=\nabla\cdot\mathbf b=0$. Taking the divergence of the first equation gives $\nabla^2P=0$ for solenoidal forcing. In a periodic or homogeneous Fourier calculation its nonconstant part therefore vanishes.

For each [Fourier mode](../../../../../fourier-mode.md) with wavevector $\mathbf q$, $|\mathbf q|=k$, define $\ell=\mathbf B\cdot\mathbf q$ and

$$
D=\nu\eta k^4+\frac{\ell^2}{m_0}>0.
$$

Solving the two coupled linear equations gives the [monochromatic coupled magnetic and velocity response](../../../../../monochromatic-coupled-magnetic-and-velocity-response.md)

$$
\boxed{\widehat{\mathbf u}=\frac{\eta k^2\widehat{\mathbf f}+i\ell\widehat{\mathbf g}/m_0}{D},
\qquad
\widehat{\mathbf b}=\frac{\nu k^2\widehat{\mathbf g}+i\ell\widehat{\mathbf f}}{D}.}
$$

The magnetic coupling suppresses modes with large projection of their wavevector along the imposed field.

To calculate the [mean-field electromotive force](../../../../../mean-field-electromotive-force.md), group each pair of opposite wavevectors into a real mode and average its spatial phase. Put $\mathbf n=\mathbf q/k$, and define its forcing correlations

$$
\mathbf C_{\mathbf q}=\langle\mathbf f_{\mathbf q}\times\mathbf g_{\mathbf q}\rangle,
\quad
h_f(\mathbf q)=\langle\mathbf f_{\mathbf q}\cdot\nabla\times\mathbf f_{\mathbf q}\rangle,
\quad
h_g(\mathbf q)=\langle\mathbf g_{\mathbf q}\cdot\nabla\times\mathbf g_{\mathbf q}\rangle.
$$

For any solenoidal real mode $\mathbf v=\mathbf a\cos(\mathbf q\cdot\mathbf x)+\mathbf c\sin(\mathbf q\cdot\mathbf x)$, its two amplitude vectors are perpendicular to $\mathbf q$. Direct multiplication gives

$$
\langle\mathbf v\times(\mathbf B\cdot\nabla)\mathbf v\rangle
=-\mathbf n(\mathbf n\cdot\mathbf B)\langle\mathbf v\cdot\nabla\times\mathbf v\rangle.
$$

Also, integration by parts gives $\langle(L\mathbf g)\times(L\mathbf f)\rangle=-\ell^2\langle\mathbf f\times\mathbf g\rangle$, where $L=\mathbf B\cdot\nabla$. Expanding the response products therefore yields

$$
\boxed{\boldsymbol{\mathcal E}_{\mathbf q}
=\frac{\nu\eta k^4-\ell^2/m_0}{D^2}\mathbf C_{\mathbf q}
+\frac{k^2}{D^2}\mathbf n(\mathbf n\cdot\mathbf B)
\left(\frac{\nu}{m_0}h_g(\mathbf q)-\eta h_f(\mathbf q)\right).}
$$

Summing over independent real modes, or integrating over their angular spectrum, is the required general answer for $\langle\mathbf u\times\mathbf b\rangle$.

At zero field, $\boldsymbol{\mathcal E}(0)=\sum_{\mathbf q}\mathbf C_{\mathbf q}/(\nu\eta k^4)$. Thus the stated zero-field condition removes the unweighted sum of the cross correlations. For anisotropic correlated forcing it does not necessarily remove their differently weighted sum at nonzero field. The displayed general formula retains that allowed contribution. It disappears if cross forcing is absent mode by mode, or under the jointly isotropic statistics assumed for the final part.

The helicity content can also be expressed directly using the actual fluctuating fields. Define their [kinetic helicity](../../../../../hydrodynamical-helicity.md) $H_u(\mathbf q)=\langle\mathbf u_{\mathbf q}\cdot\nabla\times\mathbf u_{\mathbf q}\rangle$ and [current helicity](../../../../../current-helicity.md) $H_b(\mathbf q)=\langle\mathbf b_{\mathbf q}\cdot\nabla\times\mathbf b_{\mathbf q}\rangle$. Substitute $\mathbf f=\nu k^2\mathbf u-L\mathbf b/m_0$ and $\mathbf g=\eta k^2\mathbf b-L\mathbf u$ into their cross correlation. This gives the exact identity

$$
\left(\nu\eta k^4-\frac{\ell^2}{m_0}\right)\boldsymbol{\mathcal E}_{\mathbf q}-\mathbf C_{\mathbf q}
=k^2\mathbf n(\mathbf n\cdot\mathbf B)
\left(\frac{\eta}{m_0}H_b(\mathbf q)-\nu H_u(\mathbf q)\right).
$$

It shows the competing kinetic and magnetic contributions without introducing a spurious singularity when the factor on the left vanishes. For a monochromatic field, $\mathbf a_b=\nabla\times\mathbf b/k^2$ is a [magnetic vector potential](../../../../../magnetic-vector-potential.md), so $H_b=k^2\langle\mathbf a_b\cdot\mathbf b\rangle$: [current helicity](../../../../../current-helicity.md) is $k^2$ times [magnetic helicity](../../../../../magnetic-helicity.md). In the isotropic weak-field limit, with zero-field fluctuations $\mathbf u_0,\mathbf b_0$, the scalar [alpha effect](../../../../../alpha-effect.md) is

$$
\alpha(0)=-\frac{\langle\mathbf u_0\cdot\nabla\times\mathbf u_0\rangle}{3\eta k^2}
+\frac{\langle\mathbf b_0\cdot\nabla\times\mathbf b_0\rangle}{3\nu m_0 k^2}.
$$

This identifies both signs and their different viscous and magnetic relaxation times.

For jointly isotropic forcing let $h_f,h_g$ now denote the total forcing helicities, and set $S_h=\nu h_g/m_0-\eta h_f$. The cross-forcing contribution is even in $\mathbf B$, whereas isotropy requires any vector depending only on $\mathbf B$ to be parallel to it and odd under reversal. Hence that contribution vanishes. A natural symmetric [alpha tensor](../../../../../alpha-tensor.md) is

$$
\alpha_{ij}^{\mathrm{nat}}=k^2S_h\left\langle\frac{n_in_j}{[\nu\eta k^4+k^2|B|^2\mu^2/m_0]^2}\right\rangle_{\mathbf n},
\qquad \mu=\mathbf n\cdot\widehat{\mathbf B}.
$$

Only its longitudinal coefficient contributes to $\boldsymbol{\mathcal E}=\alpha_{\parallel}\mathbf B$. Introduce $h=|B|/[k\sqrt{m_0\nu\eta}]$ and $A_0=\nu\eta k^4$. Angular integration gives

$$
\alpha_{\parallel}=\frac{k^2S_h}{A_0^2}\int_0^1\frac{\mu^2d\mu}{(1+h^2\mu^2)^2}
=\frac{k^2S_h}{2A_0^2h^3}\left(\arctan h-\frac{h}{1+h^2}\right).
$$

Therefore the [strong-field quenching of an isotropic electromotive force](../../../../../strong-field-quenching-of-an-isotropic-electromotive-force.md) is

$$
\boxed{\alpha_{\parallel}\sim\frac{\pi k^2S_h}{4A_0^2h^3}\propto |B|^{-3},\qquad
|\boldsymbol{\mathcal E}|\propto |B|^{-2},}
$$

provided $S_h\ne0$. If the two helicity contributions cancel exactly, this electromotive force vanishes.

There is a tensor qualification to the printed scaling claim. The natural transverse coefficient instead contains $\tfrac12\int_0^1(1-\mu^2)(1+h^2\mu^2)^{-2}d\mu\sim\pi/(8h)$ and scales as $|B|^{-1}$. The relation $\mathcal E_i=\alpha_{ij}B_j$ by itself leaves transverse components undetermined. One may choose the effective representative $\alpha_{ij}=\alpha_{\parallel}\delta_{ij}$, for which the requested $|B|^{-3}$ scaling holds. It is the observable longitudinal response that is fixed, rather than every component of a unique field-dependent tensor.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 67](../../paper-67-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
