<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $w(S)=|S|!(n-|S|-1)!/n!$ for $S\subseteq N\setminus\{i\}$. Under the bijection $S\mapsto R=(N\setminus\{i\})\setminus S$, the weights satisfy $w(S)=w(R)$ and $N\setminus S=R\cup\{i\}$. Consequently

$$
\sum_Sw(S)v(N\setminus S)=\sum_Rw(R)v(R\cup\{i\}).
$$

Subtracting $\sum_Sw(S)v(S)$ proves the alternative [Shapley value](../../../../../../shapley-value.md) expression

$$
\boxed{\phi_i(v)=\sum_{S\subseteq N\setminus\{i\}}w(S)\bigl(v(N\setminus S)-v(S)\bigr).}
$$

For the [dual coalitional game](../../../../../../dual-coalitional-game.md) $v'(S)=v(N)-v(N\setminus S)$, its [marginal contribution](../../../../../../marginal-contribution.md) at predecessor set $S$ is

$$
v'(S\cup\{i\})-v'(S)=v(N\setminus S)-v(N\setminus(S\cup\{i\}))=v(R\cup\{i\})-v(R).
$$

The same weight-preserving complement bijection therefore gives $\phi_i(v')=\phi_i(v)$, and both equal the displayed expression. **The [Shapley value](../../../../../../shapley-value.md) is invariant under coalitional duality.** This [Shapley self-duality](../../../../../../shapley-self-duality.md) calculation complements within $N\setminus\{i\}$, not within $N$ without accounting for the distinguished player.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
