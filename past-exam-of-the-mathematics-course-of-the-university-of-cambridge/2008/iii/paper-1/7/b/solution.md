<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $M=\lambda(\Gamma)''$, the [group von Neumann algebra](../../../../../../group-von-neumann-algebra.md), and define right translations by $\rho(g)\delta_h=\delta_{hg^{-1}}$. Left and right translations commute, so every $T\in M$ commutes with every $\rho(g)$. A [Von Neumann factor](../../../../../../von-neumann-factor.md) means that the center of $M$ is exactly $\mathbb CI$.

Suppose every nonidentity [conjugacy class](../../../../../../conjugacy-class.md) is infinite and $T$ is central. Put $\eta=T\delta_e$. Since $T$ commutes with both regular actions and $\lambda(g)\rho(g)\delta_e=\delta_e$,

$$
\lambda(g)\rho(g)\eta=\eta.
$$

The action on a [basis](../../../../../../basis.md) [vector](../../../../../../vector.md) is $\delta_h\mapsto\delta_{ghg^{-1}}$, so the coefficients of $\eta\in\ell^2(\Gamma)$ are constant on conjugacy classes. A nonzero constant on an infinite class would have infinite squared sum. Thus all coefficients away from the identity vanish and $\eta=c\delta_e$.

Commutation with the right action now gives $T\delta_h=c\delta_h$ for every $h$, because those [vectors](../../../../../../vector.md) form the right orbit of $\delta_e$. Hence $T=cI$ and $M$ is a factor. This argument also shows that $\delta_e$ is separating for $M$.

Conversely, if a nonidentity class $C$ is finite, then

$$
Z=\sum_{h\in C}\lambda(h)\in M
$$

commutes with every $\lambda(g)$, since conjugation permutes $C$. Therefore $Z\in M\cap\lambda(\Gamma)'=Z(M)$. It is not scalar: $Z\delta_e=\sum_{h\in C}\delta_h$ is nonzero and orthogonal to $\delta_e$. Consequently $M$ is not a factor. We have proved

$$
\boxed{\lambda(\Gamma)''\text{ is a factor}\iff\Gamma\text{ is an ICC group}.}
$$

The condition is vacuous for the trivial [group](../../../../../../group-split.md), whose algebra $\mathbb CI$ is indeed a factor.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7](../../7.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
