# Elston-Stewart algorithm

↑ **Parent:** [Pedigree likelihood](pedigree-likelihood.md)

Pedigree peeling eliminates latent [genotypes](genotype.md) by moving sums inside products whenever the other factors do not depend on the eliminated genotype. For one parent genotype $g$ and one child genotype $h$, the likelihood becomes

$$
\sum_g P(g)P(X_p\mid g)\left[\sum_hP(h\mid g)P(X_c\mid h)\right].
$$

The inner bracket is the child's message to its parent. With two states each, it needs four multiplications and two additions; multiplying the two parent weights and messages needs four more multiplications and the final sum one addition. The unrearranged four terms instead use twelve multiplications. Larger pedigrees use the same variable-elimination identity, with additional handling of pedigree loops.

## ↑ Ancestors (5)

1. [Pedigree likelihood](pedigree-likelihood.md)
2. [Pedigree](pedigree.md)
3. [Genetics](genetics.md)
4. [Biology](biology-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-39/3/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-45/1/f/solution.md)
