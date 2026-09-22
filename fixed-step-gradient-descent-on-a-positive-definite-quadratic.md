# Fixed-step gradient descent on a positive-definite quadratic

↑ **Parent:** [Gradient descent](gradient-descent-split.md)

Consider the original two-dimensional example

$$
f(x_1,x_2)=\frac12(x_1^2+9x_2^2),\qquad x_0=(2,1)^T,\qquad \nabla f(x)=(x_1,9x_2)^T.
$$

The [Hessian matrix](hessian-matrix.md) is $A=\operatorname{diag}(1,9)$, a [symmetric matrix](symmetric-matrix.md) and [positive-definite matrix](positive-definite-matrix.md). Its [eigenvectors](eigenvector.md) are the coordinate directions, its [eigenvalues](eigenvalue.md) are $1$ and $9$, and its [Euclidean norm](euclidean-norm.md) [condition number](condition-number.md) is $9$. The unique [global minimum](global-minimum.md) is $x_*=0$, so the error $e_k=x_k-x_*$ equals $x_k$. The [linear map](linear-map.md) $I-\eta A$, with $I$ the [identity matrix](identity-matrix.md), gives

$$
x_{1,k}=2(1-\eta)^k,\qquad x_{2,k}=(1-9\eta)^k.
$$

For $\eta=1/5=0.2$, the two coordinate error multipliers are $0.8$ and $-0.8$. Consequently $x_1=(1.6,-0.8)^T$, $x_2=(1.28,0.64)^T$, and the second coordinate changes sign at every step while both shrink. The [Euclidean norm](euclidean-norm.md) of the error contracts by $0.8$ each step. The objective gap, which we call the quadratic energy, contracts by its square:

$$
E_k=f(x_k)-f(x_*)=\frac{13}{2}\left(\frac{16}{25}\right)^k,\qquad E_0=6.5,\quad E_1=4.16,\quad E_2=2.6624.
$$

The [level sets](level-set.md) of $f$ are [ellipses](ellipse.md). Oscillation across their narrow direction is compatible with strictly decreasing energy.

<a id="image-original-gradient-descent-iterates-on-f-x-1-2-plus-9x-2-2-2-step-size-0-2-contracts-both-directions-whereas-0-25-expands-the-second"></a>
![](gradient-descent-quadratic-contour-iterates.png)

**[Figure 1](#image-original-gradient-descent-iterates-on-f-x-1-2-plus-9x-2-2-2-step-size-0-2-contracts-both-directions-whereas-0-25-expands-the-second). Original gradient descent iterates on $f=(x_1^2+9x_2^2)/2$: step size $0.2$ contracts both directions, whereas $0.25$ expands the second**.

For $\eta=1/4=0.25$, the coordinate error multipliers become $0.75$ and $-1.25$, giving $x_1=(1.5,-1.25)^T$. The first coordinate still tends to zero, but the second alternates and grows. Direct substitution gives

$$
E_k=2\left(\frac9{16}\right)^k+\frac92\left(\frac{25}{16}\right)^k,\qquad E_1=\frac{261}{32}=8.15625.
$$

Thus a larger positive [step size](step-size.md) can turn a strictly [convex function](convex-function.md) into a divergent iteration. Energy and error are different quantities: coordinate errors carry signed multipliers, while each coordinate's contribution to energy carries the squared multiplier.

<a id="image-exact-constructed-quadratic-energy-histories-from-2-1-step-sizes-0-1-and-0-2-converge-while-0-25-diverges"></a>
![](gradient-descent-quadratic-energy-histories.png)

**[Figure 2](#image-exact-constructed-quadratic-energy-histories-from-2-1-step-sizes-0-1-and-0-2-converge-while-0-25-diverges). Exact constructed quadratic-energy histories from $(2,1)$: step sizes $0.1$ and $0.2$ converge, while $0.25$ diverges**.

For the general [quadratic form](quadratic-form-split.md) with linear term

$$
f(x)=\frac12x^TAx-b^Tx,\qquad A=A^T>0,\qquad x_*=A^{-1}b,
$$

the error obeys the same [linear map](linear-map.md) $e_{k+1}=(I-\eta A)e_k$. The [spectral theorem for real symmetric matrices](spectral-theorem-for-real-symmetric-matrices.md) supplies an [orthonormal basis](orthonormal-basis.md) of [eigenvectors](eigenvector.md) $q_i$ with positive [eigenvalues](eigenvalue.md) $\lambda_i$. Writing $e_0=\sum_i c_iq_i$ gives the exact solution and energy identity

$$
e_k=\sum_i c_i(1-\eta\lambda_i)^kq_i,\qquad
E_k=\frac12\sum_i\lambda_i c_i^2(1-\eta\lambda_i)^{2k}.
$$

Therefore convergence from every initial [vector](vector.md) is equivalent to

$$
|1-\eta\lambda_i|<1\quad\text{for every }i,
\qquad\text{or equivalently}\qquad 0<\eta<\frac2{\lambda_{\max}}.
$$

At $\eta=2/\lambda_{\max}$, a nonzero error component along a largest-[eigenvalue](eigenvalue.md) [eigenvector](eigenvector.md) flips sign without shrinking. Above that threshold it grows. A particular start can still converge if it has zero components in every unstable direction; the interval is the condition for all starts. If $\rho=\max_i|1-\eta\lambda_i|<1$, then $\|e_k\|_2\leq\rho^k\|e_0\|_2$ and $E_k\leq\rho^{2k}E_0$. These bounds follow by summing the squared components in the [orthonormal basis](orthonormal-basis.md).

**Table of contents**

- [Optimal fixed step for quadratic gradient descent](optimal-fixed-step-for-quadratic-gradient-descent.md)

## ↑ Ancestors (6)

1. [Gradient descent](gradient-descent-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Gradient descent](gradient-descent-split.md)
