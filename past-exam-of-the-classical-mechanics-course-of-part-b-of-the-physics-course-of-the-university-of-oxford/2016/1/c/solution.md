<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Treat the marble as a frictionless point particle; no size, rolling constraint or [friction](../../../../friction.md) law is supplied. Neglect its vertical [kinetic energy](../../../../kinetic-energy.md) as requested, but retain the gravitational [potential energy](../../../../potential-energy.md) $mgz=m\omega^2(x_1^2+y_1^2)/2$.

For completeness keep the general constant cup [rotation](../../../../rotation-mathematics.md) rate $\nu=\Omega+\phi$. In cup components the center's [velocity](../../../../velocity.md) is $\mathbf w=R\Omega(\sin\phi t,\cos\phi t)$. With $\mathsf J(x,y)=(-y,x)$, the horizontal [velocity](../../../../velocity.md) norm is $|\dot{\mathbf q}+\nu\mathsf J\mathbf q+\mathbf w|$. Thus

$$
\boxed{L=\frac m2\left[(\dot x_1-\nu y_1+R\Omega\sin\phi t)^2+
(\dot y_1+\nu x_1+R\Omega\cos\phi t)^2\right]
-\frac{m\omega^2}{2}(x_1^2+y_1^2).}
$$

In the nonrotating translating case $\phi=-\Omega$, this reduces to

$$
\boxed{L=\frac m2\left[(\dot x_1-R\Omega\sin\Omega t)^2+
(\dot y_1+R\Omega\cos\Omega t)^2\right]-\frac{m\omega^2}{2}(x_1^2+y_1^2).}
$$

The time-only constant $mR^2\Omega^2/2$ may be dropped. Integrating the cross-velocity term by parts gives an equivalent [Lagrangian](../../../../lagrangian.md)

$$
L'=\frac m2(\dot x_1^2+\dot y_1^2)-\frac{m\omega^2}{2}(x_1^2+y_1^2)
+mR\Omega^2(x_1\cos\Omega t+y_1\sin\Omega t).
$$

It differs by a [total derivative](../../../../total-derivative.md) and a time-only term, so gives the same [trajectories](../../../../trajectory.md) but different expressions for the [canonical momenta](../../../../canonical-momentum.md). The small-vertical-velocity approximation is typically consistent at small surface slope $\omega^2|\mathbf q|/g$; it need not remain valid during unlimited resonant growth.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the classical mechanics course of Part B of the physics course of the University of Oxford](../../../split.md)
5. [Classical mechanics course of Part B of the physics course of the University of Oxford](../../../../classical-mechanics-course-of-part-b-of-the-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../d/solution.md)
