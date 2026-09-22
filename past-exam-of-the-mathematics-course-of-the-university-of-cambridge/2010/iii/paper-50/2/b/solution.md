<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\rho=\sum_n r_n\sigma_n$ in the [Generalized Bloch representation](../../../../../../generalized-bloch-representation.md). Linearity of the [Lindbladian](../../../../../../lindbladian.md) gives $\dot r_m=\sum_n\operatorname{Tr}(\sigma_m\mathcal L(\sigma_n))r_n$. For the Hamiltonian term, cyclicity yields

$$
\operatorname{Tr}(\sigma_m[-iH,\sigma_n])=-i\operatorname{Tr}(H\sigma_n\sigma_m-H\sigma_m\sigma_n)=\operatorname{Tr}(iH[\sigma_m,\sigma_n])=L_{mn}.
$$

For one [Lindblad operator](../../../../../../lindblad-operator.md) $V_d$, the jump term becomes $\operatorname{Tr}(\sigma_mV_d\sigma_nV_d^\dagger)=\operatorname{Tr}(V_d^\dagger\sigma_mV_d\sigma_n)$, and the two remaining terms give

$$
\operatorname{Tr}(\sigma_mV_d^\dagger V_d\sigma_n)+\operatorname{Tr}(\sigma_m\sigma_nV_d^\dagger V_d)=\operatorname{Tr}(V_d^\dagger V_d\{\sigma_m,\sigma_n\}).
$$

Thus

$$
\boxed{D^{(d)}_{mn}=\operatorname{Tr}(V_d^\dagger\sigma_mV_d\sigma_n)-\frac12\operatorname{Tr}(V_d^\dagger V_d\{\sigma_m,\sigma_n\}),\qquad \dot r=\left(L+\sum_dD^{(d)}\right)r}.
$$

Every coefficient is real because $\mathcal L(\sigma_n)$ is Hermitian. In addition, $L_{mn}=-L_{nm}$, although a dissipative $D^{(d)}$ need not be symmetric.

The Hamiltonian [commutator](../../../../../../commutator.md) has zero [trace](../../../../../../matrix-trace.md), and each dissipator obeys $\operatorname{Tr}(V\rho V^\dagger)=\operatorname{Tr}(V^\dagger V\rho)$, so $\operatorname{Tr}\mathcal L(\rho)=0$. Consequently $\boxed{\dot r_{N^2}=0,\qquad r_{N^2}=1/\sqrt N}$ for normalized [density operators](../../../../../../density-matrix.md). Orthogonality to $I/\sqrt N$ makes every other $\sigma_k$ traceless. Define $s=(r_1,\ldots,r_{N^2-1})^T$. With $M=L+\sum_dD^{(d)}$, [trace](../../../../../../matrix-trace.md) preservation gives the block form

$$
M=\begin{pmatrix}A&b\\0&0\end{pmatrix},\qquad \boxed{\dot s=As+c,\quad A_{mn}=M_{mn},\quad c_m=M_{m,N^2}/\sqrt N}.
$$

Here the indices of $A$ range from $1$ to $N^2-1$. Since $\mathcal L(I)=\sum_d(V_dV_d^\dagger-V_d^\dagger V_d)$, the offset can also be written $c_m=N^{-1}\operatorname{Tr}(\sigma_m\sum_d[V_d,V_d^\dagger])$. This is the [Affine Bloch equation](../../../../../../affine-bloch-equation.md); its offset is zero for unital dynamics, which preserve the identity.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
