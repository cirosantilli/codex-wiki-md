<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Introduce an orthonormal classical-label basis $|i\rangle$ and the [classical-quantum state](../../../../../../classical-quantum-state.md)

$$
\Gamma_{XA}=\sum_ip_i|i\rangle\langle i|\otimes\rho_i.
$$

Its [reduced density operators](../../../../../../reduced-density-matrix.md) are $\Gamma_X=\sum_ip_i|i\rangle\langle i|$ and $\Gamma_A=\overline\rho=\sum_ip_i\rho_i$. If $\lambda_{ij}$ are the eigenvalues of $\rho_i$, the eigenvalues of $\Gamma_{XA}$ are $p_i\lambda_{ij}$. Thus the [entropy of an orthogonal quantum mixture](../../../../../../entropy-of-an-orthogonal-quantum-mixture.md) is

$$
S(\Gamma_{XA})=H(p)+\sum_ip_iS(\rho_i),\qquad S(\Gamma_X)=H(p),
$$

where $H(p)=-\sum_ip_i\log_2p_i$ is the [Shannon entropy](../../../../../../information-entropy.md). Apply the proved [Subadditivity of Von Neumann entropy](../../../../../../subadditivity-of-von-neumann-entropy.md) to $X$ and $A$ and cancel $H(p)$. This gives [Concavity of Von Neumann entropy](../../../../../../concavity-of-von-neumann-entropy.md):

$$
\boxed{S\left(\sum_ip_i\rho_i\right)\geq\sum_ip_iS(\rho_i).}
$$

Zero-probability terms may simply be omitted. The equality condition from the preceding solution implies that equality holds precisely when all the positive-probability states are the same: the block equations $p_i\rho_i=p_i\overline\rho$ follow from $\Gamma_{XA}=\Gamma_X\otimes\Gamma_A$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
