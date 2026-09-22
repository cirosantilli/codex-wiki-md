<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take $D=\langle(12)(34)\rangle$ and

$$
P=\{1,(12)(34),(13)(24),(14)(23)\}.
$$

Every involution in $A_5$ is a double transposition. They form one conjugacy class: an odd $S_5$ conjugator can be made even by multiplying by a transposition centralizing the source double transposition. Thus all order-two subgroups of $A_5$ are conjugate. Since $|A_5|=60$, $P$ is a [Sylow subgroup](../../../../../../sylow-subgroup.md). A permutation normalizing $P$ fixes its unique common fixed letter, $5$, and every even permutation of the other four letters permutes its three double transpositions. Hence $N_{A_5}(P)=A_4$. Any permutation centralizing $(12)(34)$ fixes $5$; within $S_4$ it may exchange the two pairs and interchange letters in either pair, giving eight possibilities, of which exactly the four elements of $P$ are even. Thus $C_{A_5}(D)=P$. Since $P$ is abelian and contains $D$, also $C_{A_5}(P)=P$.

The given single block of $kA_4$ has identity $1$ and defect $P$, since $\operatorname{Br}_P^{A_4}(1)=1$ and $P$ is Sylow. By [Brauer first main theorem](../../../../../../brauer-first-main-theorem.md), $kA_5$ has exactly one block with defect $P$.

Suppose a block idempotent $b$ had defect $D$. Then $\operatorname{Br}_D^{A_5}(b)$ is a nonzero idempotent in $kP$. A [group algebra of a p-group in characteristic p is local](../../../../../../group-algebra-of-a-p-group-in-characteristic-p-is-local.md), so this image is $1$. But both the Brauer projections at $D$ and at $P$ retain exactly the basis elements of the same centralizer $P$. Consequently

$$
\operatorname{Br}_P^{A_5}(b)=\operatorname{Br}_D^{A_5}(b)=1.
$$

Thus $b$ has the full Sylow defect $P$, contradicting maximality of $D$. These are the [2-modular defect groups of A5](../../../../../../2-modular-defect-groups-of-a5.md), and $\boxed{C_2\text{ cannot be a defect group}}$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 138](../../../paper-138-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
