<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the PDF's entry $P_{12}=4$, rather than the TeX aid's $2$. To check [nondegeneracy of a bimatrix game](../../../../../../nondegeneracy-of-a-bimatrix-game.md), every opponent strategy of support size $k$ must have at most $k$ pure [best responses](../../../../../../best-response.md). Against each pure column, the unique best rows are respectively $3,1,2$. Against each pure row, the unique best columns are respectively $1,2,2$.

The only mixture making all three rows indifferent solves $-y_1+2y_3=0$ and $-2y_1+2y_2-3y_3=0$, giving $y=(4,7,2)/13$, which has support size three. Thus no two-column-support mixture has three best rows. For the other player, column $1$ strictly dominates column $3$, because their payoff difference is $(1,1,2)$, so three best columns are impossible. These observations cover all support sizes, proving **the game is nondegenerate**.

For the [Lemke-Howson algorithm](../../../../../../lemke-howson-algorithm.md), use unnormalized strategy vectors $u,v$ in the polytopes

$$
\mathcal X=\{u\geq0:Q^Tu\leq\mathbf1\},\qquad\mathcal Y=\{v\geq0:Pv\leq\mathbf1\}.
$$

A row label $i\in\{1,2,3\}$ occurs at $u_i=0$ in $\mathcal X$ or at $(Pv)_i=1$ in $\mathcal Y$. A column label $3+j$ occurs at $(Q^Tu)_j=1$ in $\mathcal X$ or at $v_j=0$ in $\mathcal Y$. The origin pair has all six labels.

Drop row label $3$ by increasing $u_3$. Column $2$ is the first binding payoff constraint, at $u_3=1/4$, so label $5$ becomes duplicated. Drop $5$ in $\mathcal Y$ by increasing $v_2$; row $1$ binds first, at $v_2=1/4$, duplicating label $1$. Drop $1$ in $\mathcal X$ by increasing $u_1$ while keeping $u_2=0$ and the column-$2$ constraint binding. Since that constraint does not involve $u_1$, $u_3$ stays $1/4$. Column $1$ binds at $u_1=1/4$, duplicating label $4$.

Now drop $4$ in $\mathcal Y$ by increasing $v_1$. Keep $v_3=0$ and row $1$ binding, so $v_2=1/4$. Row $3$ reaches payoff $1$ at $v_1=1/6$, earlier than row $2$, which would bind at $v_1=1/4$. The missing label $3$ returns, terminating the path. The successive vertex-label pairs are

$$
\begin{array}{c|c|c|c|c}
\text{step}&u&\text{labels in }\mathcal X&v&\text{labels in }\mathcal Y\\\hline
0&(0,0,0)&1,2,3&(0,0,0)&4,5,6\\
1&(0,0,1/4)&1,2,5&(0,0,0)&4,5,6\\
2&(0,0,1/4)&1,2,5&(0,1/4,0)&1,4,6\\
3&(1/4,0,1/4)&2,4,5&(0,1/4,0)&1,4,6\\
4&(1/4,0,1/4)&2,4,5&(1/6,1/4,0)&1,3,6
\end{array}
$$

The final pair is completely labelled and nonzero. Normalize each vector by its own sum to obtain

$$
\boxed{x=(\tfrac12,0,\tfrac12),\qquad y=(\tfrac25,\tfrac35,0).}
$$

The row payoffs against $y$ are $(12/5,2,12/5)$ and the column payoffs against $x$ are $(2,2,1/2)$. Both supported actions are best responses, so this is a [Nash equilibrium](../../../../../../nash-equilibrium.md), with **payoffs $\boxed{(12/5,\,2)}$**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
