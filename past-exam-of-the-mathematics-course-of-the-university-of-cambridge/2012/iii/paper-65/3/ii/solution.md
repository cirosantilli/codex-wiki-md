<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [quantum relative entropy](../../../../../../quantum-relative-entropy.md) is $S(\rho\|\sigma)=\operatorname{Tr}\rho(\log_2\rho-\log_2\sigma)$ when the [support of a positive operator](../../../../../../support-of-a-positive-operator.md) $\rho$ is contained in that of $\sigma$, and $+\infty$ otherwise. Write spectral decompositions $\rho=\sum_i r_i|i\rangle\langle i|$ and $\sigma=\sum_j t_j|u_j\rangle\langle u_j|$, and set $q_i=\langle i|\sigma|i\rangle$.

The weights $w_{ij}=|\langle i|u_j\rangle|^2$ sum to one. Concavity of the scalar logarithm gives the [diagonal logarithm concavity bound](../../../../../../diagonal-logarithm-concavity-bound.md)

$$
\langle i|\log_2\sigma|i\rangle
=\sum_jw_{ij}\log_2t_j
\leq\log_2\left(\sum_jw_{ij}t_j\right)=\log_2q_i.
$$

For $r_i>0$, support inclusion removes overlaps with zero eigenvalues of $\sigma$; alternatively take a positive regularization and pass to the limit. The two diagonal vectors $r$ and $q$ are probability distributions. Therefore

$$
\boxed{S(\rho\|\sigma)\geq\sum_i r_i\log_2\frac{r_i}{q_i}
=D(r\|q)\geq0.}
$$

This proves [nonnegativity of quantum relative entropy](../../../../../../nonnegativity-of-quantum-relative-entropy.md) without assuming the states commute. Equality in the strict logarithmic concavity condition makes each occupied $|i\rangle$ an eigenvector of $\sigma$; classical equality gives $q_i=r_i$ and no weight outside the support, hence equality occurs exactly for $\rho=\sigma$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
