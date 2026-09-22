<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a [density matrix](../../../../../density-matrix.md) $\rho$ on a $d$-dimensional [Hilbert space](../../../../../hilbert-space-split.md), its [Von Neumann entropy](../../../../../von-neumann-entropy-split.md), in bits, is

$$
S(\rho)=-\operatorname{Tr}(\rho\log_2\rho)=-\sum_{a=1}^d\lambda_a\log_2\lambda_a,
$$

where the $\lambda_a$ are its eigenvalues and $0\log_20=0$. Each summand is nonnegative, proving $S\geq0$, with equality exactly when one eigenvalue is one and the rest zero, namely for a [pure state](../../../../../pure-state.md).

We first prove the [nonnegativity of quantum relative entropy](../../../../../nonnegativity-of-quantum-relative-entropy.md) needed below. Diagonalize $\rho$ with eigenvalues $\lambda_a$ and eigenvectors $u_a$, and $\sigma$ with eigenvalues $\mu_b$ and eigenvectors $v_b$. Put $B_{ab}=|\langle u_a,v_b\rangle|^2$ and $q_a=\langle u_a|\sigma|u_a\rangle=\sum_bB_{ab}\mu_b$. Each row of $B$ sums to one. Concavity of the ordinary logarithm gives $\sum_bB_{ab}\log_2\mu_b\leq\log_2q_a$. Consequently

$$
D(\rho\|\sigma)=\operatorname{Tr}\rho(\log_2\rho-\log_2\sigma)
\geq\sum_a\lambda_a\log_2\frac{\lambda_a}{q_a}\geq0.
$$

The final [Gibbs inequality](../../../../../gibbs-inequality.md) follows directly from $\sum_{\lambda_a>0}\lambda_a\log(q_a/\lambda_a)\leq\log\sum_{\lambda_a>0}q_a\leq0$. Support failure gives $D=+\infty$; zero eigenvalues can otherwise be handled by restriction or regularization. Equality requires $q_a=\lambda_a$ and equality in the logarithm inequality on every positive-weight row. Thus $u_a$ is a $\sigma$ eigenvector of eigenvalue $\lambda_a$ wherever $\lambda_a>0$. The remaining diagonal entries of $\sigma$ vanish and positivity makes the remaining rows and columns zero. Hence equality holds exactly when $\rho=\sigma$.

Taking $\sigma=I/d$ gives $D(\rho\|I/d)=\log_2d-S(\rho)$, proving

$$
\boxed{0\leq S(\rho)\leq\log_2d.}
$$

The lower equality is attained exactly by pure states and the upper exactly by the [maximally mixed state](../../../../../maximally-mixed-state.md) $I/d$.

For $\bar\rho=\sum_ip_i\rho_i$, each positive-weight state has support contained in that of $\bar\rho$. Expanding the [quantum relative entropy](../../../../../quantum-relative-entropy.md) gives

$$
S(\bar\rho)-\sum_ip_iS(\rho_i)=\sum_ip_iD(\rho_i\|\bar\rho)\geq0.
$$

This proves [Concavity of Von Neumann entropy](../../../../../concavity-of-von-neumann-entropy.md), with equality precisely when every positive-weight $\rho_i$ is the same state.

For the upper [entropy bound for a quantum mixture](../../../../../entropy-bounds-for-a-quantum-mixture.md), diagonalize each component, $\rho_i=\sum_a\lambda_{ia}|v_{ia}\rangle\langle v_{ia}|$, and set $q_{ia}=p_i\lambda_{ia}$. Form the rectangular matrix $B$ whose columns are $\sqrt{q_{ia}}\,v_{ia}$. Then $BB^\dagger=\bar\rho$, while the [Gram matrix](../../../../../gram-matrix.md) $\Gamma=B^\dagger B$ has diagonal $q_{ia}$. The two matrices have the same nonzero eigenvalues: $B$ and $B^\dagger$ map corresponding positive-eigenvalue eigenspaces isomorphically. Thus $S(\Gamma)=S(\bar\rho)$.

If there are $L$ columns, let $W=\operatorname{diag}(1,\omega,\ldots,\omega^{L-1})$, with $\omega=e^{2\pi i/L}$. Then

$$
\operatorname{diag}(\Gamma)=\frac1L\sum_{r=0}^{L-1}W^r\Gamma W^{-r}.
$$

All the summands have the same [Von Neumann entropy](../../../../../von-neumann-entropy-split.md). The just-proved concavity therefore implies $S(\bar\rho)=S(\Gamma)\leq S(\operatorname{diag}\Gamma)=H(q)$. Finally,

$$
H(q)=-\sum_{i,a}p_i\lambda_{ia}\log_2(p_i\lambda_{ia})
=H(p)+\sum_ip_iS(\rho_i).
$$

We have proved both requested bounds:

$$
\boxed{\sum_ip_iS(\rho_i)\leq S(\bar\rho)\leq\sum_ip_iS(\rho_i)-\sum_ip_i\log_2p_i.}
$$

For the upper equality, strictness in the concavity argument forces $\Gamma$ to be diagonal. Its entries between two positive-weight component eigenvectors then force those vectors to be orthogonal. Thus upper equality holds exactly when the supports of the positive-weight component states are mutually orthogonal. In that case their classical label is perfectly distinguishable, explaining the extra $H(p)$ bits.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
