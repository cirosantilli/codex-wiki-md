<h1 id="3/f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [halting problem](../../../../../../halting-problem.md) is an unconditional example:

$$
\boxed{\mathrm{HALT}\text{ is NP-hard but not NP-complete}.}
$$

Reduce [SAT](../../../../../../boolean-satisfiability-problem.md) to it as follows. Given a [Boolean formula](../../../../../../boolean-formula.md) $\varphi$, construct a [Turing machine](../../../../../../turing-machine.md) $M_\varphi$ that ignores its input, enumerates all [Boolean valuations](../../../../../../boolean-valuation.md) of $\varphi$, and halts if it finds a satisfying one. If none satisfies $\varphi$, it enters an infinite loop after the enumeration. Then

$$
\varphi\in\mathrm{SAT}\quad\Longleftrightarrow\quad\langle M_\varphi,\varepsilon\rangle\in\mathrm{HALT}.
$$

The construction of the machine description takes [polynomial time](../../../../../../polynomial-time.md); the potentially exponential running time of the constructed machine is irrelevant to the time needed to compute the [polynomial-time reduction](../../../../../../polynomial-time-reduction.md). Since [SAT](../../../../../../boolean-satisfiability-problem.md) is [NP-complete](../../../../../../np-completeness.md), this proves [NP-hardness](../../../../../../np-hardness.md) of the [halting problem](../../../../../../halting-problem.md).

Every problem in [NP](../../../../../../np-complexity.md) is decidable, by enumerating the finitely many polynomial-length certificates and running the verifier. The [halting problem](../../../../../../halting-problem.md) is [undecidable](../../../../../../undecidable-decision-problem.md), so it is outside [NP](../../../../../../np-complexity.md) and therefore cannot be [NP-complete](../../../../../../np-completeness.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [F](../../f.md)
3. [3](../../../3.md)
4. [Knowledge representation and reasoning](../../../../knowledge-representation-and-reasoning-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
