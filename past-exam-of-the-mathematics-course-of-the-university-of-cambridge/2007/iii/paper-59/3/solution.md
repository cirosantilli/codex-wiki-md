<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Take the labels $r,s\in\{0,\ldots,n-1\}$, with basis indices read modulo $n$. There is a missing hypothesis in the printed claim: the root of unity must be primitive. For example, when $n=2$ and $\omega=1$, the two labels $(0,0)$ and $(1,0)$ produce the identical state $(|00\rangle+|11\rangle)/\sqrt2$, so they are not orthogonal. More generally, if the order of $\omega$ is $d<n$, changing $r$ to $r+d$ repeats a state. **The orthonormality claim is false for a nonprimitive root.**

For the intended result, choose a [primitive root of unity](../../../../../primitive-root-of-unity.md), for example $\omega=e^{2\pi i/n}$. Since $|\omega|=1$, expansion in the [orthonormal basis](../../../../../orthonormal-basis.md) gives

$$
\begin{aligned}
\langle\psi_{rs}|\psi_{r's'}\rangle&=\frac1n\sum_{j,k=0}^{n-1}\omega^{-jr+kr'}\langle j|k\rangle\langle j+s|k+s'\rangle\\
&=\frac{\delta_{ss'}}n\sum_{j=0}^{n-1}\omega^{j(r'-r)}.
\end{aligned}
$$

If $r=r'$, the sum is $n$. If $r\ne r'$ modulo $n$, primitiveness gives $q=\omega^{r'-r}\ne1$ while $q^n=1$, and the [finite geometric series](../../../../../finite-geometric-series.md) is $(1-q^n)/(1-q)=0$. Thus

$$
\boxed{\langle\psi_{rs}|\psi_{r's'}\rangle=\delta_{rr'}\delta_{ss'}.}
$$

There are $n^2$ vectors in an $n^2$-dimensional [Hilbert space](../../../../../hilbert-space-split.md), so they form the [generalized Bell basis](../../../../../generalized-bell-basis.md). Each has equal [Schmidt coefficients](../../../../../schmidt-coefficient.md) $1/\sqrt n$ and is a [maximally entangled state](../../../../../maximally-entangled-state.md).

For [qudit teleportation](../../../../../qudit-teleportation.md), let $C$ be Alice's unknown input, write $|\chi\rangle_C=\sum_j\alpha_j|j\rangle_C$, and let Alice and Bob share $|\Phi\rangle_{AB}=n^{-1/2}\sum_k|k\rangle_A|k\rangle_B$. Alice holds $C,A$ and Bob holds $B$. Define the [qudit shift and phase operators](../../../../../qudit-shift-and-phase-operators.md)

$$
X|j\rangle=|j+1\bmod n\rangle,\qquad Z|j\rangle=\omega^j|j\rangle.
$$

Both are unitary. Alice makes a joint [projective measurement](../../../../../projective-measurement.md) of $C,A$ in the [generalized Bell basis](../../../../../generalized-bell-basis.md), with projectors $|\psi_{rs}\rangle\langle\psi_{rs}|$. Completeness follows from the orthonormality just proved.

For outcome $(r,s)$, contracting the corresponding bra with the joint input and resource gives Bob's unnormalized state:

$$
\begin{aligned}
(\langle\psi_{rs}|_{CA}\otimes I_B)(|\chi\rangle_C\otimes|\Phi\rangle_{AB})&=\frac1n\sum_{j=0}^{n-1}\alpha_j\omega^{-jr}|j+s\rangle_B\\
&=\frac1n X^sZ^{-r}|\chi\rangle_B.
\end{aligned}
$$

The [Born rule](../../../../../born-rule.md) therefore gives $p_{rs}=1/n^2$, since $X^sZ^{-r}$ preserves the input norm. Conditional on this outcome, Bob holds $X^sZ^{-r}|\chi\rangle$. Alice sends him the classical label $(r,s)$, and he applies its inverse in the displayed order:

$$
\boxed{U_{rs}=Z^rX^{-s},\qquad U_{rs}X^sZ^{-r}|\chi\rangle=|\chi\rangle.}
$$

**The corrected receiver state is exactly the unknown input state for every outcome.** Alice needs no knowledge of the amplitudes. The label has $n^2$ possibilities and can be encoded in $\lceil\log_2(n^2)\rceil$ classical bits; when $n$ is a power of two this is exactly $2\log_2 n$. The protocol consumes the shared [maximally entangled state](../../../../../maximally-entangled-state.md) and the original carrier is measured, so it does not retain an additional copy of the unknown state.

Equivalently, the complete joint [quantum state](../../../../../quantum-state.md) has the teleportation expansion

$$
|\chi\rangle_C|\Phi\rangle_{AB}=\frac1n\sum_{r,s=0}^{n-1}|\psi_{rs}\rangle_{CA}\otimes X^sZ^{-r}|\chi\rangle_B.
$$

It follows from the contraction calculation and completeness of the [generalized Bell basis](../../../../../generalized-bell-basis.md). After correction the branch operators are all $I/n$, so their sum defines the identity [quantum channel](../../../../../quantum-channel.md): $\sum_{r,s}(I/n)\rho(I/n)=\rho$. Acting on the input part of a joint state with a reference gives the same identity, which proves [teleportation as an identity channel on a reference](../../../../../teleportation-as-an-identity-channel-on-a-reference.md) and extends the protocol to mixed inputs.

Before receiving the label, Bob instead has the outcome-averaged state

$$
\rho_B=\frac1{n^2}\sum_{r,s}X^sZ^{-r}|\chi\rangle\langle\chi|Z^rX^{-s}=\frac In.
$$

To check the equality, averaging over $r$ kills the off-diagonal matrix entries by the same root-of-unity sum; averaging the cyclic shifts $s$ makes every diagonal entry the total trace divided by $n$. This is the [Heisenberg-Weyl twirling channel](../../../../../heisenberg-weyl-twirling-channel.md). Thus the classical message is necessary to recover the input, consistently with the [no-communication theorem](../../../../../no-communication-theorem.md) derived in Question 1.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
