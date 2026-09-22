<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Schmidt decomposition](../../../../../schmidt-decomposition.md) and [local unitary operations](../../../../../local-unitary-operation.md) put any entangled two-[qubit](../../../../../qubit.md) [pure state](../../../../../pure-state.md) into

$$
|\psi\rangle=\sqrt\lambda\,|00\rangle+\sqrt{1-\lambda}\,|11\rangle,
\qquad \frac12\leq\lambda<1.
$$

Both [Schmidt coefficients](../../../../../schmidt-coefficient.md) are nonzero. Alice performs a two-outcome [generalized measurement](../../../../../generalized-measurement-postulate.md) with [Kraus operators](../../../../../kraus-operator.md)

$$
K_s=\begin{pmatrix}\sqrt{(1-\lambda)/\lambda}&0\\0&1\end{pmatrix},
\qquad
K_f=\begin{pmatrix}\sqrt{(2\lambda-1)/\lambda}&0\\0&0\end{pmatrix}.
$$

Their effects sum to the identity, so this is a legitimate local [measurement in quantum mechanics](../../../../../quantum-measurement-split.md). On success,

$$
(K_s\otimes I)|\psi\rangle=\sqrt{1-\lambda}(|00\rangle+|11\rangle),
\qquad
\boxed{p_s=2(1-\lambda)>0.}
$$

The normalized output is the [Bell state](../../../../../bell-state-split.md) $\Phi_+$. Bob's [unitary matrix](../../../../../unitary-matrix.md) $\begin{pmatrix}0&-1\\1&0\end{pmatrix}$ maps it to the [spin singlet state](../../../../../spin-singlet-state.md). Alice communicates her success flag; no shared quantum operation is needed. At $\lambda=1/2$ the filter is the identity and success is certain. This is the singlet target case of [optimal stochastic conversion of a two-qubit pure state](../../../../../optimal-stochastic-conversion-of-a-two-qubit-pure-state.md).

For dichotomic local outcomes $A_x,B_y\in\{-1,1\}$, the [CHSH inequality](../../../../../chsh-inequality.md) is

$$
\boxed{|E_{00}+E_{01}+E_{10}-E_{11}|\leq2,\qquad
E_{xy}=\mathbb E[A_xB_y].}
$$

It assumes a [local hidden-variable theory](../../../../../local-hidden-variable-theory.md) with freely chosen settings independent of the hidden-variable distribution. For the [spin singlet state](../../../../../spin-singlet-state.md), direct evaluation of its [Pauli matrices](../../../../../pauli-matrices.md) correlations gives

$$
\langle\sigma_i\otimes\sigma_j\rangle=-\delta_{ij},\qquad
E(a,b)=-a\cdot b.
$$

Choose $a_0=e_z$, $a_1=e_x$, $b_0=(e_z+e_x)/\sqrt2$, and $b_1=(e_z-e_x)/\sqrt2$. The four correlations are $-1/\sqrt2,-1/\sqrt2,-1/\sqrt2,+1/\sqrt2$, respectively, giving

$$
\boxed{|E_{00}+E_{01}+E_{10}-E_{11}|=2\sqrt2>2.}
$$

The success flag must be recorded and communicated before the subsequent independent choice of Bell-test settings. This conditioning is legitimate because [setting-independent heralding preserves Bell locality](../../../../../setting-independent-heralding-preserves-bell-locality.md): a putative [local hidden-variable theory](../../../../../local-hidden-variable-theory.md) for the entire sequential experiment would, after successful filtering, still have local response functions with a setting-independent conditional hidden-variable distribution. More explicitly, if the hidden variable is $\xi$ and $h$ is the already determined success flag, conditioning changes its distribution to $\rho(\xi\mid h=1)$ but leaves

$$
P(A,B\mid x,y,h=1)=\int \rho(\xi\mid h=1)
P_A(A\mid x,\xi,h=1)P_B(B\mid y,\xi,h=1)\,d\xi.
$$

Classical messages used in preparation can be included in $\xi$; none are exchanged during the spacelike Bell measurements. Such a conditioned model still obeys the [CHSH inequality](../../../../../chsh-inequality.md), contradicting the displayed singlet correlations. Therefore **no [local hidden-variable theory](../../../../../local-hidden-variable-theory.md) reproduces all sequential measurement correlations of any entangled two-[qubit](../../../../../qubit.md) [pure state](../../../../../pure-state.md)**. This argument does not discard outcomes on the basis of the later measurement settings.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 61](../../paper-61-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
