<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $z=\sqrt\epsilon\,\omega\cos\psi$, with $\omega=\sqrt\beta>0$ and $\psi=\phi-\phi_0$. Differentiating twice gives

$$
\frac{z''+kz}{\sqrt\epsilon}
=[\omega''-\omega(\phi')^2+k\omega]\cos\psi
-[2\omega'\phi'+\omega\phi'']\sin\psi.
$$

The coefficients must vanish for arbitrary initial phase $\phi_0$. The sine coefficient gives

$$
(\omega^2\phi')'=0,\qquad \omega^2\phi'=C.
$$

The conventional [Courant-Snyder parameters](../../../../courant-snyder-parameters.md) normalize the phase so that $C=1$; any positive constant $C$ can be absorbed into the scale assigned to $\beta$ and $\epsilon$. Explicitly, $\widetilde\beta=\beta/C$ and $\widetilde\epsilon=C\epsilon$ preserve the orbit while making $\widetilde\beta\phi'=1$. With this convention,

$$
\boxed{\phi'=\frac1\beta,\qquad
\omega''-\frac1{\omega^3}+k(s)\omega=0.}
$$

The second expression is the [Ermakov-Pinney equation](../../../../ermakov-pinney-equation.md) for the beam envelope. It follows by substituting $\phi'=1/\omega^2$ into the cosine coefficient.

**The printed equation omits the factor $\omega$ multiplying $k(s)$.** For a concrete counterexample, take the constant periodic focusing strength $k=1/16$ and the constant envelope $\omega=2$. Then $\phi'=1/4$ and $z=2\sqrt\epsilon\cos(s/4-\phi_0)$ solve $z''+z/16=0$. The correct envelope equation is $0-1/8+(1/16)2=0$, whereas the printed equation gives $-1/8+1/16=-1/16$.

The associated invariant is

$$
\epsilon=\gamma_Tz^2+2\alpha_Tzz'+\beta z'^2,
\qquad \alpha_T=-\beta'/2,\quad
\gamma_T=(1+\alpha_T^2)/\beta.
$$

Thus $\epsilon$ fixes the [phase-space](../../../../phase-space.md) ellipse of a trajectory; a beam's rms [geometric emittance](../../../../geometric-emittance.md) uses the corresponding second-moment convention. Factors of $\pi$ depend on whether emittance means ellipse area or area divided by $\pi$ and do not alter the envelope equation.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the particle physics course of the University of Oxford](../../../split.md)
5. [Particle physics course of the University of Oxford](../../../../particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
