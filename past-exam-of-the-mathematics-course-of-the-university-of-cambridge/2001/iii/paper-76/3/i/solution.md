<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The sumset form of [Plünnecke's inequality](../../../../../../plunnecke-inequality.md) states: for nonempty finite sets $A,B$ in an [abelian group](../../../../../../abelian-group.md), if $|A+B|\le K|A|$, there is a nonempty $X\subseteq A$ such that

$$
\boxed{|X+mB|\le K^m|X|\quad\text{for every integer }m\ge0.}
$$

Here $0B=\{0\}$. The same $X$ can be used for every $m$. This sumset statement follows from an elementary minimal-growth argument.

Choose $X$ minimizing $\kappa=|X+B|/|X|$ among nonempty subsets of $A$. Then $\kappa\le K$ and $|Y+B|\ge\kappa|Y|$ for every $Y\subseteq X$, including the empty set. We prove the [Petridis minimal-growth lemma](../../../../../../petridis-minimal-growth-lemma.md)

$$
|X+B+C|\le\kappa|X+C|
$$

for each finite set $C$. Enumerate $C=\{c_1,\ldots,c_t\}$. Put $C_i=\{c_1,\ldots,c_i\}$ and define

$$
X_i=\{x\in X:x+c_i\notin X+C_{i-1}\},\qquad Y_i=X\setminus X_i.
$$

The disjoint new contributions to $X+C$ have sizes $|X_i|$, so $|X+C|=\sum_i|X_i|$. For $y\in Y_i$, the point $y+c_i$ was already present in $X+C_{i-1}$, hence $y+B+c_i\subseteq X+B+C_{i-1}$. Consequently the new contribution at stage $i$ to $X+B+C$ has size at most

$$
|X+B|-|Y_i+B|\le\kappa|X|-\kappa|Y_i|=\kappa|X_i|.
$$

Summing proves the lemma. Starting with $C=\{0\}$ and then taking $C=(m-1)B$ gives inductively $|X+mB|\le\kappa^m|X|\le K^m|X|$, proving the stated [Plünnecke inequality](../../../../../../plunnecke-inequality.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
