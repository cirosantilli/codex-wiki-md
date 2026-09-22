<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For a normalized [computational history state](../../../../../../computational-history-state.md), the output projector sees only its final clock component. With $p_+(\zeta)$ the [quantum circuit](../../../../../../quantum-circuit-split.md)'s acceptance probability,

$$
\boxed{\langle\operatorname{hist}(\zeta)|H_{\rm out}|\operatorname{hist}(\zeta)\rangle=\frac{1-p_+(\zeta)}{T+1}.}
$$

This proves the hint, including for a [computational basis](../../../../../../computational-basis.md) [quantum witness](../../../../../../quantum-witness.md). Moreover $H_{\rm out}=|-\rangle\langle-|_1\otimes|T\rangle\langle T|$ is a [stoquastic Hamiltonian](../../../../../../stoquastic-hamiltonian.md) term, so adding it with positive coefficient preserves stoquasticity.

There are two substantive problems with the stated promise. First, for any basis [quantum witness](../../../../../../quantum-witness.md) the initialized state has nonnegative amplitudes, and every [permutation matrix](../../../../../../permutation-matrix.md) preserves them. Write the output as $|0\rangle|r_0\rangle+|1\rangle|r_1\rangle$, with both vectors entrywise nonnegative. Then

$$
p_+=\frac12+\operatorname{Re}\langle r_0|r_1\rangle\geq\frac12.
$$

The [stoquastic acceptance floor](../../../../../../stoquastic-acceptance-floor.md) rules out the printed one-third soundness condition. There are no NO instances of that literal promise. Second, the [ground space](../../../../../../ground-state-subspace.md) includes histories of arbitrary [quantum witnesses](../../../../../../quantum-witness.md). It is the maximum over those [quantum witnesses](../../../../../../quantum-witness.md), not the maximum over basis [quantum witnesses](../../../../../../quantum-witness.md), that determines the lowest output energy. Even the identity [quantum circuit](../../../../../../quantum-circuit-split.md) accepts each basis input with probability $1/2$, but accepts a $|+\rangle$ [quantum witness](../../../../../../quantum-witness.md) with probability one. Thus a basis-witness soundness bound would not control this Hamiltonian, even if its numerical threshold were repaired.

**The requested nontrivial hardness statement therefore needs the standard quantum-witness StoqMA promise**, with $1/2\leq b<a\leq1$ and inverse-polynomial gap $\gamma=a-b$. The intended reduction can be completed precisely under that corrected promise. Define the [quantum witness](../../../../../../quantum-witness.md) embedding $J|\zeta\rangle=|\zeta\rangle|a\rangle$ and the [witness acceptance operator](../../../../../../witness-acceptance-operator.md)

$$
F=J^\dagger U^\dagger(|+\rangle\langle+|_1\otimes I)UJ.
$$

It is a positive contraction, and $p_{\max}=\lambda_{\max}(F)$. The minimum expectation of $H_{\rm out}$ on the history [ground space](../../../../../../ground-state-subspace.md) is $\nu=(1-p_{\max})/(T+1)$. This is also consistent with a nonnegative optimal [StoqMA](../../../../../../stoqma.md) [quantum witness](../../../../../../quantum-witness.md): $F$ is entrywise nonnegative, so replacing amplitudes by their absolute values cannot decrease its [quadratic form](../../../../../../quadratic-form.md).

A uniform [ground-space perturbation bound](../../../../../../ground-space-perturbation-bound.md) is needed because the gap shrinks with [quantum circuit](../../../../../../quantum-circuit-split.md) length. Put $g=(T+1)^{-3}$, and choose a positive inverse-polynomial coefficient

$$
\delta=\frac{g\gamma}{16(T+1)}.
$$

For $P$ the history ground projector and any [unit vector](../../../../../../unit-vector.md) $\psi=p+q$ with $p=P\psi$, the [operator norm](../../../../../../operator-norm.md) bound $\|H_{\rm out}\|=1$ gives

$$
\langle\psi|(H+\delta H_{\rm out})|\psi\rangle\geq g\|q\|^2+\delta\nu\|p\|^2-2\delta\|p\|\|q\|\geq\delta\nu-\frac{\delta^2}{g-\delta}.
$$

The last inequality completes the square in $\|q\|$ and uses $0\leq\nu\leq1$. Testing a [ground space](../../../../../../ground-state-subspace.md) minimizing vector gives the upper bound $\lambda_{\min}(H')\leq\delta\nu$. Since $\delta<g/2$, we obtain

$$
\delta\nu-2\delta^2/g\leq\lambda_{\min}(H')\leq\delta\nu.
$$

YES instances of the corrected promise have energy at most $\delta(1-a)/(T+1)$; NO instances have energy at least

$$
\frac{\delta(1-b)}{T+1}-\frac{2\delta^2}{g}\geq\frac\delta{T+1}\left(1-b-\frac\gamma8\right).
$$

The separation is at least $7\delta\gamma/[8(T+1)]$, an inverse polynomial. The [quantum circuit](../../../../../../quantum-circuit-split.md) and all these Hamiltonian terms have polynomial-size descriptions. This proves [StoqMA](../../../../../../stoqma.md) hardness for the [local Hamiltonian problem](../../../../../../local-hamiltonian-problem.md) variant that permits the nonlocal clock, under the corrected [quantum witness](../../../../../../quantum-witness.md) and acceptance promise.

The printed perturbation formula also has $H_{\rm out}$ where a general perturbation $V$ belongs. Its unspecified $O(\delta^2)$ cannot be treated as uniform in a closing gap. Likewise a circuit-length-independent constant $\delta$ cannot in general satisfy the stated small-perturbation requirement for an arbitrary long [quantum circuit](../../../../../../quantum-circuit-split.md). The explicit bound above avoids both issues; it does not claim the defective literal promise defines standard [StoqMA](../../../../../../stoqma.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
