<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [coalitional game](../../../../../transferable-utility-game.md) with transferable utility has a finite player set $N$ and a [characteristic function of a coalitional game](../../../../../characteristic-function-of-a-coalitional-game.md) $v:2^N\to\mathbb R$, normalized by $v(\varnothing)=0$. The value $v(S)$ is the total payoff the [coalition](../../../../../coalition-game-theory.md) $S$ can secure and redistribute among its members.

An [imputation](../../../../../imputation-in-a-coalitional-game.md) is an efficient, individually rational payoff vector:

$$
\boxed{\sum_{i\in N}x_i=v(N),\qquad x_i\geq v(\{i\})\quad(i\in N).}
$$

The [core of a cooperative game](../../../../../core-game-theory.md) consists of imputations satisfying every coalition constraint:

$$
\boxed{C(v)=\left\{x:\sum_{i\in N}x_i=v(N),\quad \sum_{i\in S}x_i\geq v(S)\text{ for every }S\subseteq N\right\}.}
$$

A [coalition](../../../../../coalition-game-theory.md) assigned less than its characteristic value can leave and make every member better off, by sharing the positive surplus. Conversely a coalition with no such surplus cannot improve every member's payoff simultaneously. This explains the stability represented by the [core of a cooperative game](../../../../../core-game-theory.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
