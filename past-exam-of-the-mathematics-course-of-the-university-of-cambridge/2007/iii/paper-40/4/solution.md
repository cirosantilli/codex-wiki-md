<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

In a [transferable utility game](../../../../../transferable-utility-game.md), the [characteristic function of a coalitional game](../../../../../characteristic-function-of-a-coalitional-game.md) assigns each [coalition](../../../../../coalition-game-theory.md) $S$ the total payoff $v(S)$ that its members can attain or guarantee together, normalized by $v(\varnothing)=0$. If disjoint [coalitions](../../../../../coalition-game-theory.md) $S,T$ can combine their separate strategies without interference, their union can secure both payoffs, giving

$$
v(S\cup T)\geq v(S)+v(T),\qquad S\cap T=\varnothing.
$$

This is a [superadditive coalitional game](../../../../../superadditive-coalitional-game.md). The pooling assumption explains the intended assertion, but superadditivity is not automatic for an abstract characteristic function: the two-player values $v(\{1\})=v(\{2\})=v(\{1,2\})=1$, with empty value zero, are a counterexample. Thus the word “always” requires either that pooling assumption or a definition restricting the class of games to superadditive ones.

For the given [bankruptcy game](../../../../../bankruptcy-game.md), the total deficit is $19-15=4$, so the [coalition](../../../../../coalition-game-theory.md) value is $(\sum_{i\in S}c_i-4)_+$. Its computed values are

$$
\begin{gathered}
v(\varnothing)=0,\quad(v(\{1\}),v(\{2\}),v(\{3\}))=(0,2,5),\\
(v(\{1,2\}),v(\{1,3\}),v(\{2,3\}))=(6,9,11),\quad v(N)=15.
\end{gathered}
$$

It is indeed superadditive: for disjoint claim sums $p,q\geq0$, $(p+q-4)_+\geq(p-4)_++(q-4)_+$. If both right-hand terms are positive the difference is $4$; if only one is positive, adding the other claim sum cannot reduce the value; if neither is positive the right side is zero.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
