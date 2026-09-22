<h1 id="19g/solution">Solution</h1>

↑ **Parent:** [19G](../19g.md)

There are seven [irreducible characters](../../../../../irreducible-character.md), one for each [conjugacy class](../../../../../conjugacy-class.md). Besides the trivial character and the four supplied rows, let the remaining degrees be $d,e$. The sum of squared degrees gives $d^2+e^2=360-(1+25+64+64+100)=106$, whose positive integer solutions are $\{d,e\}=\{5,9\}$. Complex conjugation permutes [irreducible characters](../../../../../irreducible-character.md) while preserving degree; the known rows are real and each unknown degree occurs just once among the remaining characters, so the two missing characters are real.

Call their entries $x_j,y_j$, with degrees five and nine. Orthogonality with the regular character gives $5x_j+9y_j=-\sum_{\rm known}\chi(1)\chi(C_j)$ for $j>1$. Column norms give $x_j^2+y_j^2=360/|C_j|-\sum_{\rm known}\chi(C_j)^2$. These equations yield two possible rational pairs in some columns. For this [integral character reconstruction from column orthogonality](../../../../../integral-character-reconstruction-from-column-orthogonality.md), a further constraint is essential: character values are [algebraic integers](../../../../../algebraic-integer.md), so rational candidates must be integers. For example at $C_6$, $5x+9y=-9$ and $x^2+y^2=1$ allow $(0,-1)$ and $(-45/53,-28/53)$; the second pair is not integral. The integral choices complete the table:

$$
\boxed{\begin{array}{c|rrrrrrr}
& C_1&C_2&C_3&C_4&C_5&C_6&C_7\\\hline
1&1&1&1&1&1&1&1\\
5&5&1&2&-1&-1&0&0\\
5&5&1&-1&2&-1&0&0\\
8&8&0&-1&-1&0&(1-\sqrt5)/2&(1+\sqrt5)/2\\
8&8&0&-1&-1&0&(1+\sqrt5)/2&(1-\sqrt5)/2\\
9&9&1&0&0&1&-1&-1\\
10&10&-2&1&1&0&0&0
\end{array}}
$$

Every nontrivial row has $\chi(g)\ne\chi(1)$ for $g\ne1$. In a unitary realization, $\chi(g)=\chi(1)$ exactly when all eigenvalues of the representing matrix are one, so each nontrivial irreducible representation is faithful. If a nontrivial proper [normal subgroup](../../../../../normal-subgroup.md) existed, a nontrivial irreducible representation of the nontrivial quotient would pull back to a nontrivial representation with that subgroup in its kernel. This contradicts faithfulness. **The group is simple.**

## ↑ Ancestors (10)

1. [19G](../19g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
