<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[BQP](../../../../../../bqp.md) consists of [promise problems](../../../../../../promise-problem.md) decided by a uniform family of polynomial-size [quantum circuits](../../../../../../quantum-circuit-split.md). On input $x$, with polynomially many zero-initialized [ancilla qubits](../../../../../../ancilla-qubit.md), a designated output measurement accepts with probability at least $2/3$ on YES inputs and at most $1/3$ on NO inputs. Uniformity means a classical polynomial-time procedure produces the [quantum circuit](../../../../../../quantum-circuit-split.md) description from the input length, or equivalently produces the verifier [quantum circuit](../../../../../../quantum-circuit-split.md) with $x$ supplied as input.

For [BQP error reduction](../../../../../../bqp-error-reduction.md), run independent copies with freshly initialized registers. If the completeness and soundness thresholds are any constants $a>b$, accept when the fraction of accepting trials exceeds $(a+b)/2$. A [Hoeffding inequality](../../../../../../hoeffding-inequality.md) bounds either error by $\exp[-r(a-b)^2/2]$, with $r$ repetitions. The threshold need not be a simple majority when both $a$ and $b$ lie on the same side of $1/2$.

Choosing $r$ sufficiently large gives the usual $2/3,1/3$ thresholds, or any other fixed separated thresholds. Even an inverse-polynomial gap can be amplified using polynomially many repetitions. Classical threshold evaluation can be incorporated into the uniform computation. **Thus fixed separated acceptance probabilities define the same BQP class.** This argument concerns unrestricted [BQP](../../../../../../bqp.md) [quantum circuits](../../../../../../quantum-circuit-split.md) and does not assume such amplification is available for restricted [stoquastic circuits](../../../../../../stoquastic-circuit.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
