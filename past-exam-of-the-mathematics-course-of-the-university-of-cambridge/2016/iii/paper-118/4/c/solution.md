<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Treat $0$ as the trivial group if $G$ is not abelian. The restriction maps satisfy the presheaf identities. To verify the [sheaf gluing axiom](../../../../../../sheaf-gluing-axiom.md), take an [open cover](../../../../../../open-cover.md) $(V_i)$ of $U$. If $x\notin U$, every section group is trivial. If $x\in U$, at least one $V_i$ contains $x$. Every two such opens have an overlap containing $x$, so compatibility forces all their sections to have the same value $g\in G$. Opens not containing $x$ have their unique trivial section. The value $g\in\mathcal G(U)$ is exactly the unique glued section. Thus **the stated presheaf is a skyscraper sheaf**, including for nonabelian groups.

For the [stalk of a sheaf](../../../../../../stalk-of-a-sheaf.md), take the direct limit over neighbourhoods of $y$. If some neighbourhood $V$ of $y$ omits $x$, neighbourhoods inside $V$ are cofinal and all their groups are trivial. If every neighbourhood of $y$ contains $x$, every group in the system is $G$ and every transition map is the identity. Consequently, on the arbitrary [topological space](../../../../../../topological-space.md) in the question,

$$
\boxed{\mathcal G_y\cong
\begin{cases}
G,&y\in\overline{\{x\}},\\
0,&y\notin\overline{\{x\}}.
\end{cases}}
$$

Membership in this [closure](../../../../../../closure-topology.md) means exactly that every neighbourhood of $y$ contains $x$. In particular $\mathcal G_x=G$. If $x$ is a [closed point](../../../../../../closed-point.md), the [closure](../../../../../../closure-topology.md) is just $\{x\}$ and the familiar point-supported answer results. The separation assumption is not present in the printed question, so it cannot be imposed silently.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 118](../../../paper-118-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
