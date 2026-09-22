<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With a mass source, the [continuity equation](../../../../../../continuity-equation.md) becomes $\rho_t+\partial_i(\rho u_i)=M$. If the conservative momentum equation has no added source, repeating the elimination gives the [mass-injection term in the acoustic analogy](../../../../../../mass-injection-term-in-the-acoustic-analogy.md):

$$
\boxed{(\partial_t^2-c_0^2\Delta)\rho'=\partial_i\partial_jT_{ij}+\partial_tM.}
$$

More generally, injection can carry momentum. If its momentum source is $S_i$, the additional term is $\partial_tM-\partial_iS_i$; prescribing $M$ alone does not determine this dipole contribution. The displayed monopole formula assumes no separately imposed momentum source.

Let $\mathcal M(t)=\int M(\mathbf y,t)\,d^3y$ be the total mass rate. Convolution with the [retarded acoustic Green function](../../../../../../retarded-acoustic-green-function.md), followed by the [acoustic compact-source approximation](../../../../../../acoustic-compact-source-approximation.md), gives the extra [acoustic monopole](../../../../../../acoustic-monopole.md)

$$
\boxed{\rho'_M(\mathbf x,t)\sim\frac{\dot{\mathcal M}(t-r/c_0)}{4\pi c_0^2r}.}
$$

The stress quadrupole from the preceding part remains present. If required, a compact injected momentum rate $\mathcal S_i=\int S_i\,d^3y$ adds the dipole $n_i\dot{\mathcal S}_i/(4\pi c_0^3r)$.

A small pulsating bubble displaces liquid with volume flux $\dot{\mathcal V}(t)$ and acts acoustically like a mass rate $\mathcal M=\rho_0\dot{\mathcal V}$. Spherical symmetry makes this a monopole, with

$$
\boxed{\rho'\sim\frac{\rho_0}{4\pi c_0^2r}\ddot{\mathcal V}(t-r/c_0).}
$$

For volume oscillation $\mathcal V=\mathcal V_0+\Delta\mathcal V\cos\omega t$, the density amplitude is $\rho_0\omega^2|\Delta\mathcal V|/(4\pi c_0^2r)$. **At fixed volume-displacement amplitude, it scales as $\omega^2$.** Holding volume-flux amplitude fixed would instead give an $\omega$ scaling. The bubble must remain small compared with the wavelength, and a frequency-dependent dynamical bubble amplitude is a separate effect.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
