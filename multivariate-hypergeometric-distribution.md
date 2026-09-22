# Multivariate hypergeometric distribution

↑ **Parent:** [Hypergeometric distribution](hypergeometric-distribution.md)

Suppose a finite population is split into $m$ categories with fixed sizes $c_1,\ldots,c_m$ summing to $n$. A uniform size-$r$ sample drawn by [sampling without replacement](sampling-without-replacement.md) has category counts $K_1,\ldots,K_m$ with the displayed [joint probability mass function](joint-probability-mass-function.md), for [integers](integer-split.md) $0\leq k_i\leq c_i$ summing to $r$. It extends the two-category [hypergeometric distribution](hypergeometric-distribution.md); replacing the sampled objects instead gives a [multinomial distribution](multinomial-distribution.md).

For a box with category sizes $(5,3,2)$ and a sample of four distinct objects, the count pattern $(2,1,1)$ has [probability](probability.md)

$$
\frac{\binom52\binom31\binom21}{\binom{10}4}
=\frac{60}{210}=\frac27.
$$

Put $p_i=c_i/n$. When $n>1$, its [covariance matrix](covariance-matrix.md) is the corresponding [multinomial distribution](multinomial-distribution.md) [covariance matrix](covariance-matrix.md) multiplied by the squared [finite population correction](finite-population-correction.md):

$$
\operatorname{Var}(K_i)=rp_i(1-p_i)\frac{n-r}{n-1},
\qquad
\operatorname{Cov}(K_i,K_j)=-rp_ip_j\frac{n-r}{n-1}\quad(i\ne j).
$$

This connects the fixed-total dependence between categories with the further reduction from [sampling without replacement](sampling-without-replacement.md). X. G. Duan gives a symmetry-based explanation of this shared [covariance](covariance.md) structure.[Duan, Better understanding of the multivariate hypergeometric distribution, 2021 preprint](https://arxiv.org/abs/2101.00548)

## ↑ Ancestors (8)

1. [Hypergeometric distribution](hypergeometric-distribution.md)
2. [Discrete probability distribution](discrete-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Multinomial distribution](multinomial-distribution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2/17/b/solution.md)
