<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Shapley value](../../../../../../shapley-value.md) is the expected [marginal contribution](../../../../../../marginal-contribution.md) of a player when the players join in uniformly random order. Equivalently,

$$
\phi_i(v)=\sum_{S\subseteq N\setminus\{i\}}\frac{|S|!(n-|S|-1)!}{n!}\bigl(v(S\cup\{i\})-v(S)\bigr).
$$

For three players, the weights for predecessor sets of sizes $0,1,2$ are $1/3,1/6,1/3$. Using the computed values,

$$
\begin{aligned}
\phi_1&=\tfrac13(0)+\tfrac16[(6-2)+(9-5)]+\tfrac13(15-11)=\tfrac83,\\
\phi_2&=\tfrac13(2)+\tfrac16[(6-0)+(11-5)]+\tfrac13(15-9)=\tfrac{14}3,\\
\phi_3&=\tfrac13(5)+\tfrac16[(9-0)+(11-2)]+\tfrac13(15-6)=\tfrac{23}3.
\end{aligned}
$$

Thus

$$
\boxed{\phi(v)=x:\quad\text{(b) is true.}}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
