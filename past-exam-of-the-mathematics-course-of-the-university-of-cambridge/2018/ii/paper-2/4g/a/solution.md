<h1 id="4g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a set $S\subseteq Q_E$, let $E(S)$ be its [epsilon closure](../../../../../../epsilon-closure.md), and put

$$
\delta_E(S,a)=\bigcup_{q\in S}\delta_E(q,a).
$$

The [subset construction with epsilon transitions](../../../../../../subset-construction-with-epsilon-transitions.md) gives the [deterministic finite automaton](../../../../../../deterministic-finite-automaton.md)

$$
Q_D=\mathcal P(Q_E),
\qquad q_D=E(\{q_0\}),
$$



$$
\boxed{\delta_D(S,a)=E\bigl(\delta_E(S,a)\bigr),
\qquad
F_D=\{S\subseteq Q_E:S\cap F_E\ne\varnothing\}.}
$$

Unreachable subsets may be deleted from $Q_D$ without changing the recognized language.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4G](../../4g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
