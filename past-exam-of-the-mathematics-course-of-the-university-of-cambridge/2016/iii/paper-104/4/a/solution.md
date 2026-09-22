<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

We give a [finite semigroup presentation](../../../../../../finite-semigroup-presentation.md) using the convention that $s_0$ is blank, the tape is unbounded in both directions, and a transition $\delta(q_i,s_j)=(q_k,s_p,D)$ writes $s_p$ and moves in direction $D$. The [Turing machine](../../../../../../turing-machine.md) is deterministic, and the halting state $q_0$ has no outgoing transition. A finite configuration is encoded by

$$
hu q_i v h,\qquad u,v\in S^*,
$$

with the head scanning the first symbol of $v$; if $v$ is empty, it scans an implicit blank. Unrepresented cells beyond the boundary markers $h$ are blank. An additional generator $q$ records completed halting and erasure.

The generators of the [semigroup](../../../../../../semigroup.md) are $S\sqcup Q\sqcup\{h,q\}$. Its relations have the following finite families. For every right-moving transition, include

$$
q_i s_j=s_p q_k\qquad\text{if }\delta(q_i,s_j)=(q_k,s_p,R).
$$

For every left-moving transition and every tape symbol $s_\ell$, include

$$
s_\ell q_i s_j=q_k s_\ell s_p\qquad\text{if }\delta(q_i,s_j)=(q_k,s_p,L).
$$

If stationary moves are part of the chosen machine model, include $q_i s_j=q_k s_p$ for each such move. Include the boundary-padding relations, for every state $q_i$,

$$
hq_i=hs_0q_i,\qquad q_i h=q_i s_0h.
$$

They supply a blank immediately to the left of the head when needed, or at the right boundary when the current scanned cell was implicit. Finally include

$$
q_0=q,\qquad s_jq=q=qs_j\ (0\le j\le m),\qquad hq=q=qh.
$$

Writing $\mathcal R_T$ for this displayed list, the answer is the explicit [finite semigroup presentation](../../../../../../finite-semigroup-presentation.md)

$$
\boxed{\Gamma(T)=\langle S\sqcup Q\sqcup\{h,q\}\mid\mathcal R_T\rangle.}
$$

All relations are between nonempty words; no group inverses or empty-word generator are used. The transition families are finite because the transition table and alphabet are finite, and the padding and erasure families are visibly finite. The declared head convention determines which side of a tape symbol carries a state letter.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 104](../../../paper-104-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
