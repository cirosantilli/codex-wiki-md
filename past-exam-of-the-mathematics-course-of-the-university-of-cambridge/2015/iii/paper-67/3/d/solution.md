<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use an $n$-qubit state as the witness. Uniformly choose a term $h_j$ and perform the two-outcome [positive operator-valued measure](../../../../../../positive-operator-valued-measure.md) $\{I-h_j,h_j\}$. Regard the second outcome as an energy flag. For witness $\rho$, its probability is

$$
\Pr(\text{energy flag})=\frac1M\sum_j\operatorname{Tr}(h_j\rho)
=\operatorname{Tr}\left(\frac HM\rho\right).
$$

This is an efficient [local-energy measurement verification](../../../../../../local-energy-measurement-verification.md): a [unitary operator](../../../../../../unitary-operator.md) on the $k$ relevant [qubits](../../../../../../qubit.md) and one [ancilla qubit](../../../../../../ancilla-qubit.md) can implement the measurement using the isometry

$$
|\psi\rangle|0\rangle\longmapsto
\sqrt{I-h_j}\,|\psi\rangle|0\rangle+\sqrt{h_j}\,|\psi\rangle|1\rangle.
$$

The local dimension is constant; the term matrices and the measurement can be approximated to inverse-polynomial accuracy. Uniform choice of $j$ and the classical threshold comparison also have polynomial overhead.

Set

$$
p_{\rm y}=\frac aM,\qquad p_{\rm n}=\frac bM,\qquad
\delta=p_{\rm n}-p_{\rm y},\qquad
\theta=\frac{p_{\rm y}+p_{\rm n}}2.
$$

In the nontrivial case $0\leq a<b\leq M$, $\delta$ is inverse-polynomial. Cases outside this energy range are decided directly from $0\leq H\leq MI$.

Ask for $r$ witness registers, measure an independently sampled local term on each, and accept if the mean number of energy flags is at most $\theta$. An honest product [ground state](../../../../../../ground-state.md) on a YES instance has flag probability at most $p_{\rm y}$. The [Hoeffding inequality](../../../../../../hoeffding-inequality.md) gives failure at most $e^{-r\delta^2/2}$. For completeness, the required Bernoulli concentration estimate follows by bounding the centered log [moment-generating function](../../../../../../moment-generating-function.md) $f(\lambda)=\ln\mathbb E e^{\lambda(Y-p)}$: $f(0)=f'(0)=0$ and $f''(\lambda)$ is a tilted Bernoulli variance, at most $1/4$. Hence $f(\lambda)\leq\lambda^2/8$; exponential [Markov's inequality](../../../../../../markov-inequality.md) optimized at $\lambda=4u$ yields $\Pr(\overline Y-p\geq u)\leq e^{-2ru^2}$, and the lower-tail version follows in the same way.

Soundness must also cover entangled witness registers. The averaged flag effect is $R=H/M$. All its [eigenvalues](../../../../../../eigenvalue.md) are at least $p_{\rm n}$ on a NO instance. The repeated verifier's acceptance effect is a polynomial in the commuting tensor-factor operators $R_j$ and $I-R_j$. In their product eigenbasis its [eigenvalues](../../../../../../eigenvalue.md) are lower-tail probabilities of independent Bernoulli variables whose parameters are each at least $p_{\rm n}$. Their lower tail is bounded by the identical-parameter tail at $p_{\rm n}$, using the same uniform-variable coupling as in [QMA parallel repetition with entangled witnesses](../../../../../../qma-parallel-repetition-with-entangled-witnesses.md). Therefore its [operator norm](../../../../../../operator-norm.md) is at most $e^{-r\delta^2/2}$, which bounds acceptance for any entangled witness.

Choosing

$$
\boxed{r\geq\frac{2\ln3}{\delta^2}
=O\!\left(\frac{M^2}{(b-a)^2}\right)}
$$

gives completeness at least $2/3$ and soundness at most $1/3$. A slightly larger constant absorbs implementation errors; for example, approximate each flag effect in norm to at most $\delta/8$, retain a gap at least $3\delta/4$, and increase $r$ by a constant factor. The total witness length $rn$ and circuit size are polynomial. Thus

$$
\boxed{\text{Local Hamiltonian}\in\mathrm{QMA}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
