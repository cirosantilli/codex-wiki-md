<h1 id="2/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Use the fixed common entry law from the printed setup: $Y=\sqrt N X_{ij}$ has mean zero and [second moment](../../../../../../second-moment.md) $1$ for each upper-triangular entry, including the diagonal. Let

$$
Z_C=Y\mathbf1_{\{|Y|\geq C\}},\qquad t(C)=\mathbb E[Y^2\mathbf1_{\{|Y|\geq C\}}].
$$

Since $\mathbb EY=0$, the removed part after [centered truncation of a Wigner matrix](../../../../../../centered-truncation-of-a-wigner-matrix.md) is

$$
\Delta_{ij}=X_{ij}-\widehat X_{ij}=N^{-1/2}(Z_{C,ij}-\mathbb EZ_C).
$$

Consequently $\mathbb E\Delta_{ij}^2=N^{-1}\operatorname{Var}(Z_C)\leq N^{-1}t(C)$. Symmetry gives $\operatorname{Tr}\Delta^2=\sum_{i,j}\Delta_{ij}^2$. There are $N$ diagonal terms and $N(N-1)$ off-diagonal terms in this sum, so

$$
\mathbb E\left[\frac1N\operatorname{Tr}\Delta^2\right]=\operatorname{Var}(Z_C)\leq t(C).
$$

Mirrored entries are counted twice, as they must be; independence of those mirrored entries is neither true nor needed for this [expectation](../../../../../../expected-value.md) calculation.

By the preceding bound and the [Markov inequality](../../../../../../markov-inequality.md),

$$
\mathbb P\{D>\varepsilon\}\leq\mathbb P\left\{\frac1N\operatorname{Tr}\Delta^2>\varepsilon^2\right\}\leq\frac{t(C)}{\varepsilon^2}.
$$

The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) applies to $Y^2\mathbf1_{\{|Y|\geq C\}}\leq Y^2$, so $t(C)\to0$. Choose $C$ with $t(C)<\varepsilon^3$. Then

$$
\boxed{\mathbb P\{|\langle L_N,f\rangle-\langle\widehat L_N,f\rangle|>\varepsilon\}<\varepsilon\quad\text{for every }N.}
$$

This [second moment bound for spectral truncation](../../../../../../second-moment-bound-for-spectral-truncation.md) depends only on $\varepsilon$ and the common law of $Y$, and is uniform over [functions](../../../../../../function-split.md) with [Lipschitz bound](../../../../../../lipschitz-bound.md) $1$. No fourth-moment hypothesis is required. If the scaled entry law were allowed to vary arbitrarily with $N$, a uniform choice would instead require uniform decay of its second-moment tails; the intended fixed-law setting supplies exactly that condition.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [2](../../2.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
