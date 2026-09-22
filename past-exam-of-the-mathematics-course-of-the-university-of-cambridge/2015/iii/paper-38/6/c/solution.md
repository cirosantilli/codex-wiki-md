<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Row operations multiply each original tableau equation by an invertible matrix. The [slack variable](../../../../../../slack-variable.md) block therefore records that matrix and allows the original [payoff matrix](../../../../../../payoff-matrix.md) to be recovered without guessing.

From the first tableau, let $X$ be the coefficient block of $x$ and $S$ that of $s$. Since its original equations were $Q^Tx+s=\mathbf1$, we have $Q^T=S^{-1}X$. Here

$$
S^{-1}=\begin{pmatrix}4&0&1\\1&1&1\\3&0&3\end{pmatrix},\qquad X=\begin{pmatrix}0&1&0\\0&0&3\\1&0&1\end{pmatrix},
$$

so

$$
Q^T=\begin{pmatrix}1&4&1\\1&1&4\\3&3&3\end{pmatrix}.
$$

For the second tableau, writing its $y$ and $r$ blocks as $Y,R$, the original equations $Py+r=\mathbf1$ give $P=R^{-1}Y$. We obtain

$$
R^{-1}=\begin{pmatrix}1&1&0\\0&4&0\\0&3&1\end{pmatrix},\qquad Y=\begin{pmatrix}3/4&15/4&0\\1/4&1/4&1\\9/4&9/4&0\end{pmatrix}.
$$

Thus a representative pair of [payoff matrices](../../../../../../payoff-matrix.md) is

$$
\boxed{P=\begin{pmatrix}1&4&1\\1&1&4\\3&3&3\end{pmatrix},\qquad Q=P^T=\begin{pmatrix}1&1&3\\4&1&3\\1&4&3\end{pmatrix}.}
$$

Both reconstructed right-hand sides are $\mathbf1$, as a check on the tableau normalization. Independent transformations $P\mapsto aP+b\mathbf1\mathbf1^T$, $Q\mapsto cQ+d\mathbf1\mathbf1^T$, with $a,c>0$, preserve [best responses](../../../../../../best-response.md) and hence identify the same strategic solution up to positive affine payoff transformations.

Directly,

$$
Py'=(1,3,3)^T,\qquad Q^Tx'=Px'=(3,2,3)^T.
$$

The supports of $x'$ and $y'$ lie entirely among their respective best-response coordinates, confirming the [Nash equilibrium](../../../../../../nash-equilibrium.md) found above. Since this representative is a [symmetric bimatrix game](../../../../../../symmetric-bimatrix-game.md), swapping the players' strategies preserves the [Nash equilibrium](../../../../../../nash-equilibrium.md) conditions. Explicitly, $Px'=(3,2,3)^T$ is maximized on the support of $y'$, and $Q^Ty'=Py'=(1,3,3)^T$ is maximized on the support of $x'$. Therefore

$$
\boxed{(y',x')\text{ is also a Nash equilibrium};\quad\text{both players' payoffs are }3\text{ in either profile}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
