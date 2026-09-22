<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Suppose first that $\phi:G\to H$ is a $(\lambda,\varepsilon)$-quasi-isometry. If $k\in\ker\phi$, the lower quasi-isometry inequality gives

$$
\lambda^{-1}|k|_G-\varepsilon\leq d_H(1,\phi(k))=0,
$$

so the [kernel of a group homomorphism](../../../../../../kernel-of-a-group-homomorphism.md) lies in the finite word-metric ball of radius $\lambda\varepsilon$ and is finite. Coarse surjectivity gives an $R$ such that every $h\in H$ is within $R$ of $\phi(G)$. The finite ball $B_H(1,R)$ therefore contains representatives for every coset of $\phi(G)$, so $H/\phi(G)$ is finite.

Conversely, suppose $\ker\phi$ is finite and $phi(G)$ is a [finite-index subgroup](../../../../../../finite-index-subgroup.md) of $H$. The map factors as

$$
G\longrightarrow G/\ker\phi\xrightarrow{\ \cong\ }\phi(G)\hookrightarrow H.
$$

The first arrow is a [finite-kernel quotient quasi-isometry](../../../../../../finite-kernel-quotient-quasi-isometry.md), the middle arrow is an isomorphism of finitely generated groups, and the last arrow is a [finite-index subgroup quasi-isometry](../../../../../../finite-index-subgroup-quasi-isometry.md). Their composition is a quasi-isometry. Hence the [quasi-isometry criterion for a group homomorphism](../../../../../../quasi-isometry-criterion-for-a-group-homomorphism.md) is

$$
\boxed{\phi\text{ is a quasi-isometry}\iff |\ker\phi|<\infty\text{ and }[H:\phi(G)]<\infty.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 143](../../../paper-143-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
