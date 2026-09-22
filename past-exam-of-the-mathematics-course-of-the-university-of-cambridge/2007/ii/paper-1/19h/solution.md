<h1 id="19h/solution">Solution</h1>

↑ **Parent:** [19H](../19h.md)

Put $w_j=|C_j|/|G|$. The [character orthogonality](../../../../../character-orthogonality.md) for the five supplied rows say $\sum_jw_j\chi_r(C_j)\chi_s(C_j)=\delta_{rs}$. Solving these linear equations gives

$$
(w_1,\ldots,w_7)=\frac1{120}(1,15,20,24,10,20,30).
$$

For example orthogonality of the two degree-four rows gives $16w_1+w_3+w_4-4w_5-w_6=0$, and their norms give $16w_1+w_3+w_4+4w_5+w_6=1$; the remaining row products determine the other weights. Since $C_1=\{e\}$, $w_1=1/|G|$, so **$|G|=120$** and the class sizes are the displayed numerators.

Tensoring the fifth [irreducible representation](../../../../../irreducible-representation.md) with the second, one-dimensional one gives another [irreducible character](../../../../../irreducible-character.md), with row $(5,1,-1,0,-1,-1,1)$. It differs from all five known rows. There are seven [conjugacy classes](../../../../../conjugacy-class.md), hence seven [irreducible characters](../../../../../irreducible-character.md). The sum of squared degrees is $|G|$, so the final degree is $\sqrt{120-(1+1+16+16+25+25)}=6$.

The [regular representation](../../../../../regular-representation.md) has character zero off the identity and is the sum of irreducible characters weighted by their degrees. Applying this column by column determines the last row. The completed [character table](../../../../../character-table.md), in the supplied class order, is

$$
\boxed{\begin{array}{c|rrrrrrr}
|C_j|&1&15&20&24&10&20&30\\\hline
\chi_1&1&1&1&1&1&1&1\\
\chi_2&1&1&1&1&-1&-1&-1\\
\chi_3&4&0&1&-1&2&-1&0\\
\chi_4&4&0&1&-1&-2&1&0\\
\chi_5&5&1&-1&0&1&1&-1\\
\chi_6&5&1&-1&0&-1&-1&1\\
\chi_7&6&-2&0&1&0&0&0
\end{array}.}
$$

No identification of the group with a familiar group is needed.

## ↑ Ancestors (10)

1. [19H](../19h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
