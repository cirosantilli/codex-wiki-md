<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $\mathcal G=-i[H,\cdot]+\sum_d\mathcal D[V_d]$ denote the [Lindbladian](../../../../../../lindbladian.md). Substituting $\rho=\sum_n r_n\sigma_n$ and projecting with the [Hilbert-Schmidt inner product](../../../../../../hilbert-schmidt-inner-product.md) gives

$$
\dot r_m=\sum_n\operatorname{Tr}[\sigma_m\mathcal G(\sigma_n)]r_n.
$$

For the [Quantum Hamiltonian](../../../../../../hamiltonian-quantum-mechanics.md) term, cyclicity of the [trace](../../../../../../matrix-trace.md) yields

$$
\begin{aligned}
\operatorname{Tr}(\sigma_m[-iH,\sigma_n])
&=-i\operatorname{Tr}(\sigma_mH\sigma_n-\sigma_m\sigma_nH)\\
&=i\operatorname{Tr}[H(\sigma_m\sigma_n-\sigma_n\sigma_m)]
=L_{mn}.
\end{aligned}
$$

For each [Lindblad dissipator](../../../../../../lindblad-dissipator.md), the same cyclic rearrangement gives

$$
\begin{aligned}
\operatorname{Tr}[\sigma_m\mathcal D[V_d](\sigma_n)]
&=\operatorname{Tr}(V_d^\dagger\sigma_mV_d\sigma_n)\\
&\quad-\frac12\operatorname{Tr}[V_d^\dagger V_d(\sigma_n\sigma_m+\sigma_m\sigma_n)]
=D_{mn}^{(d)}.
\end{aligned}
$$

These are the required coefficient matrices, so $\dot r=(L+\sum_dD^{(d)})r$. They are real because both generators map [Hermitian matrices](../../../../../../hermitian-operator.md) to [Hermitian matrices](../../../../../../hermitian-operator.md), whose coordinates are real by (a).

The [trace](../../../../../../matrix-trace.md) of a [commutator](../../../../../../commutator.md) vanishes. Also

$$
\operatorname{Tr}[\mathcal D[V](\rho)]
=\operatorname{Tr}(V^\dagger V\rho)
-\tfrac12\operatorname{Tr}(V^\dagger V\rho+\rho V^\dagger V)=0.
$$

Thus the last row of $L+\sum_dD^{(d)}$ is zero and $\boxed{\dot r_{N^2}=0}$. It is [trace](../../../../../../matrix-trace.md) preservation, not preservation of the [purity of a density operator](../../../../../../purity-of-a-density-operator.md), that produces this constant coordinate.

Write $G=L+\sum_dD^{(d)}$ and $n=N^2-1$. Since $r_{N^2}=1/\sqrt N$, the remaining coordinates obey the [Affine Bloch equation](../../../../../../affine-bloch-equation.md)

$$
\boxed{\dot s=As+c,\qquad A_{mn}=G_{mn},\quad
c_m=G_{m,N^2}/\sqrt N\quad(1\leq m,n\leq n).}
$$

Because $[H,I]=0$ and $\mathcal D[V](I)=[V,V^\dagger]$, its offset can also be written

$$
c_m=\frac1N\operatorname{Tr}\left[\sigma_m\sum_d[V_d,V_d^\dagger]\right].
$$

It vanishes for unital dynamics, but need not vanish for a general dissipative evolution.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
