<h1 id="40b/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take

$$
\eta=\eta_0\cos(kx-\omega t)
$$

and define the positive normal decay rate

$$
q=\sqrt{k^2-\frac{\omega^2}{c_0^2}}.
$$

The decaying solutions of the acoustic [wave equation](../../../../../../../wave-equation-split.md) that satisfy the kinematic conditions are

$$
\phi_+=-\frac{\omega\eta_0}{q}e^{-qy}\sin(kx-\omega t)
\quad(y>0),
$$



$$
\phi_-=\frac{\omega\eta_0}{q}e^{qy}\sin(kx-\omega t)
\quad(y<0).
$$

Their pressures at the membrane are

$$
p'_+=-\frac{\rho_0\omega^2\eta_0}{q}\cos(kx-\omega t),
\qquad
p'_-=\frac{\rho_0\omega^2\eta_0}{q}\cos(kx-\omega t).
$$

Substitution into the dynamic boundary condition gives

$$
-m\omega^2\eta_0=-Tk^2\eta_0+\frac{2\rho_0\omega^2}{q}\eta_0,
$$

and hence the [acoustic wave on a tensioned massive membrane](../../../../../../../acoustic-wave-on-a-tensioned-massive-membrane.md) dispersion relation

$$
\boxed{
\left(m+\frac{2\rho_0}{\sqrt{k^2-\omega^2/c_0^2}}\right)\omega^2
=Tk^2.
}
$$

Writing the phase speed as $c=\omega/k$, the positive added-inertia term gives

$$
Tk^2>m\omega^2,
\qquad
\boxed{c<\sqrt{T/m}.}
$$

Physically, each [evanescent acoustic surface wave](../../../../../../../evanescent-acoustic-surface-wave.md) accelerates a layer of fluid on both sides of the membrane, so the inertia per unit area exceeds $m$. Moreover,

$$
q=k\sqrt{1-c^2/c_0^2},
$$

and the [added mass of an evanescent fluid layer](../../../../../../../added-mass-of-an-evanescent-fluid-layer.md) $2\rho_0/q$ diverges as $k\to0$. In that limit $c\ll c_0$, so $q\sim k$ and

$$
\boxed{c^2\sim\frac{Tk}{2\rho_0},
\qquad c(k)\to0.}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [40B](../../../40b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
