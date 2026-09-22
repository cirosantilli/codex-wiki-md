# Positive-diagonal QR decomposition preserves a complex structure

↑ **Parent:** [QR decomposition](qr-decomposition.md)

Let $K$ be block diagonal with $2\times2$ blocks $J=\begin{pmatrix}0&1\\-1&0\end{pmatrix}$. If a real invertible [matrix](matrix.md) $A$ commutes with $K$, its [QR decomposition](qr-decomposition.md) $A=BC$, with $B$ orthogonal and $C$ upper triangular with positive diagonal, has both $BK=KB$ and $CK=KC$. Indeed $CKC^{-1}=B^{-1}KB$, so $E=K^{-1}CKC^{-1}$ is orthogonal and upper triangular in $2\times2$ blocks. Orthogonality forces its off-diagonal blocks to vanish. Its diagonal blocks are $J^{-1}C_iJC_i^{-1}$. For $C_i=\begin{pmatrix}a&b\\0&d\end{pmatrix}$ with $a,d>0$, this block is $\begin{pmatrix}d/a&-b/a\\-b/a&(a^2+b^2)/(ad)\end{pmatrix}$. Orthogonality of its columns forces $b=0,d=a$, and hence each block is the identity. Thus $E=I$, proving the claim.

## ↑ Ancestors (8)

1. [QR decomposition](qr-decomposition.md)
2. [Gram-Schmidt process](gram-schmidt-process.md)
3. [Inner product](inner-product.md)
4. [Linear algebra](linear-algebra-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-3/19b/solution.md)
