<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $\mathbf r=\mathbf r_2-\mathbf r_1$ and $\mathbf v=\dot{\mathbf r}$. Relative to the [centre of mass](../../../../../center-of-mass.md), the two positions are $\mathbf r_1=-(M_2/M)\mathbf r$ and $\mathbf r_2=(M_1/M)\mathbf r$. Their velocities have the same mass factors. Adding their kinetic energies and [angular momenta](../../../../../angular-momentum.md) gives, with [reduced mass](../../../../../reduced-mass.md) $\mu=M_1M_2/M$,

$$
\boxed{E=\frac12\mu v^2-\frac{GM_1M_2}{r}},\qquad
\boxed{\mathbf J=\mu\mathbf r\times\mathbf v=\mu\mathbf h}.
$$

These are the internal orbital quantities, excluding any uniform centre-of-mass motion. [Newton's law of universal gravitation](../../../../../newton-s-law-of-universal-gravitation.md) gives

$$
\ddot{\mathbf r}_1=\frac{GM_2}{r^3}\mathbf r,\qquad
\ddot{\mathbf r}_2=-\frac{GM_1}{r^3}\mathbf r,\qquad
\ddot{\mathbf r}=-\frac{GM}{r^3}\mathbf r.
$$

For constant masses, differentiating $E$ makes the gravitational work cancel the derivative of the [potential energy](../../../../../potential-energy.md), so $\dot E=0$. Also $\dot{\mathbf h}=\mathbf r\times\ddot{\mathbf r}=0$, since the force is central; hence [conservation of angular momentum](../../../../../conservation-of-angular-momentum.md) gives $\dot{\mathbf J}=0$.

The [eccentricity vector](../../../../../eccentricity-vector.md), the normalized attractive [Laplace-Runge-Lenz vector](../../../../../laplace-runge-lenz-vector.md), is

$$
GM\mathbf e=\mathbf v\times\mathbf h-GM\widehat{\mathbf r}.
$$

Using $\dot{\widehat{\mathbf r}}=\mathbf v/r-\mathbf r(\mathbf r\mathbin\cdot\mathbf v)/r^3$ and

$$
-\frac{GM}{r^3}\mathbf r\times\mathbf h
=GM\left(\frac{\mathbf v}{r}-\frac{\mathbf r(\mathbf r\mathbin\cdot\mathbf v)}{r^3}\right)
$$

shows that its derivative also vanishes. Adding a relative perturbing acceleration $\mathbf f$ changes these cancellations only by the perturbing terms. The [perturbed Kepler-orbit conservation laws](../../../../../perturbed-kepler-orbit-conservation-laws.md) are therefore

$$
\boxed{\dot E=\mu\mathbf v\mathbin\cdot\mathbf f},\qquad
\boxed{\dot{\mathbf h}=\mathbf r\times\mathbf f},\qquad
\boxed{GM\dot{\mathbf e}=\mathbf f\times\mathbf h+\mathbf v\times(\mathbf r\times\mathbf f)}.
$$

For the distant [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md), expand each source term about the binary's [centre of mass](../../../../../center-of-mass.md):

$$
\frac1{|\mathbf x-\mathbf r_i|}
=\frac1x+\frac{\widehat{\mathbf x}\mathbin\cdot\mathbf r_i}{x^2}
+\frac{3(\widehat{\mathbf x}\mathbin\cdot\mathbf r_i)^2-r_i^2}{2x^3}
+O\left(\frac{a^3}{x^4}\right).
$$

The dipole vanishes because $\sum_iM_i\mathbf r_i=0$. With $\mathbf a=\mathbf r$, the quadratic mass moment is $\sum_iM_i\mathbf r_i\mathbf r_i=\mu\mathbf a\mathbf a$, so the [quadrupole potential of a circular binary](../../../../../quadrupole-potential-of-a-circular-binary.md) is

$$
\boxed{\phi(\mathbf x)=-\frac{GM}{x}-\frac{G\mu a^2}{2x^3}(3\cos^2\theta-1)+O\left(\frac{GMa^3}{x^4}\right)}.
$$

On the inner binary's fast timescale, the distant companion's position is approximately fixed. Averaging over the inner [circular orbit](../../../../../circular-orbit.md) in the common plane gives $\langle\cos^2\theta\rangle=1/2$ and hence

$$
\overline\phi(x)=-\frac{GM}{x}-\frac{G\mu a^2}{4x^3}.
$$

This averaged [potential function](../../../../../potential-function.md) is independent of both time and azimuth. Consequently the companion's energy and axial [angular momentum](../../../../../angular-momentum.md) are conserved in the averaged problem. The exact motion has small fast variations; the statement is a secular approximation for a hierarchical system away from an orbital resonance.

For a circular outer orbit, force balance gives

$$
x\Omega_3^2=\frac{d\overline\phi}{dx}
=\frac{GM}{x^2}+\frac{3G\mu a^2}{4x^4},
$$

so the [circumbinary orbital-period correction](../../../../../circumbinary-orbital-period-correction.md) is

$$
\boxed{P_3=2\pi\sqrt{\frac{x^3}{GM}}
\left(1+\frac{3\mu a^2}{4Mx^2}\right)^{-1/2}}
=2\pi\sqrt{\frac{x^3}{GM}}\left[1-\frac{3\mu a^2}{8Mx^2}+O\left(\frac{a^4}{x^4}\right)\right].
$$

[Conservative binary mass transfer](../../../../../conservative-binary-mass-transfer.md) leaves $M$ unchanged, so it does not change the leading monopole force. It changes $\mu$ and $a$, and therefore the quadrupole correction. If the inner orbital [angular momentum](../../../../../angular-momentum.md) is conserved, $J_{\rm in}=\mu\sqrt{GMa}$ gives $a\propto\mu^{-2}$ and $Q=\mu a^2\propto\mu^{-3}$. The correction is thus largest as the binary becomes strongly unequal in mass and widens, within the hierarchy $a\ll x$.

One must also allow the outer radius to respond. For slow axisymmetric evolution its [specific angular momentum](../../../../../specific-angular-momentum.md) $h_3$ remains constant, while its energy need not: the averaged potential now depends on time. A nearly circular outer orbit has $h_3^2=GMx+3GQ/(4x)$ and $P_3=2\pi x^2/h_3$. At fixed $M,h_3$, differentiation gives

$$
\frac{dP_3}{P_3}=-\frac{6\,dQ}{4Mx^2-3Q}
\simeq-\frac{3\,dQ}{2Mx^2}.
$$

Thus mass exchange inside the binary can produce a small measurable outer-period change even without total mass loss. Nonconservative mass loss additionally changes the leading monopole term.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 322](../../paper-322-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
