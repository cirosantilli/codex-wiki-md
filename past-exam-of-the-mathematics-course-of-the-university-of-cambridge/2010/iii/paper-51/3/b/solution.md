<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An upper bound follows directly from the [Schmidt-tail entanglement monotone](../../../../../../schmidt-tail-entanglement-monotone.md)

$$
E_2(\chi)=1-\lambda_{\max}(\rho_A^\chi),
$$

where $\rho_A^\chi$ is the [reduced density matrix](../../../../../../reduced-density-matrix.md) of a bipartite pure state. On these two-qubit states, this is the smaller squared [Schmidt coefficient](../../../../../../schmidt-coefficient.md), so $E_2(\psi)=s$ and $E_2(\phi)=t$.

Here is the average-monotonicity argument needed for all [LOCC](../../../../../../local-operations-and-classical-communication.md) strategies. The largest [eigenvalue](../../../../../../eigenvalue.md) is convex: for any unit vector $v$, $\langle v|\sum_r p_r\rho_r|v\rangle\leq\sum_r p_r\lambda_{\max}(\rho_r)$, and maximizing the left side gives the claim. Hence $1-\lambda_{\max}$ is concave. If Alice makes a local measurement, Bob's conditional reductions average to his original reduction. Concavity therefore gives $\sum_r p_rE_2(\chi_r)\leq E_2(\chi)$. If Bob measures, use Alice's reductions instead. The two reductions of a pure state have the same nonzero eigenvalues by the [Schmidt decomposition](../../../../../../schmidt-decomposition.md). Refining all measurement outcomes into individual [Kraus operators](../../../../../../kraus-operator.md) keeps conditional states pure; iterating the inequality covers adaptive rounds of classical communication. The same bound persists for limits of such protocols.

If success produces the target with probability $p$, its contribution to the final average is $pt$. Failure branches have nonnegative $E_2$. Thus

$$
pt\leq s,\qquad
\boxed{p_{\max}\leq\frac{s}{t}=\frac{\sin^2\alpha}{\sin^2\beta}.}
$$

This is a bound on arbitrary local protocols, not merely on a particular filtering measurement.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
