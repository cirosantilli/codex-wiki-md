<h1 id="2c/solution">Solution</h1>

↑ **Parent:** [2C](../2c.md)

A [group automorphism](../../../../../group-automorphism.md) is a bijective [group homomorphism](../../../../../group-homomorphism.md) from $G$ to itself. The multiplication in $\operatorname{Aut}(G)$ is composition: $(\alpha\beta)(g)=\alpha(\beta(g))$. Composition is associative, the identity map is the identity element, and each inverse [bijection](../../../../../bijection.md) is again a [homomorphism](../../../../../homomorphism.md), so these maps form the [automorphism group](../../../../../automorphism-group.md).

For conjugation by $h$, multiplication is preserved because

$$
h(g_1g_2)h^{-1}=(hg_1h^{-1})(hg_2h^{-1}).
$$

Conjugation by $h^{-1}$ is its inverse, so $\psi(h)$ is an [group automorphism](../../../../../group-automorphism.md). Moreover

$$
\psi(h_1h_2)(g)=h_1h_2g h_2^{-1}h_1^{-1}
=\psi(h_1)(\psi(h_2)(g)).
$$

Hence **$\psi:G\to\operatorname{Aut}(G)$ is a [homomorphism](../../../../../homomorphism.md)**, with image the [inner automorphisms](../../../../../inner-automorphism.md). Its [group homomorphism kernel](../../../../../kernel-of-a-group-homomorphism.md) is the [group center](../../../../../center-of-a-group.md) of $G$, since $\psi(h)$ is the identity precisely when $hg=gh$ for every $g$.

## ↑ Ancestors (10)

1. [2C](../2c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
