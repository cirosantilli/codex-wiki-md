<h1 id="13j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $n_\ell$ be the number of graduates in college $\ell$. In model 1, every edge from a person in college $k$ to a person in college $\ell$ has probability

$$
p_{k\ell}^{(1)}=\operatorname{logit}^{-1}(\beta_{k\ell}),
$$

so

$$
M_i,M_j\stackrel{\mathrm{iid}}{\sim}
\operatorname{Bin}(n_\ell,p_{k\ell}^{(1)}).
$$

In model 2 the corresponding probability is

$$
p_{k\ell}^{(2)}=\operatorname{logit}^{-1}(\beta_k+\beta_\ell).
$$

Because $k\ne\ell$, the within-college indicator in model 3 vanishes, so $p_{k\ell}^{(3)}=p_{k\ell}^{(2)}$. Consequently models 2 and 3 both give

$$
M_i,M_j\stackrel{\mathrm{iid}}{\sim}
\operatorname{Bin}(n_\ell,p_{k\ell}^{(2)}).
$$

The distinct edge indicators used in $M_i$ and $M_j$ are independent under all three models, so every model also forces $M_i$ and $M_j$ to be independent. Thus **all members of one college have the same cross-college friendship propensity, with no person-level heterogeneity or dependence between their friendship counts**. Real friendship networks can have unusually sociable individuals and correlated choices of friends, producing [overdispersion](../../../../../../overdispersion.md) and dependence that these models cannot fit.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [13J](../../13j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
