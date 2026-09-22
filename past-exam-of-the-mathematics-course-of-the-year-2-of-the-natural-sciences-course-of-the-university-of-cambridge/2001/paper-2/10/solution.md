<h1 id="10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

**Representations.** A complex [group representation](../../../../group-representation.md) is a [group homomorphism](../../../../group-homomorphism.md) $\rho:G\to\operatorname{GL}(W)$ to the invertible linear maps on a vector space. It is an [irreducible representation](../../../../irreducible-representation.md) when $W\ne0$ and the only invariant subspaces are $0$ and $W$.

**Group table.** The supplied matrices satisfy $A=-I$, $C=-B$, and $A^2=B^2=C^2=I$. Their [multiplication table](../../../../multiplication-table.md) is

$$
\boxed{\begin{array}{c|rrrr}
&I&A&B&C\\\hline
I&I&A&B&C\\
A&A&I&C&B\\
B&B&C&I&A\\
C&C&B&A&I
\end{array}.}
$$

The table proves closure and gives identity $I$ and an inverse for every element; associativity is inherited from [matrix multiplication](../../../../matrix-multiplication.md). The table is symmetric, so the [group](../../../../group-split.md) is abelian. It is the [Klein four-group](../../../../klein-four-group.md) $V\cong C_2\times C_2$.

**Dimensions and conjugacy.** The [sum of squares of irreducible representation dimensions](../../../../sum-of-squares-of-irreducible-representation-dimensions.md) is $|V|=4$. A two-dimensional irreducible would alone contribute four, leaving no room for the ever-present one-dimensional [trivial representation](../../../../trivial-representation.md). Hence the given two-dimensional representation is reducible. Since the [group](../../../../group-split.md) is abelian, every [conjugacy class](../../../../conjugacy-class.md) is a singleton. There are therefore four inequivalent complex [irreducible representations](../../../../irreducible-representation.md), each of dimension one:

$$
\boxed{\text{classes }\{I\},\{A\},\{B\},\{C\};\qquad\text{irreducible dimensions }1,1,1,1.}
$$

Taking the [trace](../../../../matrix-trace.md) of the given matrices gives their [character of a representation](../../../../character-of-a-representation.md):

$$
\boxed{\chi_{\rm given}(I,A,B,C)=(2,-2,0,0).}
$$

**Irreducible characters.** In a one-dimensional representation, the values on $A$ and $B$ must each be $\pm1$, since both elements square to $I$. Their values determine the value on $C=AB$. The four choices give the complete [character table](../../../../character-table.md):

$$
\boxed{\begin{array}{c|rrrr}
&I&A&B&C\\\hline
\chi_1&1&1&1&1\\
\chi_2&1&1&-1&-1\\
\chi_3&1&-1&1&-1\\
\chi_4&1&-1&-1&1
\end{array}.}
$$

Each row is a character because it respects the generating relations, and the rows have unit norm and pairwise zero [character inner product](../../../../character-inner-product.md). The multiplicities of these rows in $(2,-2,0,0)$ are respectively $0,0,1,1$, by [character orthogonality](../../../../character-orthogonality.md). Thus

$$
\boxed{\rho_{\rm given}\cong\rho_3\oplus\rho_4.}
$$

**Diagonal form.** The common invariant lines are spanned by $(1,1)^T$ and $(1,-1)^T$. Use their normalized vectors as columns of

$$
U=\frac1{\sqrt2}\begin{pmatrix}1&1\\1&-1\end{pmatrix},\qquad U^{-1}=U^T=U.
$$

Then simultaneous [diagonalization](../../../../diagonalization-of-a-matrix.md) gives

$$
\boxed{U^TIU=\begin{pmatrix}1&0\\0&1\end{pmatrix},\quad U^TAU=\begin{pmatrix}-1&0\\0&-1\end{pmatrix},\quad U^TBU=\begin{pmatrix}1&0\\0&-1\end{pmatrix},\quad U^TCU=\begin{pmatrix}-1&0\\0&1\end{pmatrix}.}
$$

Reading the first and second diagonal entries across the four matrices recovers $\chi_3$ and $\chi_4$, respectively, verifying the decomposition explicitly.

## ↑ Ancestors (12)

1. [10](../10.md)
2. [Paper 2](../../paper-2-split.md)
3. [2001](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
