<h1 id="9h/solution">Solution</h1>

↑ **Parent:** [9H](../9h.md)

In a two-player [zero-sum game](../../../../../zero-sum-game.md), the row player chooses a row, the column player chooses a column, and the row player's gain is the column player's loss. If their independent [mixed strategies](../../../../../mixed-strategy.md) are probability vectors $x\in\mathbb R^m$, $y\in\mathbb R^n$, the row player's expected payoff is $x^TPy$.

The [optimal mixed strategies](../../../../../optimal-mixed-strategy.md) solve

$$
x_*\in\operatorname*{arg\,max}_{x\ge0,\ \sum x_i=1}\min_j(x^TP)_j,\qquad
y_*\in\operatorname*{arg\,min}_{y\ge0,\ \sum y_j=1}\max_i(Py)_i.
$$

The [minimax theorem](../../../../../minimax-theorem.md) equates these two guaranteed values. Equivalently, for a value $v$, $x_*^TP\ge v\mathbf1^T$ and $Py_*\le v\mathbf1$ componentwise.

For a row strategy $(p,1-p)$, the payoffs against the two pure columns are $2-6p$ and $-4+6p$. Their minimum is maximized at their intersection, $p=1/2$, where both are $-1$. Symmetrically the column player's maximum of the two row payoffs is minimized at $q=1/2$. Hence

$$
\boxed{x_*=(1/2,1/2),\qquad y_*=(1/2,1/2),\qquad v=-1.}
$$

These probabilities are unique: moving either probability away from $1/2$ worsens that player's guaranteed payoff.

## ↑ Ancestors (10)

1. [9H](../9h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
