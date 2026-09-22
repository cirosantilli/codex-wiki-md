<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The printed normalization has its factors reversed. For the displayed map $\Phi(X)=\sum_kA_kXA_k^\dagger$, the condition $\sum_kA_kA_k^\dagger=I$ says $\Phi(I)=I$, which is unitality. Trace preservation instead requires

$$
\boxed{\sum_kA_k^\dagger A_k=I.}
$$

These are distinct [trace-preserving and unital Kraus conditions](../../../../../trace-preserving-and-unital-kraus-conditions.md). To disprove the printed equivalence, take $0<\gamma<1$ and

$$
B_0=\begin{pmatrix}1&0\\0&\sqrt{1-\gamma}\end{pmatrix},\qquad
B_1=\sqrt\gamma|1\rangle\langle0|.
$$

They obey $\sum_jB_jB_j^\dagger=I$, but

$$
\sum_jB_j^\dagger B_j=\operatorname{diag}(1+\gamma,1-\gamma),
\qquad
\operatorname{Tr}\!\left[\sum_jB_j|0\rangle\langle0|B_j^\dagger\right]=1+\gamma.
$$

Thus their [completely positive map](../../../../../completely-positive-map.md) is not trace preserving. They are the adjoints of the operators of an [amplitude damping channel](../../../../../amplitude-damping-channel.md). That channel is trace preserving but sends $I$ to $\operatorname{diag}(1+\gamma,1-\gamma)$, so it cannot satisfy the printed normalization in any [Kraus representation](../../../../../kraus-representation.md) either. The corrected characterization is proved next.

Work in finite-dimensional input and output [Hilbert spaces](../../../../../hilbert-space-split.md), with a linear map $\Phi$ on operators. Suppose first that $\Phi(X)=\sum_kA_kXA_k^\dagger$ and $\sum_kA_k^\dagger A_k=I$. For every auxiliary dimension $m$ and every positive operator $W$ on the extended space,

$$
(\operatorname{id}_m\otimes\Phi)(W)
=\sum_k(I_m\otimes A_k)W(I_m\otimes A_k)^\dagger\geq0.
$$

Each summand is positive because conjugation preserves positivity. This is exactly the definition of a [completely positive map](../../../../../completely-positive-map.md). Cyclicity of the trace gives

$$
\operatorname{Tr}\Phi(X)=\operatorname{Tr}\!\left[X\sum_kA_k^\dagger A_k\right]=\operatorname{Tr}X,
$$

so the map is also trace preserving.

Conversely, suppose $\Phi$ is completely positive and trace preserving, and let $|i\rangle$ be an orthonormal input basis. Use the unnormalized entangled vector $|\Omega\rangle=\sum_i|i\rangle\otimes|i\rangle$, with the reference factor first. Complete positivity makes the corresponding unnormalized [Choi matrix](../../../../../choi-matrix.md) positive:

$$
J_\Phi=(\operatorname{id}\otimes\Phi)(|\Omega\rangle\langle\Omega|)
=\sum_{i,j}|i\rangle\langle j|\otimes\Phi(|i\rangle\langle j|)\geq0.
$$

Its [spectral decomposition](../../../../../spectral-decomposition.md) can be written $J_\Phi=\sum_k|v_k\rangle\langle v_k|$, absorbing the nonnegative [eigenvalues](../../../../../eigenvalue.md) into the vectors. Define [linear operators](../../../../../linear-operator.md) $A_k$ uniquely by

$$
|v_k\rangle=\sum_i|i\rangle\otimes A_k|i\rangle.
$$

Expanding the outer products and comparing their $(i,j)$ reference blocks yields

$$
\Phi(|i\rangle\langle j|)=\sum_kA_k|i\rangle\langle j|A_k^\dagger.
$$

The matrix units span all operators, so linearity proves the [Kraus representation](../../../../../kraus-representation.md) $\Phi(X)=\sum_kA_kXA_k^\dagger$ for every $X$. Finally, trace preservation gives

$$
\operatorname{Tr}\!\left[X\left(\sum_kA_k^\dagger A_k-I\right)\right]=0
$$

for all $X$. Taking matrix units as test operators shows that the matrix in parentheses is zero. This proves both directions of the corrected CPT characterization, including the normalization rather than assuming it.

For an input [quantum state ensemble](../../../../../quantum-state-ensemble.md) $\{p_x,\rho_x\}$, write $\sigma_x=\Phi(\rho_x)$ and $\bar\sigma=\sum_xp_x\sigma_x$. Its output [Holevo quantity](../../../../../holevo-quantity.md) is

$$
\chi(\{p_x,\sigma_x\})=S(\bar\sigma)-\sum_xp_xS(\sigma_x).
$$

The [Holevo capacity](../../../../../holevo-capacity.md) is the optimized one-use quantity

$$
\boxed{\chi^*(\Phi)=\sup_{\{p_x,\rho_x\}}
\left[S\!\left(\sum_xp_x\Phi(\rho_x)\right)-\sum_xp_xS(\Phi(\rho_x))\right],}
$$

where the supremum ranges over finite input ensembles and $S$ is the [Von Neumann entropy](../../../../../von-neumann-entropy-split.md) in bits.

For $n$ uses of a [memoryless quantum channel](../../../../../memoryless-quantum-channel.md), the map is $\Phi^{\otimes n}$. An $n$-use code consists of a finite message set $\mathcal M_n$ of size $M_n$, an encoding state $\rho_m^{(n)}$ on the $n$ inputs for each message, and a decoding [POVM](../../../../../positive-operator-valued-measure.md) $\{D_m^{(n)}:m\in\mathcal M_n\}$ on the output space, with $D_m^{(n)}\geq0$ and $\sum_mD_m^{(n)}=I$. The encoding states may be entangled across uses. The measurement outcome is the receiver's decoded message, with conditional probability

$$
P(\widehat m=l\mid m)=\operatorname{Tr}\!\left[D_l^{(n)}\Phi^{\otimes n}(\rho_m^{(n)})\right].
$$

For uniformly distributed messages the average error and rate are

$$
\boxed{P_e^{(n)}=1-\frac1{M_n}\sum_m\operatorname{Tr}\!\left[D_m^{(n)}\Phi^{\otimes n}(\rho_m^{(n)})\right],\qquad
R_n=\frac1n\log_2M_n.}
$$

A rate $R$ is achievable if there is a sequence of such codes with $P_e^{(n)}\to0$ and $\liminf_nR_n\geq R$. The unassisted [classical capacity of a quantum channel](../../../../../classical-capacity-of-a-quantum-channel.md) is the supremum of achievable rates; the sender and receiver do not share prior entanglement.

The operational content of the [Holevo-Schumacher-Westmoreland theorem](../../../../../holevo-schumacher-westmoreland-theorem.md) is that $\chi^*(\Phi)$ is the capacity for product-state input encodings with collective output measurements. Allowing arbitrary entangled block inputs gives the regularized formula

$$
\boxed{C(\Phi)=\lim_{n\to\infty}\frac1n\chi^*(\Phi^{\otimes n})
=\sup_{n\geq1}\frac1n\chi^*(\Phi^{\otimes n}).}
$$

The limit equals the supremum because [superadditivity of Holevo capacity](../../../../../superadditivity-of-holevo-capacity.md) follows by taking product ensembles for two blocks and using additivity of the [Von Neumann entropy](../../../../../von-neumann-entropy-split.md) on product states. The coding theorem makes every rate below the one-block [Holevo quantity](../../../../../holevo-quantity.md) achievable through many independently encoded blocks, with collective decoding.

The converse can be seen explicitly from the [Holevo bound](../../../../../holevo-s-theorem.md) and [Fano's inequality](../../../../../fano-s-inequality.md). For a uniform transmitted message $M$ and decoded message $\widehat M$,

$$
(1-P_e^{(n)})\log_2M_n-h_2(P_e^{(n)})
\leq I(M:\widehat M)
\leq\chi\!\left(\left\{\frac1{M_n},\Phi^{\otimes n}(\rho_m^{(n)})\right\}\right)
\leq\chi^*(\Phi^{\otimes n}).
$$

The first inequality is obtained by subtracting the Fano bound on $H(M\mid\widehat M)$ from $H(M)=\log_2M_n$. Dividing by $n$ and letting the average error vanish bounds every achievable rate by the regularized expression. The block-coding achievability just described supplies the reverse bound.

Under the assumed [additivity of Holevo capacity](../../../../../additivity-of-holevo-capacity.md) across tensor powers, $\chi^*(\Phi^{\otimes n})=n\chi^*(\Phi)$ for every $n$. Thus

$$
\boxed{C(\Phi)=\chi^*(\Phi)=C_{\mathrm{product}}(\Phi).}
$$

**The stated conditional assertion is true:** under this additivity assumption, entangled input states cannot increase the asymptotic unassisted classical rate beyond the rate already achievable with product inputs. The decoder may still use collective measurements across channel outputs.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 60](../../paper-60-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
