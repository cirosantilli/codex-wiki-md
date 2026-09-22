<h1 id="23f/solution">Solution</h1>

↑ **Parent:** [23F](../23f.md)

In local coordinates centred at $p$ and $f(p)$, a nonconstant rational map has the form

$$
w=z^{e_p}u(z),\qquad u(0)\ne0.
$$

The point $p$ is a [ramification point of a holomorphic map](../../../../../ramification-point-of-a-holomorphic-map.md) when its [ramification index of a holomorphic map](../../../../../ramification-index-of-a-holomorphic-map.md) satisfies $e_p>1$. A [branch value of a holomorphic map](../../../../../branch-value-of-a-holomorphic-map.md), also called a branch point in the target, is a value $f(p)$ of some ramification point.

Let $B$ be the finite set of branch values and put $R=f^{-1}(B)$. For every $w\notin B$, all points of $f^{-1}(w)$ have local degree one, so the [holomorphic inverse function theorem](../../../../../holomorphic-inverse-function-theorem.md) supplies disjoint neighbourhoods on which $f$ is biholomorphic. Compactness of the fibre lets their target neighbourhoods be intersected to one evenly covered neighbourhood of $w$. Hence

$$
\boxed{f:\mathbb C_\infty\setminus R
\longrightarrow\mathbb C_\infty\setminus B}
$$

is an unramified covering map. Here the displayed restriction requires $R=f^{-1}(B)$; if “ramification point” is reserved only for points with $e_p>1$, then the source deletion must be written $f^{-1}(B)$.

The [Monodromy theorem](../../../../../monodromy-theorem.md) says that analytic continuations along endpoint-fixed homotopic paths have the same terminal germ. Equivalently here, the [path lifting theorem](../../../../../path-lifting-theorem.md) lifts a loop $\gamma$ based at $w\notin B$ from each point of $f^{-1}(w)$; taking the endpoint of each lift permutes that fibre. The permutation depends only on $[\gamma]\in\pi_1(\mathbb C_\infty\setminus B,w)$, giving the [monodromy group of a covering](../../../../../monodromy-group-of-a-covering.md).

For the stated function, make the Möbius change of coordinate

$$
t=\frac1{1-z}.
$$

Then

$$
f(z)=t^4-t^2.
$$

The critical points are $t=0,\pm1/\sqrt2,\infty$, with branch values

$$
0,\qquad-\frac14,\qquad\infty.
$$

A loop around $0$ interchanges the two roots born from $t=0$, so its branch cycle is a transposition. A loop around $-1/4$ simultaneously interchanges the two pairs that collide there, so its branch cycle is a product of two disjoint transpositions. With a suitable labelling these are

$$
(34),\qquad(13)(24).
$$

They generate a transitive group of order eight; their product is a four-cycle. Therefore the full monodromy group is

$$
\boxed{D_4\le S_4},
$$

the [dihedral group](../../../../../dihedral-group.md) in its action on the four vertices of a square.

## ↑ Ancestors (10)

1. [23F](../23f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
