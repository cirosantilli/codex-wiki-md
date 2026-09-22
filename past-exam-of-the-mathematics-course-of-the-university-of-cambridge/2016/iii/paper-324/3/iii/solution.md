<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $|a\rangle=\bigotimes_j|a_j\rangle$. Instead of storing the output vector, use [Heisenberg propagation of a Pauli observable through a Clifford circuit](../../../../../../heisenberg-propagation-of-a-pauli-observable-through-a-clifford-circuit.md):

$$
\langle Z_1\rangle_{\rm out}=\langle a|C^\dagger Z_1C|a\rangle.
$$

Initialize the compact [Pauli group](../../../../../../pauli-group.md) representation at $Z_1$ and conjugate successively by $U_N,U_{N-1},\ldots,U_1$, in that order, using $P\mapsto U_j^\dagger P U_j$. This gives

$$
P=C^\dagger Z_1C=U_1^\dagger\cdots U_N^\dagger Z_1U_N\cdots U_1
$$

with $O(N+n)$ local-update work and $O(n)$ storage. The resulting [Pauli operator](../../../../../../pauli-operator.md) is Hermitian, so we can express it as $P=\eta\bigotimes_j\sigma_j$, where $\eta\in\{+1,-1\}$ and each $\sigma_j$ is $I,X,Y$ or $Z$. Any factors $XZ$ in the representation from part (i) are converted using $XZ=-iY$, with their phases absorbed into $\eta$.

The [product state](../../../../../../product-state.md) input now makes the expectation factorize:

$$
\boxed{e=\langle a|P|a\rangle=\eta\prod_{j=1}^n\langle a_j|\sigma_j|a_j\rangle,\qquad
p_0=\frac{1+e}{2},\quad p_1=\frac{1-e}{2}.}
$$

Each factor is a two-by-two matrix calculation. More explicitly, for $|a_j\rangle=\alpha_j|0\rangle+\beta_j|1\rangle$, the three nontrivial expectations are $2\operatorname{Re}(\overline\alpha_j\beta_j)$, $2\operatorname{Im}(\overline\alpha_j\beta_j)$, and $|\alpha_j|^2-|\beta_j|^2$ for $X,Y,Z$, respectively.

Thus **this single-output process has a [strong classical simulation](../../../../../../strong-classical-simulation-of-a-quantum-circuit.md) in [polynomial time](../../../../../../polynomial-time.md)**, even when the individual input states are not stabilizer states. As usual, the given state identities must provide efficiently computable amplitudes. With finite-precision inputs, each factor can be evaluated to error $\delta/n$ and its approximation clipped to $[-1,1]$ to obtain the final expectation to error at most $\delta$, because all factors lie in $[-1,1]$. The required extra precision is only $O(\log(n/\delta))$ bits. Exact evaluation applies when the input descriptions support exact arithmetic. This avoids silently assigning a finite exact-computation cost to arbitrary unspecified real numbers.

Once the probabilities are known, a classical randomized computation can reproduce this measured bit. The argument concerns the specified one-[qubit](../../../../../../qubit.md) output; it does not assert that every joint measurement distribution for arbitrary product inputs can be simulated by this same single-observable calculation.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
