# Iterative spreadsheet calculation

↑ **Parent:** [Spreadsheet circular reference](spreadsheet-circular-reference.md)

A different interpretation can treat cyclic [spreadsheet formulas](spreadsheet-formula.md) as simultaneous equations and seek a [fixed point](fixed-point.md) by repeated numerical updates. This requires an explicit update rule, initial values and stopping condition. It is not automatically the meaning of a [spreadsheet formula](spreadsheet-formula.md). In particular, a [directed cycle](directed-cycle.md) alone tells us neither whether a [fixed point](fixed-point.md) exists nor whether a chosen update rule approaches it.

Two original toy examples make the distinction exact. The cyclic pair `X1=Y1+1`, `Y1=X1+1` has no solution over the [real numbers](real-number.md): substitution gives $X1=X1+2$. For `X1=Y1`, `Y1=X1`, every equal pair is a [fixed point](fixed-point.md), so there is no unique answer. Simultaneously updating both [spreadsheet cells](spreadsheet-cell.md) from the previous pair gives $(x_{n+1},y_{n+1})=(y_n,x_n)$. Starting at $(0,1)$ produces the [periodic sequence](periodic-sequence.md) $(0,1),(1,0),(0,1),\ldots$, which does not approach a [fixed point](fixed-point.md). Updating `X1` first and immediately using its new value for `Y1` instead gives $(1,1)$ in one sweep. That difference follows from the specified rules, not from a claim about any current spreadsheet product. Numerical iteration can be useful for a deliberately chosen model with a justification such as the [contraction mapping theorem](contraction-mapping-theorem.md); ordinary acyclic [spreadsheet dependency evaluation](spreadsheet-dependency-evaluation.md) already has its answer from prerequisite order.

## ↑ Ancestors (6)

1. [Spreadsheet circular reference](spreadsheet-circular-reference.md)
2. [Spreadsheet dependency graph](spreadsheet-dependency-graph.md)
3. [Spreadsheet dependency evaluation](spreadsheet-dependency-evaluation.md)
4. [Spreadsheet](spreadsheet-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)
