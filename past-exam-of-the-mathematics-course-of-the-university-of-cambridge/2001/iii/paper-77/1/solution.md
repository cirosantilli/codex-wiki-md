<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use nonnegative integer [matrix](../../../../../matrix.md) entries, including zero, and English [Young diagram](../../../../../young-diagram.md) conventions: rows run left to right and columns run down. Replace $A$ by a two-line array containing $a_{ij}$ copies of $\binom ij$, sorted lexicographically by upper letter $i$ and then lower letter $j$. Finite support makes the array finite.

In the [RSK algorithm](../../../../../robinson-schensted-knuth-correspondence.md), insert each lower letter $j$ into $P$ by [row insertion](../../../../../row-insertion.md). In the first row replace the leftmost entry strictly greater than $j$, carrying the replaced entry into the next row; if there is no such entry, append $j$ and stop. Repeat in subsequent rows until a new cell is made. Put the upper letter $i$ in that new cell of the recording tableau $Q$.

The insertion-path facts used here are the following: [row insertion](../../../../../row-insertion.md) preserves weak rows and strict columns; inserting $u$ followed by $v\ge u$ puts the latter new cell strictly to the right of the former; reverse insertion undoes insertion; and the reverse paths from a right-to-left horizontal strip recover its input letters in weakly decreasing order. These standard path facts ensure that $P$ is a [semistandard Young tableau](../../../../../semistandard-young-tableau.md). The upper letters are nondecreasing, so the entries of $Q$ are weakly increasing in rows. Equal upper letters have sorted lower letters, and hence create a [horizontal strip](../../../../../horizontal-strip.md); they cannot occupy the same column. Thus $Q$ is also a [semistandard Young tableau](../../../../../semistandard-young-tableau.md), of exactly the same shape as $P$.

Here is the inverse on any such pair. Select a largest entry $i$ in $Q$, and among the cells carrying it select the rightmost one. It is an outer corner: there can be no larger entry below it, and any entry to its right would be another maximal entry farther right. Delete that cell from $Q$ and reverse-insert the value at its cell in $P$. In each preceding row replace the rightmost entry strictly smaller than the carried value and carry that old entry upward. The value emerging from the first row is $j$. Record $\binom ij$ and repeat. Equal maximal entries form a [horizontal strip](../../../../../horizontal-strip.md), so the reverse-path fact gives their $j$'s in weakly decreasing order. Reversing the recovered list therefore gives exactly a lexicographically sorted two-line array. The procedures are mutually inverse, proving the [RSK correspondence](../../../../../robinson-schensted-knuth-correspondence.md) [bijection](../../../../../bijection.md), including the zero [matrix](../../../../../matrix.md) and the pair of empty tableaux.

Insertion only moves previous entries and adds one copy of its new letter; recording adds one copy of its upper letter. Consequently

$$
\boxed{\operatorname{content}_j(P)=\sum_i a_{ij},
\qquad \operatorname{content}_i(Q)=\sum_j a_{ij}.}
$$

For the trace assertion, use the insertion-path form of the [RSK growth-diagram local rule](../../../../../rsk-growth-diagram-local-rule.md). Let $\rho,\mu,\nu,\lambda$ be the shapes from the northwest, northeast, southwest and southeast [matrix](../../../../../matrix.md) prefixes around entry $a_{ij}$. Padding row lengths with zeros, the rule is

$$
\lambda_1=\max(\mu_1,\nu_1)+a_{ij},\qquad
\lambda_r=\max(\mu_r,\nu_r)+\min(\mu_{r-1},\nu_{r-1})-\rho_{r-1}\quad(r\ge2).
$$

This local rule counts the two merging insertion paths row by row: the entry supplies the initial carry, the longer extension supplies the current row, and the overlap of the extensions beyond $\rho$ is bumped to the next row. It is a standard insertion-path fact being used in addition to the preceding monotonicity statements.

Define $o(\gamma)=\gamma_1-\gamma_2+\gamma_3-\cdots$. Each column of the [Young diagram](../../../../../young-diagram.md) contributes its alternating vertical sum, which is one for odd length and zero for even length. Thus $o(\gamma)$ counts odd-length columns. For symmetric $A$, [transposition](../../../../../transposition-permutation.md) symmetry of [RSK](../../../../../robinson-schensted-knuth-correspondence.md) gives equal shapes for the two prefixes off the diagonal, so $\mu=\nu$ at entry $a_{ii}$. The rule becomes

$$
\lambda_1=\mu_1+a_{ii},\qquad
\lambda_r=\mu_r+\mu_{r-1}-\rho_{r-1}.
$$

Taking alternating sums makes the two sums involving $\mu$ cancel, leaving

$$
o(\lambda)=o(\rho)+a_{ii}.
$$

Starting from the empty northwest corner and proceeding along the diagonal proves the [trace and odd columns in symmetric RSK](../../../../../trace-and-odd-columns-in-symmetric-rsk.md) identity

$$
\boxed{\operatorname{tr}A=o(\operatorname{shape}P)
=\#\{\text{odd-length columns of }P\}.}
$$

This also accommodates arbitrary diagonal entries, rather than only [permutation matrices](../../../../../permutation-matrix.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 77](../../paper-77-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
