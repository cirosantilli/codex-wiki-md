<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Take $R=\mathbb Z$, $M=\mathbb Q/\mathbb Z$, and $k=2$. The group $M$ is nonzero and divisible. Since every element of $M$ has finite order, $M$ is the filtered union of finite cyclic groups. For every $n\geq1$,

$$
(\mathbb Z/n\mathbb Z)\otimes_{\mathbb Z}M
\cong M/nM=0.
$$

Tensor products commute with filtered colimits, so

$$
M\otimes_{\mathbb Z}M=0.
$$

Now suppose a nonzero finitely generated $R$-module $M$ satisfied $M^{\otimes k}=0$. Choose a [maximal ideal](../../../../../../maximal-ideal.md) $\mathfrak m$ in the [support](../../../../../../support-of-a-module.md) of $M$. The localized module $M_{\mathfrak m}$ is nonzero and finitely generated. By [Nakayama lemma](../../../../../../nakayama-lemma.md),

$$
M_{\mathfrak m}/\mathfrak mM_{\mathfrak m}\ne0.
$$

This is a nonzero vector space over the [residue field](../../../../../../residue-field.md) $\kappa(\mathfrak m)$, so its $k$-fold tensor power is nonzero. But it is the reduction modulo $\mathfrak m$ of $(M^{\otimes k})_{\mathfrak m}$, a contradiction. Thus a nonzero [tensor-nilpotent module](../../../../../../tensor-nilpotent-module.md) cannot be finitely generated.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
