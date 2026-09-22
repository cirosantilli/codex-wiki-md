# Poisson approximation bound for dependent Bernoulli variables

↑ **Parent:** [Poisson distribution](poisson-distribution.md)

For Bernoulli random variables $X_1,\ldots,X_n$, which need not be independent, put $p_i=\mathbb P(X_i=1)$, $S=\sum_iX_i$, and $\lambda=\sum_ip_i$. Then

$$
D_e\bigl(\mathcal L(S)\Vert\operatorname{Poisson}(\lambda)\bigr)
\leq\sum_ip_i^2+\sum_iH_e(X_i)-H_e(X_1,\ldots,X_n).
$$

The dependence penalty is the [total correlation](total-correlation.md). The proof compares the joint Bernoulli law with the product of Poisson laws of means $p_i$, then applies the [data processing inequality for relative entropy](data-processing-inequality-for-relative-entropy.md) to addition.

## ↑ Ancestors (8)

1. [Poisson distribution](poisson-distribution.md)
2. [Discrete probability distribution](discrete-probability-distribution-split.md)
3. [Probability distribution](probability-distribution.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-224/4/a/solution.md)
