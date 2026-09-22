<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For each fixed $z$, choose the [convex perturbation function](../../../../../../convex-perturbation-function.md)

$$
\boxed{f_z(x,u)=k(x)+h(z+u-x).}
$$

It is jointly convex and has marginal

$$
p_z(u)=\inf_x[k(x)+h(z+u-x)]=F(z+u).
$$

Because $h$ and $k$ are nonnegative and finite everywhere,

$$
0\leq F(w)\leq k(0)+h(w)<\infty
$$

for every $w$. The [inf-convolution](../../../../../../infimal-convolution.md) is convex: for approximate decompositions of $w_1,w_2$, take their convex combination and use convexity of both costs; then let their approximation errors tend to zero. Thus $F$ is a finite [convex function](../../../../../../convex-function.md) on all of $\mathbb R^n$, hence continuous everywhere. In particular $p_z$ is proper and finite near zero, so the qualification in the previous solution applies at every $z$:

$$
\boxed{\inf_x[k(x)+h(z-x)]=\max_y[-f_z^*(0,y)].}
$$

This is [strong duality](../../../../../../strong-duality.md) for a [finite-valued infimal convolution](../../../../../../finite-valued-infimal-convolution.md).

No primal attainment was used. For example $k(x)=e^x$ and $h(x)=0$ meet all the stated assumptions, but $F(z)=0$ is approached only as $x\to-\infty$. This illustrates why a proof based on an assumed minimizing decomposition would be incomplete. The printed functions are real-valued everywhere, not merely extended-real; that distinction supplies continuity and the strong-duality qualification.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
