<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $W_n(i,j)$ for the number of [locally admissible words](../../../../../../locally-admissible-word-for-a-transition-matrix.md) $(x_0,\ldots,x_n)$ with $x_0=i$ and $x_n=j$. Here local admissibility means $A_{x_rx_{r+1}}=1$ for each consecutive pair; length counts symbols, so there are $n$ transitions. For $n=0$, the single-symbol word gives $W_0(i,j)=\delta_{ij}=(A^0)_{ij}$, and for $n=1$ we have $W_1(i,j)=A_{ij}$.

To append the last symbol $j$, choose the penultimate symbol $k$. Every choice gives a [locally admissible word](../../../../../../locally-admissible-word-for-a-transition-matrix.md) exactly when its length-$n$ prefix is locally admissible and $A_{kj}=1$. Different prefixes or penultimate symbols give different words, and every admissible word is obtained once. Therefore

$$
W_{n+1}(i,j)=\sum_{k=1}^m W_n(i,k)A_{kj}.
$$

This is precisely the rule for [matrix multiplication](../../../../../../matrix-multiplication.md). [Mathematical induction](../../../../../../mathematical-induction.md) consequently gives

$$
\boxed{W_n(i,j)=(A^n)_{ij}.}
$$

Equivalently, expanding the [matrix](../../../../../../matrix.md) entry sums the products $A_{ix_1}A_{x_1x_2}\cdots A_{x_{n-1}j}$ over all intermediate symbols; each product is the [indicator function](../../../../../../indicator-function.md) of one allowed transition chain.

**The intended meaning of “allowed” here is local admissibility.** If instead it means a word that actually occurs in some two-sided [sequence](../../../../../../sequence.md) in $\Sigma_A$, the assertion needs an additional extension assumption. For example, $A=\begin{pmatrix}0&1\\0&0\end{pmatrix}$ permits the word $(1,2)$ and has $(A)_{12}=1$, but $\Sigma_A$ is empty because no symbol can continue after $2$. Having a nonzero entry in every row and every column is sufficient: one can successively choose a predecessor and a successor to extend every [locally admissible word](../../../../../../locally-admissible-word-for-a-transition-matrix.md) indefinitely in both directions. No such assumption is needed for the local counting formula.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
