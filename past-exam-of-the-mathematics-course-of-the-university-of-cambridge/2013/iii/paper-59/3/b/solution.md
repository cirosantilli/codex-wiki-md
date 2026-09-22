<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For each fixed input length, take the complete truth table of the language. For every accepted string $z\in\{0,1\}^n$, form the minterm

$$
M_z(x)=\bigwedge_{i=1}^n\begin{cases}x_i,&z_i=1,\\\neg x_i,&z_i=0.\end{cases}
$$

An OR of these minterms equals the [indicator function](../../../../../../indicator-function.md), since $M_z(x)=1$ precisely at $x=z$. This is the [truth-table upper bound for circuit size](../../../../../../truth-table-upper-bound-for-circuit-size.md).

Generate the $n$ negated input wires once and share them. With $m\leq2^n$ accepted strings, use at most $m(n-1)$ binary AND gates and $m-1$ binary OR gates, besides the [negations](../../../../../../negation.md). Empty truth tables use a constant-zero [Boolean circuit](../../../../../../boolean-circuit.md); length zero is handled by a constant [Boolean circuit](../../../../../../boolean-circuit.md). Thus

$$
\boxed{L\in\mathrm{SIZE}(O(n2^n))\quad\text{for every }L\subseteq\{0,1\}^*}.
$$

This is an existence bound for a nonuniform [circuit family](../../../../../../circuit-family.md), even when the language is [undecidable](../../../../../../undecidable-decision-problem.md). It supplies no algorithm for computing the truth tables of an arbitrary language.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
