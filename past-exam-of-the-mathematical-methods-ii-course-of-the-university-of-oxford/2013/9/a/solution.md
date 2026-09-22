<h1 id="9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume the stated continuous derivatives on an open [simply connected](../../../../simply-connected-space.md) region. If $N_x-M_y=0$, [Green's theorem](../../../../green-theorem.md) gives zero circulation around every simple closed curve and its enclosed region; a piecewise smooth closed curve can be decomposed into such loops, giving the same conclusion.

Conversely, suppose every closed-curve integral vanishes. Apply [Green's theorem](../../../../green-theorem.md) to an arbitrarily small disk about any interior point $P$. Its integral of $N_x-M_y$ is zero. Divide by the disk area and shrink its radius to zero; continuity makes the average approach $(N_x-M_y)(P)$, so that value must vanish. Thus

$$
\boxed{\oint_C M\,dx+N\,dy=0\text{ for every closed }C\quad\Longleftrightarrow\quad N_x=M_y.}
$$

Simple connectivity is needed for the global sufficiency statement, ensuring that a loop does not enclose a missing portion of the domain. Local necessity already follows from small disks.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [9](../../9.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
