<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the off-diagonal moves, the [Metropolis–Hastings acceptance probability](../../../../../../metropolis-hastings-acceptance-probability.md) gives

$$
\pi(x)q(y\mid x)\alpha(x,y)
=\min\{\pi(x)q(y\mid x),\pi(y)q(x\mid y)\}.
$$

This expression is unchanged by interchanging $x$ and $y$. The rejected-move measure $\pi(dx)r(x)\delta_x(dy)$ is supported on the diagonal and is also symmetric. Therefore the whole transition measure satisfies

$$
\boxed{\pi(dx)K(x,dy)=\pi(dy)K(y,dx),}
$$

which proves [detailed balance](../../../../../../detailed-balance.md), including the atom that an off-diagonal density alone would omit. Consequently the [Metropolis–Hastings algorithm](../../../../../../metropolis-hastings-algorithm.md) kernel preserves the normalized target measure.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
