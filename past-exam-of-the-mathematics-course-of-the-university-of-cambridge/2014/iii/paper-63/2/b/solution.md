<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The class $C$ uses [polynomial-register real-arithmetic computation](../../../../../../polynomial-register-real-arithmetic-computation.md): its storage restriction counts real registers, without limiting their precision or the running time. Use the usual decision-model interpretation that computed real values may be compared with fixed thresholds, and that the fixed universal gate set's real constants are available. Without a way to test values, arithmetic instructions alone would not specify the intended decision model.

Let a [BQP](../../../../../../bqp.md) [quantum circuit](../../../../../../quantum-circuit-split.md) use $q=\operatorname{poly}(n)$ qubits and $T=\operatorname{poly}(n)$ gates. A [matrix element](../../../../../../matrix-element.md) can be evaluated by [depth-first quantum circuit path summation](../../../../../../depth-first-quantum-circuit-path-summation.md):

$$
\langle z_T|U_T\cdots U_1|z_0\rangle=\sum_{z_1,\ldots,z_{T-1}}\prod_{t=1}^T\langle z_t|U_t|z_{t-1}\rangle.
$$

Enumerate the intermediate $q$-bit strings recursively. Store the current strings and loop positions, a partial product, and the partial sum at each depth. There are at most $T$ active levels, using $O(qT)$ registers or bits of loop information, not an exponentially long state vector. Each fixed-locality gate [matrix element](../../../../../../matrix-element.md) is computed from its few affected bits. Represent a complex number by two real registers; complex multiplication and addition require only real addition, subtraction and multiplication.

Recompute this amplitude separately for every final string $z$ whose output bit is one, accumulating the [Born rule](../../../../../../born-rule.md) probability

$$
\boxed{p_1=\sum_{z:z_1=1}|\langle z|U|x,0\cdots0\rangle|^2.}
$$

The outer enumeration needs only another $O(q)$ bits and a real accumulator. Arbitrarily large running time is allowed, so repeated recomputation is harmless. Compare $p_1$ with $1/2$ to distinguish the promised [BQP](../../../../../../bqp.md) cases. This proves **$\mathrm{BQP}\subseteq C$** using polynomial storage.

The printed probability hint omits the squares of the amplitude moduli. Summing their absolute values alone is not the [Born rule](../../../../../../born-rule.md) and can exceed one. The corrected sum above is necessary for the containment proof. The argument is about the stated real-register model, rather than a claim that exponential-precision numbers are free in an ordinary bit-cost model.

## ↑ Ancestors (11)

1. [B](../b.md)
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
