<h1 id="4/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Fix $\varepsilon>0$ and set $d=2/\varepsilon$. Suppose, towards a contradiction, that

$$
D=\operatorname{diam}_S(G)>\max\{|G|^\varepsilon,\lambda\},
$$

where $\lambda$ will absorb constants depending only on $\varepsilon$. Put $n=\lfloor|G|^\varepsilon\rfloor$. Once $\lambda$ is large enough, $n\geq N(d)$, $n<D$, and

$$
|S^n|\leq|G|\leq n^d|S|.
$$

Part (a) yields $H\trianglelefteq C<G$ with $[G:C]=O_\varepsilon(1)$, $H\subseteq S^{\lfloor n/2\rfloor}$, and $C/H$ nilpotent of class $O_\varepsilon(1)$.

The [subgroup core](../../../../../../../core-group-theory.md) $\bigcap_{g\in G}gCg^{-1}$ is normal in $G$ and has index at most $[G:C]!$. Since $G$ is a [simple group](../../../../../../../simple-group.md), the core is either $\{1\}$ or $G$. In the first case $|G|\leq [G:C]!=O_\varepsilon(1)$, which is excluded by increasing $\lambda$. Hence the core is $G$, so $C=G$.

Now $H\trianglelefteq G$. Since $n/2<D$, the ball $S^{\lfloor n/2\rfloor}$ is not all of $G$, so $H\ne G$. Simplicity gives $H=\{1\}$, and therefore $G=C/H$ is a [nilpotent group](../../../../../../../nilpotent-group.md). A nontrivial finite nilpotent group has nontrivial [center of a group](../../../../../../../center-of-a-group.md); simplicity would force that center to be all of $G$, making $G$ [Abelian](../../../../../../../abelian-group.md). This contradicts the assumption that $G$ is non-abelian. Consequently

$$
\boxed{\operatorname{diam}_S(G)\leq\max\{|G|^\varepsilon,\lambda(\varepsilon)\}.}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Paper 149](../../../../paper-149-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
