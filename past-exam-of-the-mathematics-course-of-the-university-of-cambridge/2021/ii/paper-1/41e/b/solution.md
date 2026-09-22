<h1 id="41e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**False under the hypotheses as printed.** Nonzero coefficients do not ensure the [two-column dominant-subspace condition](../../../../../../two-column-dominant-subspace-condition.md).

For a counterexample, take $n=3$, eigenvalues

$$
(\lambda_1,\lambda_2,\lambda_3)=(1,2,-2),
$$

and an orthonormal eigenbasis $w_1,w_2,w_3$ for which

$$
e_1=\frac{-2w_1+w_2+w_3}{\sqrt6},
\qquad
e_2=\frac{w_1+w_2+w_3}{\sqrt3}.
$$

The two displayed coefficient vectors are orthonormal and can be completed to an [orthogonal matrix](../../../../../../orthogonal-matrix.md), so such a real [symmetric matrix](../../../../../../symmetric-matrix.md) $A$ exists. Every $b_i$ and $c_i$ is nonzero, but

$$
b_2c_3-b_3c_2=0.
$$

Indeed, with $t=1/\sqrt2$,

$$
A^ke_1-tA^ke_2
$$

is a nonzero multiple of $w_1$, while the remaining direction in  
$\operatorname{span}(A^ke_1,A^ke_2)$ is

$$
v_k=\frac{w_2+(-1)^kw_3}{\sqrt2}.
$$

Thus

$$
\operatorname{span}(A^ke_1,A^ke_2)
=\operatorname{span}(w_1,v_k).
$$

By the [simultaneous iteration interpretation of the QR algorithm](../../../../../../simultaneous-iteration-interpretation-of-the-qr-algorithm.md), the leading two columns of the accumulated $Q$ factor span this same space. The leading block $B_k$ is therefore an orthogonal-coordinate representation of the [compression](../../../../../../compression-of-a-linear-operator.md) of $A$ to this space. Since

$$
w_1^TAw_1=1,
\qquad
v_k^TAv_k=\frac{2+(-2)}2=0,
\qquad
w_1^TAv_k=0,
$$

we have

$$
\operatorname{Spec}(B_k)=\{0,1\}
$$

for every relevant $k$, rather than $\{-2,2\}$. Hence the requested [Hausdorff convergence](../../../../../../hausdorff-distance.md) does not hold.

For completeness, the intended statement becomes true if one adds

$$
\Delta=b_{n-1}c_n-b_nc_{n-1}\ne0.
$$

Let $Z_k$ consist of the first two columns of $\overline Q_{k-1}$. The [Accumulated QR factorization identity](../../../../../../accumulated-qr-factorization-identity.md) gives

$$
\operatorname{col}(Z_k)
=\operatorname{span}(A^ke_1,A^ke_2).
$$

After division by $|\lambda_n|^k$, every component along  
$w_1,\ldots,w_{n-2}$ tends to zero because of the strict [spectral gap](../../../../../../spectral-gap.md), while $\Delta\ne0$ makes the two surviving dominant components independent. Therefore these two-dimensional subspaces converge to the [dominant invariant subspace](../../../../../../dominant-invariant-subspace.md)

$$
E=\operatorname{span}(w_{n-1},w_n).
$$

There are two-by-two orthogonal matrices $U_k$ such that

$$
Z_kU_k\longrightarrow W_*=(w_{n-1},w_n).
$$

Because

$$
B_k=Z_k^TAZ_k,
$$

up to the harmless index convention at $k=0$, we obtain

$$
U_k^TB_kU_k
\longrightarrow
W_*^TAW_*
=\operatorname{diag}(\lambda_{n-1},\lambda_n)
$$

in the [matrix 2-norm](../../../../../../matrix-2-norm.md). Orthogonal similarity preserves the [spectrum](../../../../../../spectrum-functional-analysis.md), and the stated spectral perturbation bound now gives

$$
\boxed{d_H\!\left(\operatorname{Spec}(B_k),
\{\lambda_{n-1},\lambda_n\}\right)\longrightarrow0.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [41E](../../41e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
