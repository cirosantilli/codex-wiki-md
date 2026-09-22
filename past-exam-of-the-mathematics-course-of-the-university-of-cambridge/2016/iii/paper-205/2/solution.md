<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the normalization

$$
\boxed{\widehat\beta_\lambda=\mathop{\arg\min}_{\beta\in\mathbb R^p}\left\{\frac12\|Y-X\beta\|_2^2+\frac\lambda2\|\beta\|_2^2\right\}.}
$$

This is [ridge regression](../../../../../ridge-regression.md); the penalty is the squared [Euclidean norm](../../../../../euclidean-norm.md). The centering removes the need for an intercept. Differentiating gives the normal equation

$$
(X^TX+\lambda I_p)\widehat\beta_\lambda=X^TY.
$$

For every nonzero $v$, $v^T(X^TX+\lambda I_p)v=\|Xv\|_2^2+\lambda\|v\|_2^2>0$. The coefficient matrix is therefore a [positive-definite matrix](../../../../../positive-definite-matrix.md), even if the [design matrix](../../../../../design-matrix.md) has deficient [matrix rank](../../../../../matrix-rank.md). The objective is a [strictly convex function](../../../../../strictly-convex-function.md), so the unique minimizer is the [closed-form ridge regression estimator](../../../../../closed-form-ridge-regression-estimator.md), with fitted values

$$
\boxed{\widehat Y=X(X^TX+\lambda I_p)^{-1}X^TY.}
$$

For the [primal-dual identity for ridge regression](../../../../../primal-dual-identity-for-ridge-regression.md), put $K=XX^T$ and observe

$$
(X^TX+\lambda I_p)X^T=X^T(K+\lambda I_n).
$$

Both parenthesized matrices are [positive-definite matrices](../../../../../positive-definite-matrix.md). Multiplying by their inverses gives

$$
(X^TX+\lambda I_p)^{-1}X^T=X^T(K+\lambda I_n)^{-1}.
$$

Thus the same fitted vector has the dual expression

$$
\boxed{\widehat Y=K(K+\lambda I_n)^{-1}Y.}
$$

No inverse of $X^TX$ or $K$ alone was needed. This is also the [kernel-ridge hat matrix](../../../../../kernel-ridge-hat-matrix.md) for the [linear kernel](../../../../../linear-kernel.md).

Here a [positive-definite kernel](../../../../../positive-semidefinite-kernel.md) means a symmetric real-valued function $k$ whose every finite [kernel matrix](../../../../../kernel-matrix.md) is [positive semidefinite](../../../../../positive-semidefinite-matrix.md): for all $m$, $x_1,\ldots,x_m\in\mathcal X$ and $a_1,\ldots,a_m\in\mathbb R$,

$$
\sum_{i,j=1}^ma_ia_jk(x_i,x_j)\geq0.
$$

This is the usual [positive-semidefinite kernel](../../../../../positive-semidefinite-kernel.md) convention; strict positivity for distinct points is not required. In particular $k(x,x)\geq0$. Write $a=k(x,x)$, $b=k(x',x')$ and $r=k(x,x')$. Positivity of the two-point [kernel matrix](../../../../../kernel-matrix.md) implies

$$
a+2tr+t^2b\geq0\qquad(t\in\mathbb R).
$$

If $b>0$, substitute $t=-r/b$ to obtain $a-r^2/b\geq0$. If $b=0$, the affine expression $a+2tr$ can be nonnegative for every $t$ only if $r=0$. Both cases give the [Cauchy-Schwarz inequality for positive-semidefinite kernels](../../../../../cauchy-schwarz-inequality-for-positive-semidefinite-kernels.md):

$$
\boxed{k(x,x')^2\leq k(x,x)k(x',x').}
$$

The zero-diagonal case is essential when the [positive-definite kernel](../../../../../positive-semidefinite-kernel.md) is not strictly positive.

To construct a [feature map](../../../../../feature-map.md), let $F$ be the real [vector space](../../../../../vector-space-split.md) of finite formal linear combinations of symbols $e_x$, one for each $x\in\mathcal X$. Define a [symmetric bilinear form](../../../../../symmetric-bilinear-form.md) by

$$
B\left(\sum_i a_i e_{x_i},\sum_j b_j e_{y_j}\right)=\sum_{i,j}a_ib_jk(x_i,y_j).
$$

The [positive-definite kernel](../../../../../positive-semidefinite-kernel.md) property makes this a [positive semidefinite bilinear form](../../../../../positive-semidefinite-bilinear-form.md). It need not yet be an [inner product](../../../../../inner-product.md): distinct formal vectors can have zero squared length. The same quadratic-polynomial argument, now applied to $B(u+tv,u+tv)$, proves

$$
|B(u,v)|^2\leq B(u,u)B(v,v).
$$

Therefore $B(u,u)=0$ implies $B(u,v)=0$ for every $v$. The set

$$
N=\{u\in F:B(u,u)=0\}=\{u\in F:B(u,v)=0\text{ for every }v\in F\}
$$

is the [radical of a bilinear form](../../../../../radical-of-a-bilinear-form.md), hence a [linear subspace](../../../../../vector-subspace.md). Set

$$
\mathcal H=F/N,\qquad\langle u+N,v+N\rangle=B(u,v).
$$

The [quotient vector space](../../../../../quotient-vector-space.md) has a well-defined [inner product](../../../../../inner-product.md): changing representatives by elements of $N$ changes no pairing, and a zero-length class is exactly the zero class. It is therefore an [inner product space](../../../../../inner-product-space.md).

Define $\phi(x)=e_x+N$. By construction,

$$
\boxed{\langle\phi(x),\phi(x')\rangle=B(e_x,e_{x'})=k(x,x').}
$$

**Every positive-definite kernel thus has a feature representation**, including degenerate kernels and the zero kernel. This is its [canonical feature space of a positive-semidefinite kernel](../../../../../canonical-feature-space-of-a-positive-semidefinite-kernel.md). The construction already gives the requested [inner product space](../../../../../inner-product-space.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
