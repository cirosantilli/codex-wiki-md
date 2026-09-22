<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $v=\operatorname{Var}(S)>0$ and $v_I=\operatorname{Var}(S_I)$. The variance-matching [quota share reinsurance](../../../../../../quota-share-reinsurance.md) in this part has the nonnegative retained fraction $\alpha^*=\sqrt{v_I/v}$. For claimwise retentions $0\leq h(x)\leq x$, its existence within $[0,1]$ follows from $v_I=\lambda\mathbb E[h(X)^2]\leq\lambda\mathbb E[X^2]=v$. The comparison below only needs the matching contract specified in the question.

Because $S_R=S-S_I$, the [variance](../../../../../../variance-split.md) and [covariance](../../../../../../covariance.md) identities give

$$
\operatorname{Var}(S_I)+\operatorname{Var}(S_R)
=v+2v_I-2\operatorname{Cov}(S,S_I).
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) bounds $\operatorname{Cov}(S,S_I)\leq\sqrt{vv_I}=\alpha^*v$. Therefore the [quota share comparison at matched retained variance](../../../../../../quota-share-comparison-at-matched-retained-variance.md) is

$$
\operatorname{Var}(S_I)+\operatorname{Var}(S_R)
\geq v+2(\alpha^*)^2v-2\alpha^*v
=\bigl((\alpha^*)^2+(1-\alpha^*)^2\bigr)v.
$$

The last expression is the sum of [variances](../../../../../../variance-split.md) under the matching [quota share reinsurance](../../../../../../quota-share-reinsurance.md). Hence

$$
\boxed{\operatorname{Var}(S_I^*)+\operatorname{Var}(S_R^*)
\leq\operatorname{Var}(S_I)+\operatorname{Var}(S_R).}
$$

If $v=0$, the given matching contract forces $v_I=0$, so all relevant totals are constant and equality holds. For $v>0$, equality in the bound is equivalent to $S_I-\mathbb E[S_I]=\alpha^*(S-\mathbb E[S])$ almost surely.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
