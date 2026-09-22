<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Apply the [shearing-wave ansatz](../../../../../../shearing-wave-ansatz.md) to each disturbance. Acting on its phase gives

$$
D_0e^{i[k_x(t)x+k_y(t)y]}=i[(\dot k_x-Sk_y)x+\dot k_y y]e^{i\mathbf k\cdot\mathbf x}.
$$

Thus a spatially uniform amplitude system exists when

$$
\boxed{\dot{\mathbf k}=Sk_y\mathbf e_x,\qquad k_y=\text{constant},\qquad k_x(t)=k_x(0)+Sk_yt.}
$$

For a nonzero horizontal [wavenumber](../../../../../../wavenumber.md) $k=|\mathbf k|$, the [razor-thin disk Poisson kernel](../../../../../../razor-thin-disk-poisson-kernel.md) follows from $(\partial_z^2-k^2)\widetilde\Phi_d'=4\pi G\widetilde\Sigma'\delta(z)$. The potential decays above and below the sheet as $\widetilde\Phi_{d,m}'e^{-k|z|}$. Integrating across the midplane gives the jump $-2k\widetilde\Phi_{d,m}'=4\pi G\widetilde\Sigma'$, hence

$$
\widetilde\Phi_{d,m}'=-\frac{2\pi G}{k}\widetilde\Sigma'.
$$

Substitute this potential and the phase evolution into the linearized equations. The [barotropic shearing-wave gravitational amplitude system](../../../../../../barotropic-shearing-wave-gravitational-amplitude-system.md) is

$$
\boxed{\begin{aligned}\dot{\widetilde\Sigma}'&=-i\Sigma_0(k_x\widetilde v_x+k_y\widetilde v_y),\\\dot{\widetilde v}_x-2\Omega\widetilde v_y&=-ik_x\left(c_s^2-\frac{2\pi G\Sigma_0}{k}\right)\frac{\widetilde\Sigma'}{\Sigma_0},\\\dot{\widetilde v}_y+(2\Omega-S)\widetilde v_x&=-ik_y\left(c_s^2-\frac{2\pi G\Sigma_0}{k}\right)\frac{\widetilde\Sigma'}{\Sigma_0}.\end{aligned}}
$$

The self-gravity sign is attractive and opposes the [pressure](../../../../../../pressure.md) response. The uniform $k=0$ [mass density](../../../../../../density.md) shift requires its own gravitational reference and is not obtained by dividing by $k$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
