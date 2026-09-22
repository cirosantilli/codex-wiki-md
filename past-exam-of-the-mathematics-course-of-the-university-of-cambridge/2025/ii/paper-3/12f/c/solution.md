<h1 id="12f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The subset construction theorem gives $\mathcal L(D)=\mathcal L(N)$. Removing inaccessible states does not alter any computation from the initial state, so

$$
\mathcal L(D')=\mathcal L(N).
$$

Every state of $D'$ is accessible by construction. It remains to separate distinct subset states $S,T$ of $D'$. Choose $q\in S\mathbin\triangle T$, and without loss of generality take $q\in S\setminus T$. By (Br2), some word $w$ has a witnessing sequence from $q$ to the unique final state $q_*$. Part (b)(iii) implies

$$
q_*\in\widehat\Delta(q,w),
$$

so the state reached from $S$ on $w$ is accepting.

If the state reached from $T$ on $w$ were also accepting, there would be some $p\in T$ with a witnessing sequence labelled $w$ from $p$ to $q_*$. But $q$ has such a sequence too, and (Br3) says that its starting state is unique. Hence $p=q$, contradicting $q\notin T$. Thus $w$ distinguishes $S$ and $T$.

No two distinct states of $D'$ are indistinguishable, and all are accessible. Therefore $D'$ is irreducible and accepts $\mathcal L(N)$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [12F](../../12f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
