<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

After transients have decayed, seek the driven response $\mathbf x=\mathbf a\sin\omega t$. At the given $\omega^2=k/m$, substitution gives

$$
\begin{pmatrix}2&-2\\-2&0\end{pmatrix}\mathbf a=\begin{pmatrix}F\\0\end{pmatrix}.
$$

The second row forces $a_1=0$, and the first gives $a_2=-F/2$. Hence, in the negligible-damping steady-response limit,

$$
\boxed{x_1(t)=0,\qquad x_2(t)=-\frac F2\sin\omega t.}
$$

The support forcing on the first mass is balanced by the inter-mass spring force while the second mass moves in antiphase. This is a [support-driven unequal-mass spring antiresonance](../../../../support-driven-unequal-mass-spring-antiresonance.md), not a resonance: the drive frequency lies between the two normal-mode frequencies. A genuinely finite damping coefficient produces small phase shifts and a small nonzero first-mass response; the displayed formula uses the source's instruction to neglect damping except for removal of transients.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [9](../../9.md)
3. [2013 resit](../../../2013-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
