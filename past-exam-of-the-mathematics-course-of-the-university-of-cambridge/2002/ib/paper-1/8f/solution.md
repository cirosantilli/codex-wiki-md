<h1 id="8f/solution">Solution</h1>

↑ **Parent:** [8F](../8f.md)

For a real [symmetric bilinear form](../../../../../symmetric-bilinear-form.md), a basis puts its quadratic expression in diagonal form with $p$ positive, $q$ negative and $r$ zero squares. Its rank is $p+q$, the rank of the coefficient matrix, or equivalently the codimension of its radical. Its [signature](../../../../../signature-of-a-quadratic-form.md) is $p-q$; the [signature pair](../../../../../signature-pair-of-a-real-symmetric-bilinear-form.md) is $(p,q)$, another common convention.

These quantities do not depend on the basis. A basis change replaces the matrix $M$ by $P^TMP$ with $P$ invertible, preserving matrix rank. The number $p$ is intrinsically the largest dimension of a subspace on which the form is positive definite. In a diagonal representation the positive coordinate space attains this dimension; any subspace of dimension greater than $p$ intersects the negative-plus-null coordinate space nontrivially and therefore cannot be positive definite. The same argument with signs reversed characterizes $q$. This proves the needed invariance, rather than assuming it from a chosen representation.

Decompose the full matrix space as

$$
M_n(\mathbb R)=\operatorname{Sym}_0(n)\oplus\operatorname{Skew}(n)\oplus\mathbb RI,
$$

using the symmetric traceless, skew-symmetric and scalar parts. The summands are orthogonal for the given form. Indeed $\operatorname{tr}(SK)=0$ for symmetric $S$ and skew-symmetric $K$, by transposition and cyclic invariance of [trace](../../../../../matrix-trace.md), while both non-scalar summands are traceless and hence orthogonal to $I$. On them,

$$
\phi(S,S)=\operatorname{tr}(S^2)=\|S\|_F^2>0,\quad\phi(K,K)=\operatorname{tr}(K^2)=-\|K\|_F^2<0,\quad\phi(tI,tI)=-n(n-1)t^2<0
$$

for nonzero vectors in their respective summands. The dimensions are $n(n+1)/2-1$, $n(n-1)/2$ and one. Therefore the [modified trace form on real matrices](../../../../../modified-trace-form-on-real-matrices.md) has

$$
\boxed{\operatorname{rank}\phi=n^2,\qquad\operatorname{signature}\phi=n-2},\qquad\boxed{(p,q)=\left(\frac{n(n+1)}2-1,\frac{n(n-1)}2+1\right)}.
$$

There is no radical for $n\geq2$.

## ↑ Ancestors (10)

1. [8F](../8f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
