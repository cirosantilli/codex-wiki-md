<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Define the perturbation energy per unit mass by $E=\langle v^2/2+B^2/(2\mu_0\rho)\rangle$. Dot the momentum equation with $\mathbf v$ and the induction equation with $\mathbf B/(\mu_0\rho)$, then take [volume averages](../../../../../../volume-average.md). The [Coriolis force](../../../../../../coriolis-force.md) does no work. Pressure work and nonlinear advection are divergences and integrate to zero, as does the background $x\partial_y$ transport. The two magnetic exchange terms add to

$$
\frac1{\mu_0\rho}\left\langle\mathbf v\cdot(\mathbf B\cdot\nabla\mathbf B)
+\mathbf B\cdot(\mathbf B\cdot\nabla\mathbf v)\right\rangle
=\frac1{\mu_0\rho}\langle\nabla\cdot[\mathbf B(\mathbf v\cdot\mathbf B)]\rangle=0.
$$

The velocity shear term supplies $2A\langle v_xv_y\rangle$, while magnetic shear supplies $-2A\langle B_xB_y\rangle/(\mu_0\rho)$. Integration by parts gives the viscous and resistive losses as $-\nu\langle|\nabla\mathbf v|^2\rangle$ and $-\eta\langle|\nabla\mathbf B|^2\rangle/(\mu_0\rho)$. For a solenoidal field $\mathbf F$, another integration by parts shows

$$
\langle|\nabla\mathbf F|^2\rangle=\langle|\nabla\times\mathbf F|^2\rangle.
$$

All boundary terms cancel by the shearing-periodic identities. The resulting balance is

$$
\boxed{\frac{dE}{dt}=2A\left\langle v_xv_y-\frac{B_xB_y}{\mu_0\rho}\right\rangle
-\nu\langle|\nabla\times\mathbf v|^2\rangle
-\frac\eta{\mu_0\rho}\langle|\nabla\times\mathbf B|^2\rangle}.
$$

The source is work extracted from maintained differential rotation by [Reynolds stress](../../../../../../reynolds-stress.md) and the magnetic part of the [Maxwell stress tensor](../../../../../../maxwell-stress-tensor.md); internal magnetic/kinetic exchange has canceled.

For the decay bound, the elementary inequality $2|ab|\le a^2+b^2$ gives

$$
2A\left\langle v_xv_y-\frac{B_xB_y}{\mu_0\rho}\right\rangle
\le |A|\left\langle v^2+\frac{B^2}{\mu_0\rho}\right\rangle=2|A|E.
$$

A uniform [spectral gap of a shearing-periodic box](../../../../../../spectral-gap-of-a-shearing-periodic-box.md) is needed; ordinary radial periodicity cannot simply be assumed. At each time the compatible [Fourier modes](../../../../../../fourier-mode.md) are

$$
\exp\!\left[2\pi i\left(\frac{nx}{L_x}+\frac{m(y+2Axt)}{L_y}+\frac{pz}{L_z}\right)\right],
\qquad(n,m,p)\in\mathbb Z^3.
$$

They are orthogonal over the box. Their wavevectors are

$$
\mathbf k=\left(\frac{2\pi n}{L_x}+2At\frac{2\pi m}{L_y},\frac{2\pi m}{L_y},\frac{2\pi p}{L_z}\right).
$$

For every nonconstant mode, $|\mathbf k|\ge2\pi/L$, where $L=\max(L_x,L_y,L_z)$: if $m$ or $p$ is nonzero, its corresponding unsheared component supplies the bound; otherwise $n\ne0$ and the radial component does. Zero mean excludes precisely the constant mode. The [Parseval identity](../../../../../../parseval-identity.md) therefore proves the time-uniform [Poincaré inequality](../../../../../../poincare-inequality.md)

$$
\langle|\nabla f|^2\rangle\ge\frac{4\pi^2}{L^2}\langle|f|^2\rangle.
$$

Apply it componentwise to $\mathbf v$ and $\mathbf B$. With $\nu=\eta$, the [energy decay criterion for a viscous-resistive shearing box](../../../../../../energy-decay-criterion-for-a-viscous-resistive-shearing-box.md) becomes

$$
\frac{dE}{dt}\le2\left(|A|-\frac{4\pi^2\eta}{L^2}\right)E
=-\frac{2\eta}{L^2}(4\pi^2-\mathrm{Rm})E.
$$

Hence

$$
\boxed{\mathrm{Rm}<4\pi^2\ \Longrightarrow\
E(t)\le E(0)\exp\!\left[-\frac{2\eta}{L^2}(4\pi^2-\mathrm{Rm})t\right]\longrightarrow0}.
$$

This excludes sustained finite-amplitude turbulence as well as infinitesimal growth. It is a sufficient stability condition, not a claim that every box above the threshold must become turbulent. The zero-mean restrictions matter: an imposed uniform magnetic field or bulk epicycle is not controlled by this spatial spectral-gap inequality.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
