<h1 id="24f/solution">Solution</h1>

↑ **Parent:** [24F](../24f.md)

A function element is a pair $(f,D)$ consisting of a domain $D\subseteq G$ and a [holomorphic function](../../../../../holomorphic-function.md) $f:D\to\mathbb C$ belonging to the given complete analytic function. Its [germ of a holomorphic function](../../../../../germ-of-a-holomorphic-function.md) at $z\in D$ is the equivalence class $[f]_z$, where two elements are equivalent when they agree on a neighbourhood of $z$.

For every function element $(f,D)$ and sufficiently small open $U\subseteq D$, set

$$
U_f=\{[f]_z:z\in U\}.
$$

These sets form a basis for the [space of germs of holomorphic functions](../../../../../space-of-germs-of-holomorphic-functions.md). The projection

$$
\pi:\mathcal G\to G,
\qquad \pi([f]_z)=z,
$$

restricts to a homeomorphism $U_f\to U$. The inverse projections $\pi|_{U_f}$ are compatible complex charts, making $\mathcal G$ a [Riemann surface](../../../../../riemann-surfaces.md) and $\pi$ a covering map and local biholomorphism. In such a chart, the [evaluation map on a space of germs](../../../../../evaluation-map-on-a-space-of-germs.md) has coordinate expression

$$
\mathcal E\circ(\pi|_{U_f})^{-1}(z)=f(z).
$$

It is therefore holomorphic on every chart, hence analytic on each component of $\mathcal G$.

Now let $f:R\to S$ be a nonconstant analytic map of compact connected Riemann surfaces, and let $B$ be its finite branch-value set. Each point of $B$ is a [branch value of a holomorphic map](../../../../../branch-value-of-a-holomorphic-map.md). At every point of $R\setminus f^{-1}(B)$ the local degree is one, so the holomorphic inverse-function theorem supplies a neighbourhood on which $f$ is biholomorphic. For $y\in S\setminus B$, the fibre is finite. Choose disjoint inverse neighbourhoods around all its points and shrink their common image; compactness, or equivalently properness of $f$, ensures that no additional preimages enter. Thus

$$
f:R\setminus f^{-1}(B)\longrightarrow S\setminus B
$$

is an ordinary unramified covering map.

Fix $P\in S\setminus B$. Given a loop $\gamma$ based at $P$, lift it from every $Q\in f^{-1}(P)$ and send $Q$ to the endpoint of its lift. The [path lifting theorem](../../../../../path-lifting-theorem.md) makes this a permutation; concatenation of loops composes the permutations and reversal gives inverses. Its image is the [monodromy group of a covering](../../../../../monodromy-group-of-a-covering.md). The punctured surface $R\setminus f^{-1}(B)$ is path connected. Given two points of the fibre, join them there by a path; its projection is a loop whose lift joins those points. Hence the monodromy action is transitive.

Finally consider

$$
F(z)=z^2+z^{-2}=\frac{z^4+1}{z^2}.
$$

It has degree four. Its finite critical points satisfy

$$
F'(z)=2z-2z^{-3}=0,
\qquad z^4=1,
$$

with branch values $2$ and $-2$; the double poles at zero and infinity give the branch value infinity. For a regular value, the fibre is

$$
\{z,-z,z^{-1},-z^{-1}\}.
$$

The two commuting involutions $z\mapsto-z$ and $z\mapsto z^{-1}$ preserve $F$ and act transitively on this fibre. They generate all four deck transformations, so the covering is normal and its monodromy group is

$$
\boxed{\ H\cong V_4=C_2\times C_2.\ }
$$

With the displayed ordering of the fibre, its elements are

$$
1,\qquad(12)(34),\qquad(13)(24),\qquad(14)(23).
$$

This is the [monodromy group of z squared plus z to the minus two](../../../../../monodromy-group-of-z-squared-plus-z-to-the-minus-two.md).

## ↑ Ancestors (10)

1. [24F](../24f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
