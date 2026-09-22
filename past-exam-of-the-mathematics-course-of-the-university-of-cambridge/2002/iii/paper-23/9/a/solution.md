<h1 id="9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For an unrestricted binary relation $R$, the extension axioms permit arbitrary directed edges and loops. For each $m\ge0$ and each choice of bits $\epsilon_i,\delta_i,\eta\in\{0,1\}$, require that every tuple of distinct $x_1,\ldots,x_m$ has a fresh element $y$ with

$$
y\ne x_i\quad\text{for all }i,\qquad
R(y,y)^\eta\land\bigwedge_{i=1}^m
\bigl(R(y,x_i)^{\epsilon_i}\land R(x_i,y)^{\delta_i}\bigr).
$$

Here $P^1$ denotes $P$ and $P^0$ denotes $\neg P$; the notation is a literal abbreviation, not exponentiation of a relation. Incoming and outgoing choices are independent, and the loop bit is also specified. These are the [extension axioms for an unrestricted binary relation](../../../../../../extension-axioms-for-an-unrestricted-binary-relation.md). If one instead restricts to undirected loop-free graphs, the allowable patterns reduce to the random-graph extension axioms of Question 2; no such restriction is imposed here.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9](../../9.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
