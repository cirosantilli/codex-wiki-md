<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $p_i=\langle\psi_i|\rho|\psi_i\rangle$. The [rank-one dephasing](../../../../../../rank-one-dephasing.md) is $\rho'=\sum_ip_i|\psi_i\rangle\langle\psi_i|$. If $p_i=0$, positivity gives

$$
0=p_i=\|\sqrt\rho\,|\psi_i\rangle\|^2,
$$

so $\rho|\psi_i\rangle=0$. The kernel of $\rho'$ is exactly the span of these zero-probability basis vectors and is therefore contained in the kernel of $\rho$. Taking orthogonal complements proves [support inclusion under rank-one dephasing](../../../../../../support-inclusion-under-rank-one-dephasing.md):

$$
\boxed{\operatorname{supp}\rho\subseteq\operatorname{supp}\rho'.}
$$

Here the [support of a positive operator](../../../../../../support-of-a-positive-operator.md) is the orthogonal complement of its kernel.

On that support, $\log_2\rho'$ is diagonal in the measurement basis, giving

$$
\operatorname{Tr}(\rho\log_2\rho')=\sum_{i:p_i>0}p_i\log_2p_i=\operatorname{Tr}(\rho'\log_2\rho').
$$

Consequently the [relative-entropy identity for rank-one dephasing](../../../../../../relative-entropy-identity-for-rank-one-dephasing.md) is

$$
D_{\mathrm{rel}}(\rho\|\rho')=\operatorname{Tr}\bigl[\rho(\log_2\rho-\log_2\rho')\bigr]=S(\rho')-S(\rho).
$$

[Klein's inequality](../../../../../../klein-s-inequality.md) gives $D_{\mathrm{rel}}(\rho\|\rho')\geq0$, since both [density operators](../../../../../../density-matrix.md) have trace one. For singular $\rho$, first restrict to $\operatorname{supp}\rho'$ where $\rho'$ is positive definite, replace $\rho$ by $(\rho+\eta I)/(1+\eta\dim\operatorname{supp}\rho')$, and let $\eta\downarrow0$. The support inclusion ensures that the limit is finite. Thus

$$
\boxed{S(\rho')\geq S(\rho).}
$$

This proves [entropy increase under nonselective projective measurement](../../../../../../entropy-increase-under-nonselective-projective-measurement.md) using [Klein's inequality](../../../../../../klein-s-inequality.md). Equality holds exactly when $\rho=\rho'$, so the original [density operator](../../../../../../density-matrix.md) was already diagonal in the chosen basis.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
