<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write both the input and output integer labels in most-significant-bit-first order, $x=\sum_{j=1}^n x_j2^{n-j}$ and $y=\sum_{j=1}^n y_j2^{n-j}$. Factoring the Fourier phase over the bits of $y$ gives the [product decomposition of a Fourier phase state](../../../../../product-decomposition-of-a-fourier-phase-state.md):

$$
\operatorname{QFT}_{2^n}|x\rangle
=\bigotimes_{j=1}^n\frac{|0\rangle+e^{2\pi ix/2^j}|1\rangle}{\sqrt2}
=\bigotimes_{j=1}^n\frac{|0\rangle+e^{2\pi i\,0.x_{n-j+1}\cdots x_n}|1\rangle}{\sqrt2}.
$$

Here $0.x_l\cdots x_n$ denotes the binary fraction $\sum_{r=l}^n x_r/2^{r-l+1}$; the integer part of $x/2^j$ does not affect the phase.

Build a [dyadic quantum Fourier transform circuit](../../../../../dyadic-quantum-fourier-transform-circuit.md) as follows. Process wires $j=1,\ldots,n$ in that order. First apply a [Hadamard gate](../../../../../hadamard-gate.md) to wire $j$. Then, for each $l=j+1,\ldots,n$, apply the [controlled phase gate](../../../../../controlled-phase-gate.md) $R_{l-j+1}$ with control wire $l$ and target wire $j$. On a [computational-basis state](../../../../../computational-basis-state.md), every unprocessed control is still the bit $x_l$, so wire $j$ becomes

$$
\frac{|0\rangle+(-1)^{x_j}\prod_{l=j+1}^n e^{2\pi ix_l/2^{l-j+1}}|1\rangle}{\sqrt2}
=\frac{|0\rangle+e^{2\pi i\,0.x_j\cdots x_n}|1\rangle}{\sqrt2}.
$$

Once a wire has been processed it is not touched by later stages. Reversing the order of the output wires gives exactly the Fourier product above. Agreement on every [computational-basis state](../../../../../computational-basis-state.md) proves agreement as [linear operators](../../../../../linear-operator.md) on all superpositions, even though the intermediate operation on a general input can create [entanglement](../../../../../entangled-state.md).

There are $n$ [Hadamard gates](../../../../../hadamard-gate.md) and $n(n-1)/2$ [controlled phase gates](../../../../../controlled-phase-gate.md). Output reversal may be treated as wire relabelling. If it must instead be implemented physically while using only the requested gate family, use $\lfloor n/2\rfloor$ [swap operators](../../../../../swap-operator.md). Each swap is three [controlled-NOT gates](../../../../../controlled-not-gate.md), and

$$
\operatorname{CNOT}_{a\to b}=H_b\,\operatorname{controlled}\!R_1(a,b)\,H_b,
\qquad R_1=Z.
$$

Thus the swaps use only [Hadamard gates](../../../../../hadamard-gate.md) and [Controlled-Z gates](../../../../../controlled-z-gate.md), which are controlled $R_1$ gates. An exact physical network has

$$
g_n=\frac{n(n+1)}2+9\lfloor n/2\rfloor=O(n^2)
$$

elementary gates from the stated family. **This implements the positive-exponent Fourier transform with the correct output order in quadratic size.** Omitting the output reversal without relabelling the wires would produce the reversed-order transform instead.

For the perturbation bound, the [operator norm](../../../../../operator-norm.md) in the source is equivalently $\|A\|=\sup_{\|\psi\|=1}\|A\psi\|$. It satisfies the [triangle inequality](../../../../../triangle-inequality.md), is unchanged by left or right multiplication by a [unitary operator](../../../../../unitary-operator.md), and a [unitary operator](../../../../../unitary-operator.md) has norm one. The exact telescoping identity is

$$
U_1\cdots U_m-V_1\cdots V_m
=\sum_{j=1}^m U_1\cdots U_{j-1}(U_j-V_j)V_{j+1}\cdots V_m.
$$

It follows by replacing one factor at a time; alternatively all intermediate products cancel in the sum. Taking the [operator norm](../../../../../operator-norm.md) and using unitary invariance gives the [quantum circuit gate-error telescoping bound](../../../../../quantum-circuit-gate-error-telescoping-bound.md)

$$
\|U_1\cdots U_m-V_1\cdots V_m\|
\le\sum_{j=1}^m\|U_j-V_j\|<m\epsilon.
$$

The original PDF assumes strict $\|U_j-V_j\|<\epsilon$, so its strict conclusion is justified. If the hypothesis were weakened to a non-strict inequality, the conclusion would likewise be $\le m\epsilon$. The TeX aid misreads this hypothesis; the PDF resolves it.

Apply the non-strict version to each approximate unitary gate in the Fourier network. Extending a gate by the identity on other wires leaves its [operator norm](../../../../../operator-norm.md) error unchanged. Including the physical swap decompositions, all gates are of the required type and can obey the stated accuracy. Hence

$$
\boxed{\|U_n-\operatorname{QFT}_{2^n}\|\le\frac{g_n}{n^4}
=\frac{n(n+1)/2+9\lfloor n/2\rfloor}{n^4}
=O(n^{-2}).}
$$

With exact output relabelling rather than physical swaps the numerator is just $n(n+1)/2$. The proof retains gate phases and makes no assumption of cancellation between coherent errors.

For every normalized input the output-state [norm](../../../../../norm.md) error is at most this same bound. If $M$ is any [positive operator](../../../../../positive-operator.md) satisfying $0\le M\le I$, the change in its [measurement in quantum mechanics](../../../../../quantum-measurement-split.md) outcome probability is at most $2\delta$, where $\delta=\|U_n-\operatorname{QFT}_{2^n}\|$: expand the difference of the two expectations into two terms, each bounded by $\delta$ using the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md). Thus **inverse-polynomial gate accuracy gives an inverse-polynomial total error**, rather than requiring exponential precision in the number of qubits. For the [phase gates](../../../../../phase-gate.md) this corresponds to specifying angles with $O(\log n)$ bits of precision, since $|e^{i\theta}-e^{i\theta'}|\le|\theta-\theta'|$. This is a robustness statement for unitary gate approximations; it does not by itself correct [quantum decoherence](../../../../../quantum-decoherence.md), correlated stochastic faults, or limitations of hardware connectivity.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
