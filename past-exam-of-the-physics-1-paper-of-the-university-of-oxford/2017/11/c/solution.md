<h1 id="11/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $h=J/m=bv_0$ be the [specific angular momentum](../../../../specific-angular-momentum.md), and measure the orbital angle $\vartheta$ from [periapsis](../../../../periapsis.md). Set $w=1/r$. From $\dot\vartheta=h/r^2$, differentiating gives $\dot r=-h\,dw/d\vartheta$. The radial [equation of motion](../../../../equation-of-motion.md) $\ddot r-r\dot\vartheta^2=-\mu_J/r^2$ becomes the [Binet equation](../../../../binet-equation.md)

$$
\frac{d^2w}{d\vartheta^2}+w=\frac{\mu_J}{h^2}.
$$

Its solution symmetric about [periapsis](../../../../periapsis.md) is

$$
w=\frac{\mu_J}{h^2}(1+e\cos\vartheta),\qquad
e=\sqrt{1+\frac{v_0^2h^2}{\mu_J^2}}
=\sqrt{1+\frac{b^2v_0^4}{\mu_J^2}}.
$$

For example, the expression for the [orbital eccentricity](../../../../orbital-eccentricity.md) follows by substituting $w$ and $\dot r=-hw'$ into the [energy](../../../../energy-split.md) equation: $E/m=\mu_J^2(e^2-1)/(2h^2)=v_0^2/2$. Since $e>1$, this is a [hyperbolic Kepler orbit](../../../../hyperbolic-kepler-orbit.md).

The outgoing asymptote occurs at $\vartheta_\infty$ with $\cos\vartheta_\infty=-1/e$, where $\pi/2<\vartheta_\infty<\pi$. The incoming [velocity](../../../../velocity.md) points inward along the incoming radial asymptote, whereas the outgoing [velocity](../../../../velocity.md) points outward. Therefore the change in [velocity](../../../../velocity.md) direction is $\phi=2\vartheta_\infty-\pi$, not $2\vartheta_\infty$. It follows that

$$
\sin\frac\phi2=\frac1e,\qquad
\boxed{\cot\frac\phi2=\sqrt{e^2-1}=\frac{bv_0^2}{GM_J}.}
$$

For $b>0$, this gives $0<\phi<\pi$: a large [impact parameter](../../../../impact-parameter.md) produces a small deflection, and the ideal point-mass limit $b\to0^+$ approaches a reversal.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [11](../../11.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the physics 1 paper of the University of Oxford](../../../split.md)
5. [Physics 1 paper of the University of Oxford](../../../../physics-1-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
