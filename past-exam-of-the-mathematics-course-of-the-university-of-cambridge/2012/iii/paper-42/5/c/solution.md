<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For three players, the predecessor-set weights are $1/3$ for sizes zero and two, and $1/6$ for size one. Thus

$$
\begin{aligned}
\phi_1&=\tfrac13(4)+\tfrac16(10-3)+\tfrac16(11-2)+\tfrac13(12-5)=\tfrac{19}3,\\
\phi_2&=\tfrac13(3)+\tfrac16(10-4)+\tfrac16(5-2)+\tfrac13(12-11)=\tfrac{17}6,\\
\phi_3&=\tfrac13(2)+\tfrac16(11-4)+\tfrac16(5-3)+\tfrac13(12-10)=\tfrac{17}6.
\end{aligned}
$$

Therefore **the [Shapley value](../../../../../../shapley-value.md) is $\boxed{(19/3,17/6,17/6)}$**, whose coordinates sum to $12$.

For the [nucleolus](../../../../../../nucleolus.md), use [imputations](../../../../../../imputation-in-a-coalitional-game.md) $x_1+x_2+x_3=12$, $x_1\geq4$, $x_2\geq3$, $x_3\geq2$. The excess of $\{1,3\}$ is $11-(12-x_2)=x_2-1\geq2$. Thus the smallest possible largest excess is at least $2$. It is attained when $x_2=3$, $x_3=9-x_1$, and $5\leq x_1\leq7$: the remaining proper-coalition excesses then are

$$
e_1=4-x_1,\quad e_2=0,\quad e_3=x_1-7,\quad e_{12}=7-x_1,\quad e_{23}=x_1-7,
$$

all at most $2$, while $e_{13}=2$. Conversely, a largest excess of $2$ forces $x_2=3$ and precisely this interval for $x_1$.

On this first-stage face the top excess $2$ is fixed. The next largest excess is $7-x_1\geq0$, because the other varying excesses are nonpositive and $e_2=0$ is fixed. Its unique minimum is zero at $x_1=7$. No further lexicographic tie remains. Hence **the [nucleolus](../../../../../../nucleolus.md) is $\boxed{(7,3,2)}$**. Its proper-coalition excesses, sorted decreasingly, are $(2,0,0,0,0,-3)$.

Finally, a core allocation would require $x_2\geq3$ and $x_1+x_3\geq11$, whose sum contradicts the efficient total $12$. Thus **the [core of a cooperative game](../../../../../../core-game-theory.md) is empty**. The game is not superadditive, so neither core nonemptiness nor individual rationality of the [Shapley value](../../../../../../shapley-value.md) should be presumed. Under the distinct [prenucleolus](../../../../../../prenucleolus.md) convention the answer would be $(15/2,2,5/2)$. Balancing $e_2=3-x_2$ and $e_{13}=x_2-1$ gives a first-stage maximum of $1$ and forces $x_2=2$. The remaining first-stage constraints restrict $x_1$ to $[7,8]$. The next largest complaints are $e_{12}=8-x_1$ and $e_{23}=x_1-7$, balanced at $x_1=15/2$, with $x_3=5/2$. This is not an [imputation](../../../../../../imputation-in-a-coalitional-game.md) and is not the [nucleolus](../../../../../../nucleolus.md) under the definition in (a).

## ↑ Ancestors (11)

1. [C](../c.md)
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
