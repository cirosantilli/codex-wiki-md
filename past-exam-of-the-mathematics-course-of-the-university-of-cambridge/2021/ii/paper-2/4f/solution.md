<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

For a [deterministic finite automaton](../../../../../deterministic-finite-automaton.md) the [extended transition function of a deterministic finite automaton](../../../../../extended-transition-function-of-a-deterministic-finite-automaton.md) is recursively

$$
\widehat\delta(q,\epsilon)=q,
\qquad
\widehat\delta(q,wa)=\delta(\widehat\delta(q,w),a).
$$

The accepted language is

$$
L(D)=\{w\in\Sigma^*: \widehat\delta(q_0,w)\in F\}.
$$

For a [nondeterministic finite automaton](../../../../../nondeterministic-finite-automaton.md), $\widehat\delta(q,w)$ is the set of all states reachable from $q$ while reading $w$; recursively,

$$
\widehat\delta(q,\epsilon)=\{q\},
\qquad
\widehat\delta(q,wa)=\bigcup_{r\in\widehat\delta(q,w)}\delta(r,a).
$$

Thus

$$
L(N)=\{w\in\Sigma^*: \widehat\delta(q_0,w)\cap F\ne\varnothing\}.
$$

The [powerset construction](../../../../../powerset-construction.md) has state set $\mathcal P(Q)$, initial state $\{q_0\}$, transition

$$
\overline\delta(S,a)=\bigcup_{q\in S}\delta(q,a),
$$

and accepting states $\{S\subseteq Q:S\cap F\ne\varnothing\}$. Induction on $|w|$ gives

$$
\widehat{\overline\delta}(\{q_0\},w)=\widehat\delta(q_0,w),
$$

so the two automata accept exactly the same language. If $|Q|=m$ and $F$ has one state, exactly $2^{m-1}$ of the $2^m$ subset states contain it and are accepting, including states that may be unreachable.

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
