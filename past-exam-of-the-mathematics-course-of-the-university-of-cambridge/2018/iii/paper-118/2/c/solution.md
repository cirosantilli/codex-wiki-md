<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The restriction maps of this point sheaf satisfy the presheaf composition identities: every possible restriction is either the identity on $\mathbb C$ or the unique map to the zero group. We check the sheaf identity and gluing axioms for any open cover $U=\bigcup_iU_i$.

If $p\notin U$, every section group in the cover is zero, so a compatible family has the unique zero gluing. If $p\in U$, at least one $U_i$ contains $p$. For any two members containing $p$, their intersection also contains $p$, and compatibility forces their complex values to be equal, since the restriction maps there are identities. Call the common value $c$. Members not containing $p$ have only the zero section. The section $c\in\mathbb C_p(U)$ restricts to every member of the family, proving existence of a gluing; its restriction to any member containing $p$ determines $c$, proving uniqueness.

This also proves local identity for sections, and $\mathbb C_p(\varnothing)=0$ handles the empty open set. Hence

$$
\boxed{\mathbb C_p\text{ is a sheaf of abelian groups}.}
$$

It is the point-pushforward sheaf, usually called a [skyscraper sheaf](../../../../../../skyscraper-sheaf.md). Its restrictions are all surjective, so it is also a [flasque sheaf](../../../../../../flasque-sheaf.md). No separation assumption on $X$ is needed for the preceding sheaf-axiom argument.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 118](../../../paper-118-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
