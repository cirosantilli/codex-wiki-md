<h1 id="section-a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The original diagram places hard walls at $0$ and $3L$, and the central plateau on $L<x<2L$ is **exactly at the indicated ground-state [energy](../../../../../energy-split.md)**. This equality determines the middle of the requested sketch. In the [time-independent Schrödinger equation](../../../../../time-independent-schrodinger-equation.md),

$$
\psi''=\frac{2m}{\hbar^2}(V-E)\psi,
$$

the central interval has $V=E$, hence $\psi''=0$. The [ground state](../../../../../ground-state.md) can be chosen real and positive inside the walls by the [nodeless theorem for a one-dimensional ground state](../../../../../nodeless-theorem-for-a-one-dimensional-ground-state.md). Reflection symmetry makes it even about $x=3L/2$, so its linear central segment must be constant.

The hard-wall boundary conditions are $\psi(0)=\psi(3L)=0$. On both outer intervals $V=0<E$, so the positive [wavefunction](../../../../../wave-function-split.md) has negative curvature and is sinusoidal. [Wavefunction matching at a finite potential step](../../../../../wavefunction-matching-at-a-finite-potential-step.md) requires both $\psi$ and $\psi'$ to remain continuous at $L,2L$; the [derivative](../../../../../derivative.md) therefore vanishes where each sinusoidal flank meets the flat middle. A normalized representative is

$$
\boxed{\psi_0(x)=\frac1{\sqrt{2L}}\begin{cases}
\sin\!\left(\dfrac{\pi x}{2L}\right),&0<x<L,\\
1,&L\le x\le2L,\\
\sin\!\left(\dfrac{\pi(3L-x)}{2L}\right),&2L<x<3L,\\
0,&x\le0\ \text{or}\ x\ge3L.
\end{cases}}
$$

Each side contributes $L/2$ and the plateau contributes $L$ to the squared norm before multiplying by $1/(2L)$. The corresponding consistency condition is $E=\pi^2\hbar^2/(8mL^2)$; a numerical [energy](../../../../../energy-split.md) is not required for the sketch.

<a id="section-a/1/image-the-positive-ground-state-wavefunction-has-sinusoidal-flanks-and-a-flat-central-segment-at-v-equals-e"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-1-q1-flat-barrier-state.png)

**[Figure 1](#section-a/1/image-the-positive-ground-state-wavefunction-has-sinusoidal-flanks-and-a-flat-central-segment-at-v-equals-e). The positive ground-state wavefunction has sinusoidal flanks and a flat central segment at V equals E**.

Thus the [ground state at the top of a central rectangular barrier](../../../../../ground-state-at-the-top-of-a-central-rectangular-barrier.md) has **no internal nodes, continuous value and slope, and a flat middle**, rather than an exponential dip through a classically forbidden region. Multiplication by an overall constant phase changes none of these physical features.

## ↑ Ancestors (14)

1. [1](../1.md)
2. [Section A](../../section-a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
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
