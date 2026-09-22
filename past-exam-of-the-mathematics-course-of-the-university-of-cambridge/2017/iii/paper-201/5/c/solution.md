<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First suppose $|x+z|\leq r$ for some lattice point $-z$. If $|x+z|=r$, the desired hit is already at time zero. If $|x+z|<r$, finite exit from that bounded [open ball](../../../../../../open-ball.md) and continuity give the required [sphere](../../../../../../sphere.md) hit [almost surely](../../../../../../almost-sure-convergence.md).

It remains to consider $|x+z|>r$ for every $z\in\mathbb Z^3$. At each integer time $n$, choose a nearest lattice point $-z_n$ to $B_n$ by rounding its three coordinates, with a fixed rule at ties. Then $|B_n+z_n|\leq\sqrt3/2$. Put $\delta=\min(r/2,1/4)>0$. Conditional on the past, $B_{n+1}-B_n$ is a standard three-dimensional [Gaussian vector](../../../../../../gaussian-random-vector.md). Its [probability density function](../../../../../../probability-density-function.md) is bounded below on the [open ball](../../../../../../open-ball.md) of radius $\delta$ centered at $-(B_n+z_n)$ by

$$
(2\pi)^{-3/2}\exp\!\left[-\tfrac12(\sqrt3/2+\delta)^2\right].
$$

Multiplying by the volume of that [open ball](../../../../../../open-ball.md) gives a constant $\varepsilon>0$, independent of $n$ and the past, such that

$$
\mathbb P\bigl(|B_{n+1}+z_n|<\delta\mid\mathcal F_n\bigr)\geq\varepsilon.
$$

The probability of avoiding all lattice-centered radius-$r$ [open balls](../../../../../../open-ball.md) at the first $N$ positive integer times is therefore at most $(1-\varepsilon)^N$, by iterated [conditional expectation](../../../../../../conditional-expectation.md). Eventually the path enters one such [open ball](../../../../../../open-ball.md) [almost surely](../../../../../../almost-sure-convergence.md). Since the initial point was outside that particular [open ball](../../../../../../open-ball.md), continuity forces an earlier crossing of its [sphere](../../../../../../sphere.md). This proves [Brownian hitting of lattice spheres](../../../../../../brownian-hitting-of-lattice-spheres.md):

$$
\boxed{\mathbb P_x\!\left(\exists t\geq0,\ z\in\mathbb Z^3:\ |B_t+z|=r\right)=1.}
$$

A uniform chance of hitting some member of the periodic family replaces recurrence to any one prescribed [sphere](../../../../../../sphere.md); there is no contradiction with (b).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
