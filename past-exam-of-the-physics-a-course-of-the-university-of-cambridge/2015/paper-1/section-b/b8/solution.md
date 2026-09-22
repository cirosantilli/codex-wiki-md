<h1 id="section-b/b8/solution">Solution</h1>

↑ **Parent:** [B8](../b8.md)

**Factorization.** Put $\alpha=\sqrt{m\omega/(2\hbar)}$ and use the [canonical commutation relation](../../../../../canonical-commutation-relation.md) $[x,p]=i\hbar$:

$$
a^\dagger a=\alpha^2\left(x-\frac{ip}{m\omega}\right)
\left(x+\frac{ip}{m\omega}\right)
=\frac{m\omega x^2}{2\hbar}+\frac{p^2}{2m\hbar\omega}-\frac12.
$$

It follows that

$$
\boxed{H=\hbar\omega(a^\dagger a+\tfrac12)}.
$$

The $-1/2$ arises from [quantum operator ordering](../../../../../quantum-operator-ordering.md); treating $x$ and $p$ as commuting would lose the [zero-point energy](../../../../../zero-point-energy.md).

**[commutators](../../../../../commutator.md).** Direct use of $[x,p]=i\hbar$ gives $[a,a^\dagger]=1$. The product rule for [commutators](../../../../../commutator.md) then yields $[a^\dagger a,a]=-a$ and $[a^\dagger a,a^\dagger]=a^\dagger$, hence

$$
\boxed{[a,a^\dagger]=1,\quad[H,a]=-\hbar\omega a,\quad
[H,a^\dagger]=\hbar\omega a^\dagger}.
$$

**Raising the [energy](../../../../../energy-split.md).** If $H|\phi\rangle=E|\phi\rangle$, then

$$
Ha^\dagger|\phi\rangle
=(a^\dagger H+[H,a^\dagger])|\phi\rangle
=(E+\hbar\omega)a^\dagger|\phi\rangle.
$$

Thus the [creation operator](../../../../../creation-operator.md) produces an [energy eigenstate](../../../../../energy-eigenstate.md) with **[energy](../../../../../energy-split.md) $E+\hbar\omega$**. It is nonzero: for a normalized physical oscillator [eigenstate](../../../../../eigenstate.md), $\|a^\dagger\phi\|^2=\langle aa^\dagger\rangle=E/(\hbar\omega)+1/2>0$. Normalize by this norm if a normalized state is wanted.

**Lowest [wavefunctions](../../../../../wave-function-split.md) and [orthogonality](../../../../../orthogonal-vectors.md).** In the [position representation in quantum mechanics](../../../../../position-representation-in-quantum-mechanics.md),

$$
a=\sqrt{\frac{m\omega}{2\hbar}}\left(x+\frac{\hbar}{m\omega}\frac{d}{dx}\right).
$$

The annihilation condition therefore gives $\psi_0'=-(m\omega/\hbar)x\psi_0$. Applying $a^\dagger$ to its solution gives

$$
\boxed{\psi_0\propto e^{-m\omega x^2/(2\hbar)},\qquad
\psi_1\propto x e^{-m\omega x^2/(2\hbar)}}.
$$

Their [inner product](../../../../../inner-product-split.md) is proportional to $\int_{-\infty}^\infty x e^{-m\omega x^2/\hbar}\,dx=0$, since the integrand is odd. These are the even and odd lowest [wavefunctions](../../../../../wave-function-split.md) shown in A2, with [energies](../../../../../energy-split.md) $\hbar\omega/2$ and $3\hbar\omega/2$.

## ↑ Ancestors (14)

1. [B8](../b8.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
