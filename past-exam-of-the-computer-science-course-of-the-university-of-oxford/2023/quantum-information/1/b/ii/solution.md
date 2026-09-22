<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write the proposed [quantum state ensemble](../../../../../../quantum-state-ensemble.md) as $\{(|u\rangle,p),(|v\rangle,1-p)\}$ with normalized [pure states](../../../../../../pure-state.md), so that

$$
\frac I2=p|u\rangle\langle u|+(1-p)|v\rangle\langle v|.
$$

Taking the [expectation values](../../../../../../expectation-value.md) in $|u\rangle$ and $|v\rangle$, and setting $c=|\langle u|v\rangle|^2$, gives

$$
\frac12=p+(1-p)c\geq p,
\qquad
\frac12=pc+1-p\geq1-p.
$$

Consequently $p\leq1/2$ and $p\geq1/2$. Substitution then gives $c=0$. The two [pure states](../../../../../../pure-state.md) are therefore [orthogonal](../../../../../../orthogonal-vectors.md), with equal [probabilities](../../../../../../probability.md):

$$
\boxed{p=\frac12,\qquad |v\rangle=|u^\perp\rangle\ \text{up to a global phase}.}
$$

Conversely, any [orthonormal basis](../../../../../../orthonormal-basis.md) of a [qubit](../../../../../../qubit.md) has projectors summing to $I$, so such a [quantum state ensemble](../../../../../../quantum-state-ensemble.md) does give $I/2$. This proves the characterization of [two-state ensembles of a maximally mixed qubit](../../../../../../two-state-ensembles-of-a-maximally-mixed-qubit.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
