<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [promise problem](../../../../../../promise-problem.md) $(L_{\rm yes},L_{\rm no})$ belongs to [QMA](../../../../../../qma.md) if there are polynomials $p,q$ and a uniform family of [quantum circuits](../../../../../../quantum-circuit-split.md) $V_x$ of size at most $q(|x|)$, taking a $p(|x|)$-qubit witness and clean ancillas, with one output qubit interpreted as acceptance, such that

$$
\boxed{\begin{aligned}
x\in L_{\rm yes}&\Longrightarrow
\exists\rho:\ \Pr[V_x\text{ accepts }\rho]\geq\frac23,\\
x\in L_{\rm no}&\Longrightarrow
\forall\rho:\ \Pr[V_x\text{ accepts }\rho]\leq\frac13.
\end{aligned}}
$$

No condition is imposed outside the promise. The witness may be an arbitrary [density operator](../../../../../../density-matrix.md), and the verifier is efficient but need not know how to prepare an honest witness. Pure witnesses suffice for completeness because the acceptance probability is linear in the witness. [QMA](../../../../../../qma.md) is quantum verification with polynomially many witness [qubits](../../../../../../qubit.md) and a constant completeness-soundness gap.

## ↑ Ancestors (11)

1. [A](../a.md)
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
