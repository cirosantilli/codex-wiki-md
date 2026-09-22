<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $0\ne f:S^\lambda\to M^\mu$ be a module homomorphism. Since $S^\lambda$ is simple, $f$ is injective. Fix a $\lambda$-tableau $t$; its nonzero [polytabloid](../../../../../../polytabloid.md) $e_t$ then has $f(e_t)\ne0$. The sign sum in the column group satisfies

$$
\kappa_t^2=|C_t|\kappa_t,
$$

because every coefficient in the square receives $|C_t|$ equal contributions. Thus $\kappa_te_t=|C_t|e_t$, and equivariance gives

$$
\kappa_tf(e_t)=f(\kappa_te_t)=|C_t|f(e_t)\ne0.
$$

The [column antisymmetrizer](../../../../../../column-antisymmetrizer-of-a-young-tableau.md) therefore acts nontrivially on $M^\mu$, so some basis [tabloid](../../../../../../tabloid.md) $[s]$ has $\kappa_t[s]\ne0$. The stated [dominance from a nonzero column antisymmetrizer](../../../../../../dominance-from-a-nonzero-column-antisymmetrizer.md) yields

$$
\boxed{\operatorname{Hom}_{\mathbb CS_n}(S^\lambda,M^\mu)\ne0\Longrightarrow\lambda\unrhd\mu.}
$$

For $\mu=\lambda$, the same calculation forces $f(e_t)=|C_t|^{-1}\kappa_tf(e_t)$ into the one-dimensional space $\mathbb Ce_t$. Write $f(e_t)=ce_t$. Since $e_t$ generates the [Specht module](../../../../../../specht-module.md), equivariance gives $f(ge_t)=cge_t$ for every $g$, so $f$ is $c$ times the inclusion $S^\lambda\hookrightarrow M^\lambda$. That inclusion is nonzero, hence

$$
\boxed{\dim\operatorname{Hom}_{\mathbb CS_n}(S^\lambda,M^\lambda)=1.}
$$

As a useful consequence, if $S^\lambda\cong S^\mu$, their inclusions into $M^\lambda,M^\mu$ give dominance both ways. Antisymmetry of the [dominance order on partitions](../../../../../../dominance-order-on-partitions.md) then gives $\lambda=\mu$, so different partitions produce nonisomorphic simple modules.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
