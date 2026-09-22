<h1 id="12i/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Suppose first that $A$ is a [regular language](../../../../../../regular-language.md), accepted by a [deterministic finite automaton](../../../../../../deterministic-finite-automaton.md) $D$. If two words reach the same state, then every continuation is accepted from both or rejected from both. Thus they are equivalent under $\sim_A$, and the number of equivalence classes is at most the finite number of states of $D$.

Conversely, suppose $\sim_A$ has finitely many classes. Define a deterministic automaton by

$$
Q=\Sigma^*/{\sim_A},
\qquad
q_0=[\varepsilon],
\qquad
\delta([w],a)=[wa],
$$

and

$$
F=\{[w]:w\in A\}.
$$

The transition is well defined: if $v\sim_Aw$, then for every suffix $u$,

$$
vau\in A\Longleftrightarrow wau\in A,
$$

so $va\sim_Awa$. Likewise, membership in $F$ is independent of the representative by taking the empty suffix in the definition of $\sim_A$. Induction gives

$$
\widehat\delta([\varepsilon],w)=[w],
$$

so the automaton accepts exactly $A$. It has finitely many states, and therefore $A$ is regular. This proves the [Myhill-Nerode theorem](../../../../../../myhill-nerode-theorem.md) in the stated formulation. The assumption $\varepsilon\notin A$ merely says that the initial state is not accepting.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [12I](../../12i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
