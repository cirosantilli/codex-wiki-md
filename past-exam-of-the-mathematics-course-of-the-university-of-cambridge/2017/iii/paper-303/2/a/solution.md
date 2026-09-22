<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take the couplings in the [Hamiltonian](../../../../../../hamiltonian.md) to include [inverse temperature](../../../../../../inverse-temperature.md), so the [Boltzmann factor](../../../../../../boltzmann-factor.md) is $e^{-H}$. If physical energies are used instead, first replace $J,L,D,K$ by their products with $1/(k_BT)$. Split the on-site term equally between its two bonds. For spin states $s,t\in\{1,0,-1\}$ the [spin-chain transfer matrix](../../../../../../transfer-matrix-for-a-classical-spin-chain.md) has entries

$$
W_{st}=\exp\left[Jst+Ls^2t^2+\frac D2(s^2+t^2)+K\right].
$$

Using the specified coupling coordinates, in the order $(1,0,-1)$ this is

$$
\boxed{W=\frac{e^K}{z}\begin{pmatrix}1&x&y\\x&z&x\\y&x&1\end{pmatrix}.}
$$

For example, $e^{D/2}=x/z$ and $e^{-J+L+D}=y/z$. This is the nearest-neighbour [Blume–Emery–Griffiths model](../../../../../../blume-emery-griffiths-model.md) with an additive constant and the paper's sign convention for $D$.

Summing the periodic spin chain gives the [partition function](../../../../../../canonical-partition-function.md) $Z_N=\operatorname{tr}W^N=\sum_{a=1}^3\lambda_a^N$. For finite real couplings all entries of $W$ are strictly positive; the [Perron–Frobenius theorem](../../../../../../perron-frobenius-theorem.md) gives a unique positive [dominant eigenvalue](../../../../../../dominant-eigenvalue.md) with $\lambda_1>|\lambda_a|$ for $a\ne1$. Since $W$ is a [symmetric matrix](../../../../../../symmetric-matrix.md), all its [eigenvalues](../../../../../../eigenvalue.md) are real. Thus in the [thermodynamic limit](../../../../../../thermodynamic-limit.md),

$$
\boxed{\frac{F_N}{Nk_BT}\longrightarrow-\log\lambda_1.}
$$

The positivity condition is stronger and more useful than mere ordering by signed value: subdominant [eigenvalues](../../../../../../eigenvalue.md) can be negative. Also, the printed strict ordering between the other two is not guaranteed for all couplings. For instance, $J=L=D=0$ makes $W$ the positive constant [matrix](../../../../../../matrix.md) $e^K\mathbf1\mathbf1^T$ with two equal zero [eigenvalues](../../../../../../eigenvalue.md). Degeneracy there does not affect the largest-eigenvalue limit; no explicit generic [eigenvalues](../../../../../../eigenvalue.md) are needed.

For [spin magnetization](../../../../../../spin-magnetization.md), introduce a dimensionless field $h$ through $-h\sum_i\sigma_i$, or insert $S=\operatorname{diag}(1,0,-1)$ into the [trace](../../../../../../matrix-trace.md). Then

$$
\langle\sigma_i\rangle=\frac{\operatorname{tr}(SW^N)}{\operatorname{tr}W^N}\longrightarrow v_1^TSv_1=\left.\partial_h\log\lambda_1(h)\right|_{h=0},
$$

where $v_1$ is a normalized [eigenvector](../../../../../../eigenvector.md) of the largest [eigenvalue](../../../../../../eigenvalue.md) and $W_{st}(h)=e^{h(s+t)/2}W_{st}(0)$. [Spin inversion symmetry](../../../../../../spin-inversion-symmetry.md) gives $v_{1,+}=v_{1,-}$, since the positive [eigenvector](../../../../../../eigenvector.md) of the largest [eigenvalue](../../../../../../eigenvalue.md) is unique. Therefore

$$
\boxed{\langle\sigma_i\rangle=0}
$$

at zero field, both at finite $N$ and in the finite-coupling [thermodynamic limit](../../../../../../thermodynamic-limit.md). The finite-$N$ result follows directly by pairing each configuration with its spin-reversed partner. [Eigenvalues](../../../../../../eigenvalue.md) at a single fixed field do not determine a general observable: a field derivative of the largest [eigenvalue](../../../../../../eigenvalue.md), or its [eigenvector](../../../../../../eigenvector.md), is required. Positivity and the [real analytic](../../../../../../real-analytic-function.md) dependence on the couplings exclude a finite-temperature [spontaneous symmetry breaking](../../../../../../spontaneous-symmetry-breaking.md) transition in this one-dimensional finite-range chain; singular zero-temperature coupling limits require separate treatment.

For even $N$, [spin decimation](../../../../../../spin-decimation.md) on alternate sites sums the middle spin of each two-bond segment, hence the coarse [spin-chain transfer matrix](../../../../../../transfer-matrix-for-a-classical-spin-chain.md) is $W'=W^2$. Define

$$
A=1+x^2+y^2,\qquad B=x(1+y+z),\qquad C=x^2+2y,\qquad E=z^2+2x^2.
$$

Direct multiplication gives $W^2=e^{2K}z^{-2}\begin{pmatrix}A&B&C\\B&E&B\\C&B&A\end{pmatrix}$. Matching its entry ratios to the original parameterization yields the [spin-1 chain decimation recursion](../../../../../../spin-1-chain-decimation-recursion.md)

$$
\boxed{x'=\frac{x(1+y+z)}{1+x^2+y^2},\qquad y'=\frac{x^2+2y}{1+x^2+y^2},\qquad z'=\frac{z^2+2x^2}{1+x^2+y^2}.}
$$

The remaining overall positive factor is absorbed into $K'$. Keeping that factor preserves the [free energy](../../../../../../thermodynamic-free-energy.md) as well as normalized spin [probabilities](../../../../../../probability.md). Indeed $\operatorname{tr}(W^2)^{N/2}=\operatorname{tr}W^N$, exactly; on an odd ring an unmatched boundary segment needs separate handling rather than assuming a uniform two-site block decomposition.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 303](../../../paper-303-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
