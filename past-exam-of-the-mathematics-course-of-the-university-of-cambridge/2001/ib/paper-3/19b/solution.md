<h1 id="19b/solution">Solution</h1>

↑ **Parent:** [19B](../19b.md)

First write $T=\begin{pmatrix}a&b\\0&d\end{pmatrix}$ with $a,d>0$. Direct multiplication gives

$$
E=J_1^{-1}TJ_1T^{-1}=\begin{pmatrix}d/a&-b/a\\-b/a&(a^2+b^2)/(ad)\end{pmatrix}.
$$

The [inner product](../../../../../inner-product.md) of its two columns is

$$
-\frac b{a^2}\left(d+\frac{a^2+b^2}{d}\right).
$$

If $E$ is orthogonal this is zero, and positivity of the bracket forces $b=0$. The first column must then have length one, so $d/a=1$. Thus $T=aI$, $E=I$, and $J_1T=TJ_1$.

For the general [QR decomposition](../../../../../qr-decomposition.md), apply the [Gram-Schmidt process](../../../../../gram-schmidt-process.md) to the ordered columns $v_1,\ldots,v_N$ of the invertible real [matrix](../../../../../matrix.md) $A$. At stage $j$, subtract projections onto the already chosen orthonormal vectors to get $u_j$; independence of the columns gives $u_j\ne0$. Set $q_j=u_j/\|u_j\|$. The [matrix](../../../../../matrix.md) $B$ with columns $q_j$ is orthogonal, and

$$
C=B^TA,\qquad C_{ij}=q_i\cdot v_j,
$$

is upper triangular. Its diagonal entry $C_{jj}=\|u_j\|$ is strictly positive. This proves $A=BC$ with the required properties.

Now suppose $KA=AK$ in dimension $2n$. Substitution of $A=BC$ gives

$$
CKC^{-1}=B^{-1}KB.
$$

The [matrix](../../../../../matrix.md) $K$ is orthogonal, as are $B$ and $B^{-1}$, so this matrix and $E=K^{-1}CKC^{-1}$ are orthogonal. Regard $C$ as upper triangular in $2\times2$ blocks, with invertible diagonal blocks $C_i$. The inverse is upper triangular in the same blocks, by solving the triangular block equations; multiplication by block diagonal $K$ preserves this pattern. Thus $E$ is block upper triangular.

An orthogonal block upper-triangular matrix is block diagonal. Indeed its first two columns are supported in the first two rows and are orthonormal, so span that first coordinate plane. Orthogonality of every subsequent column to them makes its first two entries zero. The remaining lower-right matrix is orthogonal; iterate this argument. Therefore $E=\operatorname{diag}(E_1,\ldots,E_n)$ with each $E_i$ orthogonal. The rule for diagonal blocks of products of block upper-triangular matrices gives

$$
E_i=J_1^{-1}C_iJ_1C_i^{-1}.
$$

Each $C_i$ is itself an upper-triangular real $2\times2$ matrix with positive diagonal. The first calculation gives $E_i=I$. Consequently $E=I$, whence $CK=KC$. Finally $B=AC^{-1}$ is a product of matrices commuting with $K$, so $BK=KB$. We have proved

$$
\boxed{KC=CK,\qquad KB=BK.}
$$

This is [positive-diagonal QR decomposition preserves a complex structure](../../../../../positive-diagonal-qr-decomposition-preserves-a-complex-structure.md); the positivity convention is important in the two-dimensional step.

## ↑ Ancestors (10)

1. [19B](../19b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
