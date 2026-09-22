<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the energy

$$
J(v)=\frac12a(v,v)-\int_{-1}^1f(x)v(x)dx.
$$

Its first variation in direction $w\in\mathcal H$ is

$$
\delta J(v;w)=a(v,w)-\int_{-1}^1fw\,dx.
$$

Thus its minimizer $u$ satisfies the [weak formulation](../../../../../../weak-formulation.md)

$$
a(u,w)=\int_{-1}^1fw\,dx
\qquad\text{for every }w\in\mathcal H,
$$

which is the weak equation $Lu=f$. Positive definiteness makes $J$ strictly convex, so this stationary point is the unique minimizer; under uniform positivity of $p$, existence follows from the [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
