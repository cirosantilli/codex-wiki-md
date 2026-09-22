<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use signature $(-,+,+,+)$, $\{\gamma^\mu,\gamma^\nu\}=2\eta^{\mu\nu}$, and unit-weight antisymmetrized gamma products. The massless [Rarita-Schwinger field](../../../../../rarita-schwinger-field.md) has the gauge freedom

$$
\psi_\mu\longmapsto\psi_\mu+\partial_\mu\epsilon,
$$

since the antisymmetric $\gamma^{\mu\nu\rho}$ annihilates $\partial_\nu\partial_\rho\epsilon$. This gauge freedom is essential to remove the lower-spin components of the vector-spinor.

Put $\chi=\gamma^\mu\psi_\mu$. Contracting the field equation with $\gamma_\mu$ and using $\gamma_\mu\gamma^{\mu\nu\rho}=2\gamma^{\nu\rho}$ gives

$$
\not\partial\chi-\partial^\mu\psi_\mu=0.
$$

Expanding the original three-gamma product then reduces its equation to

$$
\not\partial\psi^\mu-\partial^\mu\chi=0.
$$

A gauge transformation changes $\chi$ by $\not\partial\epsilon$. Locally solve $\not\partial\epsilon=-\chi$ to impose gamma-trace gauge. The two equations become

$$
\boxed{\gamma\cdot\psi=0,\qquad\partial\cdot\psi=0,\qquad\not\partial\psi_\mu=0.}
$$

Applying $\not\partial$ again gives $\Box\psi_\mu=0$. Nonzero propagating Fourier modes therefore have $p^2=0$: **the physical modes are massless**.

For the [massless Rarita-Schwinger polarization count](../../../../../massless-rarita-schwinger-polarization-count.md), choose a nonzero future null momentum $p^\mu=(\omega,0,0,\omega)$. The remaining gauge parameters satisfy $\not p\epsilon=0$. Transversality gives $\psi_0+\psi_3=0$, and this residual gauge removes $\psi_0$, hence also $\psi_3$, because $\psi_0$ itself satisfies $\not p\psi_0=0$. Only $\psi_1,\psi_2$ remain, with

$$
\not p\psi_1=\not p\psi_2=0,\qquad
\gamma^1\psi_1+\gamma^2\psi_2=0,\qquad
\psi_2=\gamma^1\gamma^2\psi_1.
$$

The kernel of $\not p$ on four-component spinors has complex dimension two, so there are exactly two independent polarization amplitudes.

To identify their [helicities](../../../../../helicity.md), the spinor rotation generator about the third axis in this convention is $S_3=-i\gamma^1\gamma^2/2$. Its two eigenvalues on that kernel are $h_s=\pm1/2$. If $\psi_1$ is such an eigenvector, then $\psi_2=2ih_s\psi_1$. Its transverse vector polarization is consequently $(1,+i)$ for $h_s=+1/2$ or $(1,-i)$ for $h_s=-1/2$. These carry vector helicity $+1$ or $-1$, respectively. Adding the vector and spinor angular momenta leaves

$$
\boxed{h=+\frac32,\quad h=-\frac32,\qquad\text{two physical helicity states}.}
$$

The unwanted opposite-sign vector-spinor combinations, which would have helicity $\pm1/2$, violate the gamma-trace constraint. For the [gravitino](../../../../../gravitino.md) of simple [supergravity](../../../../../supergravity.md), its [Majorana spinor](../../../../../majorana-spinor.md) reality condition identifies the negative-frequency antiparticle modes, giving two propagating degrees of freedom. If one instead chooses a complex Dirac vector-spinor, its independent antiparticle sector doubles the particle-plus-antiparticle count; the equation alone does not impose a Majorana condition.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 60](../../paper-60-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
