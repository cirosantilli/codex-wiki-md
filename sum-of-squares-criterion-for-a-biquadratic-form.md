# Sum of squares criterion for a biquadratic form

↑ **Parent:** [Polynomial SOS](polynomial-sos.md)

For a real [symmetric matrix](symmetric-matrix.md) $A$, set $v(z)=(z_1^2,\ldots,z_n^2)^T$. Then

$$
v(z)^TAv(z)\text{ is a sum of squares}
\quad\Longleftrightarrow\quad
A=P+N,\quad P\succeq0,\quad N=N^T\geq0\text{ entrywise}.
$$

For sufficiency, factor $P=B^TB$. Its contribution is a sum of squares of linear combinations of $z_i^2$, while the contribution of $N$ is $\sum_i N_{ii}(z_i^2)^2+\sum_{i<j}2N_{ij}(z_iz_j)^2$. For necessity, use a [homogeneous sum of squares representation](homogeneous-sum-of-squares-representation.md) and [sign averaging of a sum of squares](sign-averaging-of-a-sum-of-squares.md). Writing each quadratic summand with coefficients $a_{\ell i},b_{\ell ij}$ gives $P=\sum_\ell a_\ell a_\ell^T$, $N_{ii}=0$ and $N_{ij}=\frac12\sum_\ell b_{\ell ij}^2$ for $i<j$. Comparing coefficients gives $A=P+N$.

This is the basic [semidefinite programming](semidefinite-programming.md) certificate of copositivity discussed in [Parrilo's paper on matrix copositivity](https://www.mit.edu/~parrilo/pubs/files/Parrilo-Semidefinite%20programming%20based%20tests%20for%20matrix%20copositivity.pdf).

## ↑ Ancestors (7)

1. [Polynomial SOS](polynomial-sos.md)
2. [Nonnegative polynomial](nonnegative-polynomial.md)
3. [Polynomial](polynomial-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-339/3/b/solution.md)
- [Positive-semidefinite-plus-nonnegative cone](positive-semidefinite-plus-nonnegative-cone.md)
