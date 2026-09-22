<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The triangular support can be written $0\le x\le\pi/2$, $\pi/2-x\le y\le\pi/2$. The density is nonnegative there, and the [normalization of a probability distribution](../../../normalization-of-a-probability-distribution.md) requires

$$
1=A\int_0^{\pi/2}\sin x(1-\cos x)\,dx=\frac A2.
$$

Hence $\boxed{A=2}$. Multiplying the [joint probability density](../../../joint-probability-density.md) by the required function cancels $\sin x$ on the interior. Its [expectation](../../../expected-value-split.md) is

$$
\boxed{\mathbb E\left[\frac1{\sin X}\right]=2\int_0^{\pi/2}(1-\cos x)\,dx=\pi-2.}
$$

The singularity at $x=0$ lies at a support vertex of zero probability; the displayed [integral](../../../integral-split.md) establishes integrability. Assigning any value to the random function at that single vertex does not change the [expectation](../../../expected-value-split.md).

## ↑ Ancestors (11)

1. [6](../6.md)
2. [2022](../../2022-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
