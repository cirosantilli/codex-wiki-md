<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $n_n=c_n^\dagger c_n$ and $P_n=\prod_{m<n}(1-2n_m)$. The [Jordan–Wigner transformation](../../../../../../jordan-wigner-transformation.md) is $S_n^+=P_nc_n$, $S_n^-=P_nc_n^\dagger$ and $S_n^z=1/2-n_n$. Since $\sigma_n^x=P_n(c_n+c_n^\dagger)$, $P_{n+1}=P_n(1-2n_n)$ and $(c_n+c_n^\dagger)(1-2n_n)=c_n^\dagger-c_n$, adjacent bonds become

$$
\sigma_n^x\sigma_{n+1}^x=(c_n^\dagger-c_n)(c_{n+1}+c_{n+1}^\dagger).
$$

Thus, apart from the end bond,

$$
H=-J\sum_n(c_n^\dagger-c_n)(c_{n+1}+c_{n+1}^\dagger)+2Jg\sum_n n_n-JgN.
$$

The end bond contains the global [fermion parity](../../../../../../fermion-parity.md) and sets the sector-dependent periodic or antiperiodic fermion modes. It contributes an order-one boundary term, which is negligible for the thermodynamic energy density; it is not identically zero for the finite spin chain.

Choose the [discrete Fourier transform](../../../../../../discrete-fourier-transform.md) convention $c_n=N^{-1/2}\sum_ke^{-ikn}c_k$. Hopping gives $-2J\cos k\,c_k^\dagger c_k$. Opposite-momentum pairing gives $iJ\sin k(c_k^\dagger c_{-k}^\dagger+c_kc_{-k})$, using the [canonical anticommutation relations](../../../../../../canonical-anticommutation-relations.md) to antisymmetrize the coefficient. Therefore

$$
H=2J\sum_k(g-\cos k)c_k^\dagger c_k+iJ\sum_k\sin k(c_k^\dagger c_{-k}^\dagger+c_kc_{-k})-JgN.
$$

For the [Ising-chain Nambu spinor](../../../../../../ising-chain-nambu-spinor.md) $\Psi_k=(c_k,-ic_{-k}^\dagger)^T$, expansion of

$$
\boxed{H=J\sum_k\Psi_k^\dagger\begin{pmatrix}g-\cos k&-\sin k\\-\sin k&-(g-\cos k)\end{pmatrix}\Psi_k}
$$

recovers every term: the diagonal contributes $J(g-\cos k)(n_k+n_{-k}-1)$, and the two off-diagonal entries supply the pairing. Since $\sum_k\cos k=0$, the constant is $-JgN$. Reversing the Fourier sign changes the pairing convention; the specified sign makes the displayed matrix agree directly.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
