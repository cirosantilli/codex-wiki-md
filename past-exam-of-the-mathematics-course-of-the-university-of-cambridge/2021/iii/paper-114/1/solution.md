<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Choose the intersection point $p=[(\theta_0,\theta_1)]$ as the zero-cell. Let $a$ be the horizontal one-cell $S^1\times\{\theta_1\}$ and $b$ the vertical one-cell $\{\theta_0\}\times S^1$. The usual [CW complex](../../../../../cw-complex.md) structure on the [torus](../../../../../torus.md) has one two-cell $c$ attached by the word $aba^{-1}b^{-1}$, and the extra disk gives a two-cell $d$ attached along $b$ with degree one. Collapsing $a$ leaves one zero-cell $p$, one one-cell $b$, and the two two-cells $c,d$. The [cellular boundary formula](../../../../../cellular-boundary-formula.md) gives

$$
C_2\cong\mathbb Zc\oplus\mathbb Zd,
\qquad
C_1\cong\mathbb Zb,
\qquad
\partial_2(c)=0,quad\partial_2(d)=b.
$$

Therefore

$$
H_i(X;\mathbb Z)\cong
\begin{cases}
\mathbb Z,&i=0,2,\\
0,&\text{otherwise}.
\end{cases}
$$

The [Excision theorem](../../../../../excision-theorem.md) says that if $Z\subseteq A\subseteq X$ and $\overline Z\subseteq\operatorname{int}A$, then inclusion induces

$$
H_i(X\setminus Z,A\setminus Z)\xrightarrow{\sim}H_i(X,A).
$$

It lets us compute [local homology](../../../../../local-homology.md) in arbitrarily small neighborhoods.

Let $C\subseteq X$ be the image of $\{\theta_0\}\times S^1$. At a point of $X\setminus C$, a neighborhood is a disk, whose link is a circle. At a point of $C\setminus\{p\}$, three half-disks meet along their diameters, and the link is a [Theta graph](../../../../../theta-graph.md), with first homology $\mathbb Z^2$. At $p$, the two folds created by collapsing the horizontal circle give a [dumbbell graph](../../../../../dumbbell-graph.md) as link: two circles joined by an interval. Its first homology is again $\mathbb Z^2$. The [local homology from a link](../../../../../local-homology-from-a-link.md) therefore gives

$$
H_i(X,X\setminus\{x\};\mathbb Z)
\cong
\begin{cases}
\mathbb Z^2,&i=2\text{ and }x\in C,\\
\mathbb Z,&i=2\text{ and }x\notin C,\\
0,&\text{otherwise}.
\end{cases}
$$

Because [local homology](../../../../../local-homology.md) is invariant under a [homeomorphism](../../../../../homeomorphism.md), every self-homeomorphism of $X$ preserves the rank-two locus $C$.

It must also preserve $p$. Indeed, $p$ is the unique point of $C$ whose sufficiently small local link is a dumbbell graph; every other point of $C$ has a theta-graph link. The connecting edge of a dumbbell graph is a [bridge in a graph](../../../../../bridge-graph-theory.md), whereas no edge of a theta graph is a bridge, so these local topological types are distinct.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 114](../../paper-114-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
