<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The constraints $-I\leq T\leq I$ are in the order of [Hermitian operators](../../../../../../hermitian-operator.md). They imply $-1\leq\langle\alpha_i|T|\alpha_i\rangle\leq1$. Using the [spectral decomposition](../../../../../../spectral-decomposition.md) of $X$,

$$
\operatorname{Tr}(XT)=\sum_i\lambda_i\langle\alpha_i|T|\alpha_i\rangle\leq\sum_i|\lambda_i|=\|X\|_1.
$$

Choose $T=\operatorname{sgn}(X)$, with eigenvalues $+1$ on the positive spectral subspace, $-1$ on the negative spectral subspace, and zero on the kernel. It satisfies the constraints and attains equality. The [trace-norm variational principle for Hermitian operators](../../../../../../trace-norm-variational-principle-for-hermitian-operators.md) is therefore

$$
\boxed{\|X\|_1=\max_{-I\leq T\leq I}\operatorname{Tr}(XT).}
$$

To prove the [Holevo–Helstrom theorem](../../../../../../holevo-helstrom-theorem.md), write a binary [POVM](../../../../../../positive-operator-valued-measure.md) as $\{E,I-E\}$, where $0\leq E\leq I$, and associate the first outcome with $\rho$. Any larger outcome set followed by a binary decision can be grouped into this form. Put $\Delta=p\rho-(1-p)\sigma$. Its success probability is

$$
P_{\mathrm{succ}}=p\operatorname{Tr}(\rho E)+(1-p)\operatorname{Tr}(\sigma(I-E))=(1-p)+\operatorname{Tr}(\Delta E).
$$

The substitution $T=2E-I$ bijects the allowed effects with the interval $-I\leq T\leq I$. Since $\operatorname{Tr}\Delta=2p-1$,

$$
P_{\mathrm{succ}}=\frac12+\frac12\operatorname{Tr}(\Delta T)\leq\frac12(1+\|\Delta\|_1).
$$

Choosing $E$ as the positive spectral projection of $\Delta$ attains this value, with an arbitrary decision on its kernel. **This proves the optimal success probability and constructs an optimal measurement.**

## ↑ Ancestors (11)

1. [Iii](../iii.md)
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
