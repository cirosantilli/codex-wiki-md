<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For clarity, each $\rho_\beta(\alpha)$ is an ordered finite sequence. Its [minimal walk along a club sequence](../../../../../../../minimal-walk-along-a-club-sequence.md) is finite because its nodes strictly decrease until reaching $\alpha$, and an infinite strictly decreasing sequence of [ordinals](../../../../../../../ordinal.md) cannot exist. At a step from $\delta>\alpha$, unboundedness of $C_\delta$ supplies $\min(C_\delta\setminus\alpha)$ in $[\alpha,\delta)$.

Compare the two [minimal walks along a club sequence](../../../../../../../minimal-walk-along-a-club-sequence.md) to $\xi$ and to $\alpha$. As long as their current node is the same $\delta>\alpha$, their next nodes agree exactly when $C_\delta$ has no point in $[\xi,\alpha)$. At the first such point, the walk to $\xi$ moves to

$$
\min(C_\delta\setminus\xi)\in[\xi,\alpha),
$$

whereas the walk to $\alpha$ stays at or above $\alpha$. If this does not occur before the second walk terminates, the first walk reaches $\alpha$ with it and then makes its next step below $\alpha$.

Thus there is an index $j$, possibly the terminal index of the walk to $\alpha$, with

$$
\boxed{\beta_i^\xi=\beta_i^\alpha\ (i\leq j),\qquad
\xi\leq\beta_{j+1}^\xi<\alpha.}
$$

It is unique: after this step the first walk stays below $\alpha$, so it can never again coincide with a node of the walk to $\alpha$. This is the [first-divergence lemma for minimal walks](../../../../../../../first-divergence-lemma-for-minimal-walks.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 24](../../../../paper-24-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
