<h1 id="section-c/c11/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Ehrenfest theorem](../../../../../../ehrenfest-theorem.md) relates the dynamics of quantum [expectation values](../../../../../../expectation-value.md) to operator [commutators](../../../../../../commutator.md). For a normalized state obeying $i\hbar|\dot\psi\rangle=\widehat H|\psi\rangle$ and a possibly time-dependent [observable](../../../../../../observable.md) $\widehat A$, differentiate $\langle A\rangle=\langle\psi|\widehat A|\psi\rangle$. Using the adjoint [Schrödinger equation](../../../../../../schrodinger-equation.md) for the bra gives

$$
\begin{aligned}
\frac d{dt}\langle A\rangle
&=\frac i\hbar\langle HA\rangle-\frac i\hbar\langle AH\rangle
+\left\langle\frac{\partial A}{\partial t}\right\rangle\\
&=\frac1{i\hbar}\langle[A,H]\rangle
+\left\langle\frac{\partial A}{\partial t}\right\rangle.
\end{aligned}
$$

Thus

$$
\boxed{\frac d{dt}\langle A\rangle=
\frac1{i\hbar}\langle[A,H]\rangle+\langle\partial_t A\rangle.}
$$

The identity assumes a common domain on which the required products and [derivatives](../../../../../../derivative.md) are defined.

For $H=p^2/(2m)+V(x)$, the [canonical commutation relation](../../../../../../canonical-commutation-relation.md) gives $[x,H]=i\hbar p/m$ and $[p,H]=-i\hbar V'(x)$. Therefore

$$
\boxed{\frac d{dt}\langle x\rangle=\frac{\langle p\rangle}{m},\qquad
\frac d{dt}\langle p\rangle=-\langle V'(x)\rangle.}
$$

These resemble [Hamilton's equations](../../../../../../hamilton-s-equations.md) and [Newton's second law](../../../../../../newton-s-second-law.md), but generally $\langle V'(x)\rangle\ne V'(\langle x\rangle)$. If the state is localized about $\overline x=\langle x\rangle$, a local expansion gives

$$
\langle V'(x)\rangle=V'(\overline x)+\frac12V^{(3)}(\overline x)
\langle(x-\overline x)^2\rangle+\cdots.
$$

The classical trajectory equation for the mean is accurate when the force changes little across the [wave packet](../../../../../../wave-packet.md). For a quadratic [harmonic potential](../../../../../../harmonic-potential.md), $V'$ is linear and this closure is exact for every state with the relevant finite moments: $m\,d^2\langle x\rangle/dt^2=-m\omega^2\langle x\rangle$. This exact classical evolution of the centroid does not eliminate its quantum [position uncertainty](../../../../../../position-uncertainty.md) or make every state a point particle.

The [correspondence principle](../../../../../../correspondence-principle.md) is broader: quantum predictions recover classical ones in an appropriate limit, such as large action compared with $\hbar$ and observations that cannot resolve individual quantum levels. It is not the assertion that every large [quantum number](../../../../../../quantum-number.md) automatically makes every possible state classical. Delocalized superpositions and interference can remain significant unless the physical preparation and measurement justify a classical description.

A spectral example is useful. For a [quantum harmonic oscillator](../../../../../../quantum-harmonic-oscillator-split.md), neighboring levels differ by $\hbar\omega$, giving transition [frequency](../../../../../../frequency.md) $\omega/(2\pi)$, equal to its classical oscillation [frequency](../../../../../../frequency.md). A [coherent state](../../../../../../coherent-state.md) makes the connection more concrete: its mean [position](../../../../../../position.md) and [momentum](../../../../../../momentum-split.md) oscillate classically while the finite-width Gaussian profile retains its quantum uncertainty. For hydrogenic Bohr levels $E_n=-A/n^2$, transitions between nearby large $n$ have $\Delta E/\hbar\simeq2A/(\hbar n^3)$, which equals the classical circular orbital angular [frequency](../../../../../../frequency.md) in that model. **Ehrenfest's theorem supplies an exact expectation-value bridge; a classical trajectory follows only when the force can also be evaluated at the mean [position](../../../../../../position.md).**

## ↑ Ancestors (15)

1. [B](../b.md)
2. [C11](../../c11.md)
3. [Section C](../../../section-c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
