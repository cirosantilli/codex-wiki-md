# Word length

↑ **Parent:** [Word metric](word-metric.md)

The [word length](word-length.md) is the cost of building a [group element](group-element.md) from the allowed [generators of a group](generator-of-a-group.md). For a symmetric [generating set of a group](generating-set-of-a-group.md) $S$ of a [group](group-split.md) $G$, define

$$
|g|_S=\min\{n\geq0:g=s_1\cdots s_n,\ s_i\in S\}.
$$

The empty [word over an alphabet](string.md) represents the [identity element](identity-element.md) and has length zero. A representative with this least number of letters labels a shortest [graph path](path-in-a-graph.md) from $1$ to $g$ in the [Cayley graph](cayley-graph.md). Thus [word length](word-length.md) minimizes over all representatives, rather than counting the letters in whichever expression we happened to write down.[Mann, Definition 1.1: word norm](https://webusers.imj-prg.fr/~kathryn.mann/classes/GGRminicourse.pdf)

For the additive [integers](integer-split.md) with $S=\{-1,1\}$, the expression $1+1-1$ has three letters but represents $1$, whose [word length](word-length.md) is one. With $T=\{-2,-1,1,2\}$, the [integer](integer-split.md) $5$ has [word length](word-length.md) three, realized by $2+2+1$. The [Cayley graphs of the integers](cayley-graphs-of-the-integers.md) visualize why these are minimal. A [freely reduced word](freely-reduced-word.md) is always shortest in a [free group](free-group.md) with its free generators and their inverses; [free reduction](free-reduction.md) alone need not give a shortest representative in a general [group](group-split.md).

Concatenating representatives and reversing their letters with [inverse elements](inverse-element.md) give

$$
|gh|_S\leq|g|_S+|h|_S,\qquad |g^{-1}|_S=|g|_S,\qquad |g|_S=d_S(1,g).
$$

These make [word length](word-length.md) a [length function](length-function.md). A finite $S$ gives finite [word metric balls](word-metric-ball.md), since only finitely many [words over an alphabet](string.md) have length at most a fixed radius. The definition itself also works for infinite symmetric [generating sets of a group](generating-set-of-a-group.md); the bounded-metric example in [equivalence of finite word metrics](equivalence-of-finite-word-metrics.md) shows what finiteness adds.

## ↑ Ancestors (7)

1. [Word metric](word-metric.md)
2. [Cayley graph](cayley-graph.md)
3. [Geometric group theory](geometric-group-theory-split.md)
4. [Geometry and topology](geometry-and-topology-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Length of a word over an alphabet](length-of-a-word-over-an-alphabet.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-16/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-16/5/b/solution.md)
- [Shortest conjugacy representative](shortest-conjugacy-representative.md)
- [Word length](word-length.md)
- [Word metric](word-metric.md)
- [Word metric balls in the integer lattice](word-metric-balls-in-the-integer-lattice.md)
