<h1 id="20h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $V_4=\langle u,v\mid u^2=v^2=[u,v]=1\rangle$. Define a surjection

$$
\phi:\pi_1(X_n)\longrightarrow V_4,
\qquad
\phi(a_1)=u,\quad\phi(b)=v,\quad
\phi(a_i)=1\ (i>1).
$$

Its kernel determines a connected regular [four-sheeted cover of a wedge of circles and a real projective plane](../../../../../../four-sheeted-cover-of-a-wedge-of-circles-and-a-real-projective-plane.md), say $\widetilde X_n\to X_n$.

Use the CW structure on $X_n$ with one vertex, one edge for every $a_i$ and for $b$, and one two-cell attached along $b^2$. In the regular cover, the degree-two cellular chain group is

$$
C_2(\widetilde X_n)\cong\mathbb Z[V_4].
$$

The [cellular boundary formula](../../../../../../cellular-boundary-formula.md) gives the lifted attaching word $b^2$ the boundary

$$
\partial_2(c)=(1+v)c
$$

in the $b$-edge summand of $C_1$. Therefore

$$
\ker\partial_2
=\mathbb Z(1-v)\oplus\mathbb Z(u-uv)
\cong\mathbb Z^2.
$$

There are no three-cells, so

$$
\boxed{H_2(\widetilde X_n;\mathbb Z)\cong\mathbb Z^2.}
$$

If $X_n$ were homotopy equivalent to a compact connected surface $S$, the subgroup corresponding to this cover would produce a connected four-sheeted cover $\widetilde S$ homotopy equivalent to $\widetilde X_n$. A finite cover of a compact surface is again a compact connected surface. But the [integral top homology of a compact connected surface](../../../../../../integral-top-homology-of-a-compact-connected-surface.md) has rank at most one, contradicting the displayed rank two. Hence **$X_n$ is not homotopy equivalent to a compact connected surface for any $n\geq1$.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [20H](../../20h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
