<h1 id="14f/solution">Solution</h1>

↑ **Parent:** [14F](../14f.md)

If an open set meets $\overline A$, it meets $A$. Thus if two open sets meet the closure of an irreducible set, they both meet $A$, their intersection meets $A$ by irreducibility, and therefore it also meets $\overline A$. This proves irreducibility of the closure. A singleton is irreducible, so its closure is an [irreducible closed subset](../../../../../irreducible-closed-subset.md).

In a [Hausdorff space](../../../../../hausdorff-space.md), two distinct points have disjoint open neighborhoods. An irreducible set cannot contain both, so every nonempty irreducible closed subset is a singleton, which is closed and has a unique generating point. Hence every Hausdorff space is a [sober topological space](../../../../../sober-space.md). An infinite set with the [cofinite topology](../../../../../cofinite-topology.md) is itself irreducible, because any two nonempty open sets meet, but every singleton is closed. Its whole space is therefore not the closure of a singleton, proving that it is not sober.

For the proposed [sobrification](../../../../../sobrification.md), let $\widehat X$ consist of nonempty irreducible closed subsets. The basic operations are

$$
\widehat\varnothing=\varnothing,\quad
\widehat X=\widehat{\,X\,},\quad
\widehat{\bigcup_\alpha U_\alpha}=\bigcup_\alpha\widehat U_\alpha,\quad
\widehat U\cap\widehat V=\widehat{U\cap V}.
$$

The last identity uses irreducibility of each member of $\widehat X$. Hence these sets already form a topology. The map $U\mapsto\widehat U$ is injective: $\overline{\{x\}}$ meets an open $U$ exactly when $x\in U$, so equality of the hats forces equality of the original opens. It is surjective onto the topology just constructed by definition.

Now let $C$ be a nonempty irreducible closed subset of $\widehat X$. Its complement is $\widehat W$ for a unique open $W\subseteq X$. Put $F=X\setminus W$. Then

$$
C=\{A\in\widehat X:A\subseteq F\}.
$$

If opens $U,V$ meet $F$, choose points in those intersections. Their singleton closures lie in $C$, so $\widehat U,\widehat V$ meet $C$. Irreducibility of $C$ forces $\widehat{U\cap V}$ to meet $C$, and hence $U\cap V$ meets $F$. Thus $F$ is nonempty, closed and irreducible, so $F$ is itself a point of $\widehat X$.

The closure of this point in $\widehat X$ is exactly $\{A:A\subseteq F\}$: inclusion makes every open meeting $A$ meet $F$, whereas a point of $A\setminus F$ is separated by the open $X\setminus F$. Hence $C=\overline{\{F\}}$. Any other point $G$ with the same closure satisfies $G\subseteq F$ and $F\subseteq G$, forcing $F=G$. This proves **the constructed space is sober**.

## ↑ Ancestors (10)

1. [14F](../14f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
