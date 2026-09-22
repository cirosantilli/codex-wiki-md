<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The matrices obey $Q=P^T$, so both players' pure [best response](../../../../../../best-response.md) vectors have the form $Px$ against opponent mixture $x$. Against pure actions $1,2,3$, the unique best responses are respectively $3,1,2$. This three-cycle has no mutual best-response pair, so there is no pure [Nash equilibrium](../../../../../../nash-equilibrium.md).

In a game satisfying [nondegeneracy of a bimatrix game](../../../../../../nondegeneracy-of-a-bimatrix-game.md), the two equilibrium [strategy supports](../../../../../../strategy-support.md) have equal cardinality: each support consists of best responses to the other strategy, so each size is at most the other. If both supports have size three, $Px$ must have all coordinates equal. The first-minus-second and second-minus-third equations imply

$$
2x_1+x_2-x_3=0,\qquad -3x_1+x_2+2x_3=0,
\qquad x_1+3x_2=0.
$$

This has no fully positive simplex solution. Thus both supports have size two.

For full [support enumeration for a bimatrix game](../../../../../../support-enumeration-for-a-bimatrix-game.md), denote the three possible supports by $12,13,23$. On equal supports $12$ and $23$, indifference requires respectively probabilities $(-1,2)$ and $(2,-1)$, so those pairs fail. Equal support $13$ gives $x_1=x_3=1/2$, whose omitted-action payoff is $1<3/2$. The cross pair $(12,13)$ yields

$$
s=(2/3,1/3,0),\qquad t=(1/3,0,2/3),
$$

with $Pt=(4/3,4/3,1)^T$ and $Ps=(7/3,2/3,7/3)^T$. Thus the supported actions are best responses. Its reversed pair is also an equilibrium. The remaining unordered cross pairs fail: for $(12,23)$ the necessary $s=(1/4,3/4,0)$ gives $Ps=(11/4,3/2,3/2)^T$, so the opponent has a profitable action outside its support. For $(13,23)$, the necessary opponent mixture on $23$ is $(0,-1,2)$, which is infeasible. Reversing either failed pair cannot rescue it.

Hence **all three equilibria** are

$$
\boxed{\begin{aligned}
(s,t)&=((2/3,1/3,0),(1/3,0,2/3)),\\
(s,t)&=((1/3,0,2/3),(2/3,1/3,0)),\\
(s,t)&=((1/2,0,1/2),(1/2,0,1/2)).
\end{aligned}}
$$

Their payoffs are respectively $(4/3,7/3)$, $(7/3,4/3)$ and $(3/2,3/2)$. The support-size argument and exhaustion above rule out every other equilibrium.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
