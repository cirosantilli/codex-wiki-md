<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For any linear operator, the [trace norm](../../../../../../trace-norm.md) is $\|X\|_1=\operatorname{Tr}\sqrt{X^\dagger X}$, the sum of its [singular values](../../../../../../singular-value.md). For a [Hermitian operator](../../../../../../hermitian-operator.md),

$$
\boxed{\|X\|_1=\operatorname{Tr}|X|=\sum_i|\lambda_i|.}
$$

The [Holevo–Helstrom theorem](../../../../../../holevo-helstrom-theorem.md) concerns minimum-error discrimination of two [density operators](../../../../../../density-matrix.md) $\rho,\sigma$. If their prior probabilities are $p$ and $1-p$, the maximum success probability over all [measurement in quantum measurements](../../../../../../quantum-measurement-split.md) is

$$
\boxed{P_{\mathrm{succ}}^*=\frac12\left(1+\|p\rho-(1-p)\sigma\|_1\right).}
$$

An optimal binary [POVM](../../../../../../positive-operator-valued-measure.md) declares $\rho$ on the positive spectral subspace of $p\rho-(1-p)\sigma$ and declares $\sigma$ on its negative spectral subspace; zero-eigenvalue vectors can be assigned either way. For equal priors the formula becomes $P_{\mathrm{succ}}^*=\tfrac12+\tfrac14\|\rho-\sigma\|_1$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
