# Pedigree likelihood

↑ **Parent:** [Pedigree](pedigree.md)

For latent [genotypes](genotype.md) $G_i$ and observed [phenotypes](phenotype.md) $X_i$, assume conditional phenotype independence, independent founder genotypes, and conditionally independent Mendelian transmissions. The [likelihood function](likelihood-function.md) is

$$
\sum_{(G_i)}\prod_i P(X_i\mid G_i)\prod_{i\in F}P(G_i)\prod_{i\notin F}P(G_i\mid G_{m(i)},G_{f(i)}).
$$

This follows by the chain rule applied to the acyclic ancestry graph, then the law of total probability over all latent genotypes. [Penetrance](penetrance.md) supplies the phenotype factors and [genetic recombination](genetic-recombination.md) supplies multilocus transmission factors.

**Table of contents**

- [Phase averaging in a linkage likelihood](phase-averaging-in-a-linkage-likelihood.md)
  - [Score equation for a phase-averaged linkage likelihood](score-equation-for-a-phase-averaged-linkage-likelihood.md)
- [Pedigree graphical model](pedigree-graphical-model.md)
- [Elston-Stewart algorithm](elston-stewart-algorithm.md)

## ↑ Ancestors (4)

1. [Pedigree](pedigree.md)
2. [Genetics](genetics.md)
3. [Biology](biology-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (16)

- [Founder in a pedigree](founder-in-a-pedigree.md)
- [Genetic-study ascertainment](genetic-study-ascertainment.md)
- [Junction-tree sum-product message](junction-tree-sum-product-message.md)
- [Parametric linkage analysis](parametric-linkage-analysis.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-29/6/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-29/6/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-29/6/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-40/5/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-40/5/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-39/3/d/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-39/3/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-45/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-45/1/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-45/1/a/solution.md)
- [Phase averaging in a linkage likelihood](phase-averaging-in-a-linkage-likelihood.md)
- [Phenotype](phenotype.md)
