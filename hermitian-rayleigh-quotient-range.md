# Hermitian Rayleigh quotient range

↑ **Parent:** [Rayleigh quotient](rayleigh-quotient.md)

For a finite-dimensional [Hermitian matrix](hermitian-operator.md) $A$, the [Rayleigh quotient](rayleigh-quotient.md) has precisely the range $[\lambda_{\min},\lambda_{\max}]$, where the endpoints are its extreme [eigenvalues](eigenvalue.md). The [finite-dimensional spectral theorem](finite-dimensional-spectral-theorem.md) writes a nonzero [vector](vector.md) as $x=\sum_jc_je_j$ in an [orthonormal eigenbasis](orthonormal-eigenbasis.md), giving

$$
R_A(x)=\sum_j\lambda_jw_j,\qquad
w_j=\frac{|c_j|^2}{\sum_k|c_k|^2},\qquad
w_j\geq0,\quad\sum_jw_j=1.
$$

Thus the quotient is a [convex combination](convex-combination.md) of [eigenvalues](eigenvalue.md). The bounds follow immediately, and equality at either endpoint means that $x$ lies in the corresponding extreme [eigenspace](eigenspace.md), including any repeated [eigenvalue](eigenvalue.md). Every intermediate value occurs: for orthonormal extreme [eigenvectors](eigenvector.md), $x=\sqrt{1-t}\,e_{\min}+\sqrt t\,e_{\max}$ gives $R_A(x)=(1-t)\lambda_{\min}+t\lambda_{\max}$ for $0\leq t\leq1$. If all [eigenvalues](eigenvalue.md) are equal, the quotient is constant.

The Hermitian hypothesis matters. The real [matrix](matrix.md) $B=\begin{pmatrix}1&4\\0&1\end{pmatrix}$ has only the [eigenvalue](eigenvalue.md) $1$, but $(1,1)B(1,1)^T/2=3$. Its quotient is governed by the [symmetric part of a matrix](symmetric-part-of-a-matrix.md) $(B+B^T)/2$, not by a real [orthonormal eigenbasis](orthonormal-eigenbasis.md) of $B$. A nonsymmetric [matrix](matrix.md) therefore need not obey the displayed eigenvalue bounds.

## ↑ Ancestors (7)

1. [Rayleigh quotient](rayleigh-quotient.md)
2. [Operator theory](linear-operator-theory-split.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Finite-dimensional spectral theorem](finite-dimensional-spectral-theorem.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-1/7a/c/solution.md)
- [Rayleigh quotient](rayleigh-quotient.md)
