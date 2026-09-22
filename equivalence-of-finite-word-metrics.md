# Equivalence of finite word metrics

↑ **Parent:** [Word metric](word-metric.md)

Changing a finite [generating set of a group](generating-set-of-a-group.md) changes individual distances, but it cannot introduce arbitrarily large relative distortion. For two finite symmetric [generating sets of a group](generating-set-of-a-group.md) $S,T$ of the same [group](group-split.md), set

$$
K=\max\bigl(\{1\}\cup\{|s|_T:s\in S\}\bigr),\qquad L=\max\bigl(\{1\}\cup\{|t|_S:t\in T\}\bigr).
$$

Each $S$-letter can be replaced by at most $K$ $T$-letters, and conversely each $T$-letter by at most $L$ $S$-letters. Applying these substitutions to shortest representatives of $g^{-1}h$ gives

$$
\frac1L d_S(g,h)\leq d_T(g,h)\leq Kd_S(g,h).
$$

Thus the [identity map](identity-function.md) is a [bilipschitz equivalence](bilipschitz-equivalence.md) between the two [word metrics](word-metric.md), and hence a [quasi-isometry](quasi-isometry.md). The constants depend on the chosen [generating sets of a group](generating-set-of-a-group.md).[Mann, Proposition 1.2: bilipschitz equivalence](https://webusers.imj-prg.fr/~kathryn.mann/classes/GGRminicourse.pdf)

In the [Cayley graphs of the integers](cayley-graphs-of-the-integers.md) example, $S=\{-1,1\}$ and $T=\{-2,-1,1,2\}$ give $K=1$ and $L=2$: a unit move costs one in either alphabet, and a move of size two costs two unit moves. This recovers $d_T\leq d_S\leq2d_T$. The diamond and square in [word metric balls in the integer lattice](word-metric-balls-in-the-integer-lattice.md) obey the same comparison, because $\max\{|m|,|n|\}\leq|m|+|n|\leq2\max\{|m|,|n|\}$.

Finiteness cannot simply be dropped from this universal statement. For the additive [integers](integer-split.md), take the infinite symmetric [generating set of a group](generating-set-of-a-group.md) $U=\mathbb Z\setminus\{0\}$. Every nonzero displacement is a single allowed move, so $d_U(a,b)=1$ whenever $a\ne b$, whereas $d_S(0,n)=|n|$ for $S=\{-1,1\}$. There is no finite $L$ with $d_S\leq Ld_U$: choosing an [integer](integer-split.md) $n>L$ violates it. This is a counterexample to unrestricted equivalence, not a claim that every infinite [generating set of a group](generating-set-of-a-group.md) fails; two such sets with uniformly bounded generator lengths can still satisfy the same substitution bounds.[Mann, remark after Proposition 1.2: bounded metric from allowing all elements](https://webusers.imj-prg.fr/~kathryn.mann/classes/GGRminicourse.pdf)

## ↑ Ancestors (7)

1. [Word metric](word-metric.md)
2. [Cayley graph](cayley-graph.md)
3. [Geometric group theory](geometric-group-theory-split.md)
4. [Geometry and topology](geometry-and-topology-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-5/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-133/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-133/3/b/solution.md)
- [Word length](word-length.md)
