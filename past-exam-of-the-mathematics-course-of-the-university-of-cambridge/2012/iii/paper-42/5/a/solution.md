<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [transferable utility game](../../../../../../transferable-utility-game.md) with $v(\varnothing)=0$, an efficient allocation satisfies $\sum_{i\in N}x_i=v(N)$. An [imputation](../../../../../../imputation-in-a-coalitional-game.md) is efficient and individually rational, $x_i\geq v(\{i\})$. Write $x(S)=\sum_{i\in S}x_i$ and define the [excess of a coalition](../../../../../../excess-of-a-coalition.md) as $e(S,x)=v(S)-x(S)$.

The [core of a cooperative game](../../../../../../core-game-theory.md) is

$$
\boxed{\{x:x(N)=v(N),\quad x(S)\geq v(S)\text{ for every }S\subseteq N\}.}
$$

It consists of allocations immune to a [coalition](../../../../../../coalition-game-theory.md)'s blocking: no [coalition](../../../../../../coalition-game-theory.md) can obtain more for its members by leaving. The singleton inequalities imply individual rationality. The core may be empty.

The [nucleolus](../../../../../../nucleolus.md), when the [imputation](../../../../../../imputation-in-a-coalitional-game.md) set is nonempty, is the unique [imputation](../../../../../../imputation-in-a-coalitional-game.md) that lexicographically minimizes the list of [coalition](../../../../../../coalition-game-theory.md) excesses arranged from largest to smallest. It first minimizes the largest complaint, then the second largest among ties, and so on. Including the empty and grand [coalitions](../../../../../../coalition-game-theory.md) adds constant zeros and does not change the solution. Minimization on efficient allocations without individual rationality instead defines the [prenucleolus](../../../../../../prenucleolus.md), a different convention that matters for this paper's game.

The [Shapley value](../../../../../../shapley-value.md) is the average [marginal contribution](../../../../../../marginal-contribution.md) of each player over all uniformly ordered player arrivals:

$$
\boxed{\phi_i(v)=\sum_{S\subseteq N\setminus\{i\}}\frac{|S|!(n-|S|-1)!}{n!}\bigl(v(S\cup\{i\})-v(S)\bigr).}
$$

Exactly $|S|!(n-|S|-1)!$ orderings have $S$ as the predecessor set of $i$. This is an average-contribution fairness rule, rather than a blocking-stability condition; it need not be individually rational for an arbitrary game.

## ↑ Ancestors (11)

1. [A](../a.md)
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
