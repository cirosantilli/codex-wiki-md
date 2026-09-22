<h1 id="10d/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the construction in part (c) for the marked-state phase reflection in each [Grover search algorithm](../../../../../../grover-s-algorithm.md) iteration. Every such reflection costs one query to $U_f$; the identity-oracle circuit, Hadamard gates, and $I_0$ are independent of $f$.

Starting from $|s\rangle$, after $r$ iterations the success probability is

$$
\sin^2((2r+1)\theta),
\qquad
\sin\theta=N^{-1/2},
$$

by the [Grover rotation angle](../../../../../../grover-rotation-angle.md). Choose an integer

$$
r=\left\lfloor\frac{\pi}{4\theta}-\frac12\right\rceil.
$$

Then $(2r+1)\theta$ differs from $\pi/2$ by at most $\theta$, so

$$
\Pr(\text{measure }x_0)
\geq\cos^2\theta
=1-\frac1N.
$$

For every sufficiently large $N$ this is greater than $1/2$, while

$$
r=O(\theta^{-1})=O(\sqrt N).
$$

**Thus measuring the search register determines the faulty input with the required constant success probability using $O(\sqrt N)$ oracle queries.**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [10D](../../10d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
