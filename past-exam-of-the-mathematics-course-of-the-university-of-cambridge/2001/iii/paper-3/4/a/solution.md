<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose $\alpha\in\Omega$. Since $G$ acts regularly, $g\mapsto g\alpha$ identifies $\Omega$ with the underlying set of $G$, and the given action becomes left multiplication $L_g(x)=gx$.

A [permutation](../../../../../../permutation.md) $c$ centralizing all $L_g$ satisfies

$$
c(x)=c(L_x(1))=L_x(c(1))=xc(1).
$$

Conversely every right translation commutes with every left translation. To make the multiplication convention explicit, define $R_g(x)=xg^{-1}$. Then $R_gR_h(x)=xh^{-1}g^{-1}=x(gh)^{-1}=R_{gh}(x)$, using rightmost-first composition. The map $g\mapsto R_g$ is injective and its image is the entire [centralizer](../../../../../../centralizer.md), since any possible $c(1)$ can be written $g^{-1}$. Thus

$$
\boxed{C_{\operatorname{Sym}(\Omega)}(G)\cong G.}
$$

This is [centralizer of a regular permutation subgroup](../../../../../../centralizer-of-a-regular-permutation-subgroup.md). If one instead writes right multiplication as $x\mapsto xg$, the resulting map is an antihomomorphism; including the inverse avoids suppressing that reversal. Choosing a different base point changes the identification but not the isomorphism type.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
