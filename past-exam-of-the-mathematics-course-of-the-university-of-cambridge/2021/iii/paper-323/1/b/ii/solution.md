<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The linear extension of the stated [k-reduction map](../../../../../../../k-reduction-map.md) is

$$
\Lambda_k(X)=k\operatorname{Tr}(X)I-X.
$$

It suffices to consider a pure state $|v\rangle$ of [Schmidt rank](../../../../../../../schmidt-rank.md) $r\leq k$, because positivity is preserved by sums. Write

$$
|v\rangle=\sum_{j=1}^r\sqrt{\lambda_j}|j\rangle|j\rangle,
\qquad
\rho_A=\sum_{j=1}^r\lambda_j|j\rangle\langle j|.
$$

Then

$$
(\operatorname{id}\otimes\Lambda_k)(|v\rangle\langle v|)
=k\rho_A\otimes I-|v\rangle\langle v|.
$$

For every $|x\rangle=\sum_{ij}x_{ij}|ij\rangle$, the [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md) gives

$$
|\langle v|x\rangle|^2
=\left|\sum_{j=1}^r\sqrt{\lambda_j}x_{jj}\right|^2
\leq r\sum_{j=1}^r\lambda_j|x_{jj}|^2
\leq k\langle x|\rho_A\otimes I|x\rangle.
$$

Thus the operator is a [positive semidefinite operator](../../../../../../../positive-operator.md). Applying this to every vector in a Schmidt-number-$k$ ensemble proves

$$
\boxed{\operatorname{SN}(\sigma)\leq k
\ \Longrightarrow\
(\operatorname{id}_n\otimes\Lambda_k)(\sigma)\geq0}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 323](../../../../paper-323-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
