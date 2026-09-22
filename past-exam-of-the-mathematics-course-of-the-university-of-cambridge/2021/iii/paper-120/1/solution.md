<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Knaster-Tarski theorem](../../../../../knaster-tarski-theorem.md) states that the fixed points of a monotone map $f:L\to L$ on a [complete lattice](../../../../../complete-lattice.md) form a complete lattice. Let

$$
P=\{x\in L:f(x)\leq x\},
\qquad
m=\bigwedge P.
$$

For every $x\in P$, monotonicity gives $f(m)\leq f(x)\leq x$, hence $f(m)\leq m$. Applying $f$ once more gives $f(f(m))\leq f(m)$, so $f(m)\in P$. The definition of $m$ then gives $m\leq f(m)$, and therefore $f(m)=m$. Thus

$$
\mu f=\bigwedge\{x:f(x)\leq x\}
$$

is the least fixed point. The order-dual argument shows that

$$
\nu f=\bigvee\{x:x\leq f(x)\}
$$

is the greatest fixed point.

More generally, for a family $S$ of fixed points, let $P_S$ be the set of prefixed points $x$ satisfying $f(x)\leq x$ and $s\leq x$ for every $s\in S$. Its meet $m_S$ is again prefixed. Since $s=f(s)\leq f(m_S)$ for every $s\in S$, the element $f(m_S)$ also lies in $P_S$, so the preceding argument gives $f(m_S)=m_S$. It is the join of $S$ within the fixed-point order. The dual construction gives the meet of $S$ within that order, proving completeness.

For the [Myhill-Nerode theorem](../../../../../myhill-nerode-theorem.md), let $A\subseteq\Sigma^*$ and define the [Myhill-Nerode equivalence](../../../../../myhill-nerode-equivalence.md)

$$
u\sim_Av
\quad\Longleftrightarrow\quad
\forall w\in\Sigma^*,
uw\in A\Longleftrightarrow vw\in A.
$$

This is an equivalence relation and a right congruence: $u\sim_Av$ implies $ua\sim_Ava$ for every letter $a$.

If a [deterministic finite automaton](../../../../../deterministic-finite-automaton.md) accepts $A$, any two words reaching the same state are equivalent, because every continuation has the same subsequent run. Hence $\sim_A$ has at most as many classes as the automaton has states. Conversely, if $\sim_A$ has finitely many classes, define an automaton with state set $\Sigma^*/{\sim_A}$, initial state $[\epsilon]$, transition

$$
\delta([u],a)=[ua],
$$

and accepting states $[u]$ with $u\in A$. Right congruence makes the transition well defined, and induction on word length shows that the state reached by $u$ is $[u]$, so the automaton accepts exactly $A$. Therefore $A$ is a [regular language](../../../../../regular-language.md) exactly when $\sim_A$ has finite index. Moreover, every automaton for $A$ has at least one state for each equivalence class, so this quotient is the [minimal deterministic finite automaton](../../../../../minimal-deterministic-finite-automaton.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 120](../../paper-120-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
