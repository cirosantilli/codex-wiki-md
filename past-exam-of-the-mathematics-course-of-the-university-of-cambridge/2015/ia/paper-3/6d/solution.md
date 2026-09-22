<h1 id="6d/solution">Solution</h1>

↑ **Parent:** [6D](../6d.md)

A [group homomorphism](../../../../../group-homomorphism.md) satisfies $\varphi(ab)=\varphi(a)\varphi(b)$ for every $a,b\in G$. Its [kernel of a group homomorphism](../../../../../kernel-of-a-group-homomorphism.md) is $K=\{g:\varphi(g)=e_H\}$. The homomorphism equation gives $\varphi(e_G)=e_H$ by cancellation, and $\varphi(g^{-1})=\varphi(g)^{-1}$. Therefore $K$ contains the identity and is closed under multiplication and inverses, so it is a [subgroup](../../../../../subgroup.md).

For $k\in K$ and $x\in G$,

$$
\varphi(x^{-1}kx)=\varphi(x)^{-1}e_H\varphi(x)=e_H.
$$

Thus conjugation carries $K$ into itself, and applying the inverse conjugation gives equality: $K$ is a [normal subgroup](../../../../../normal-subgroup.md). If $K=\{e,\xi\}$, conjugation cannot send $\xi$ to the identity because it is injective. Consequently

$$
\boxed{x^{-1}\xi x=\xi\quad\text{for every }x\in G.}
$$

This proves directly the [normal subgroup of order two is central](../../../../../normal-subgroup-of-order-two-is-central.md) principle for kernels, including the kernel facts needed below.

## ↑ Ancestors (10)

1. [6D](../6d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
