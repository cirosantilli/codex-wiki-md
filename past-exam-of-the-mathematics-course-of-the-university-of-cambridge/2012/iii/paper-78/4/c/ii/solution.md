<h1 id="4/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Substitution into the [Tikhonov regularization](../../../../../../../tikhonov-regularization.md) series gives an explicit reconstruction for every $y\in L^2(0,1)$:

$$
\boxed{x_\alpha(x)=\sum_{n=1}^{\infty}\frac{a_n}{1+\alpha a_n^2}\left[\int_0^1 y(t)\sqrt2\sin(a_nt)\,dt\right]\sqrt2\cos(a_nx),\qquad a_n=(n-\tfrac12)\pi.}
$$

Equivalently the summand is $\sigma_n\langle y,v_n\rangle u_n/(\alpha+\sigma_n^2)$. The [Tikhonov stability bound](../../../../../../../tikhonov-stability-bound.md) makes the series converge in $L^2$ for every positive $\alpha$. It suppresses high-frequency components of unstable differentiation, rather than differentiating arbitrary noisy data pointwise.

The [range of the Volterra integration operator](../../../../../../../range-of-the-volterra-integration-operator.md) is $\{y\in H^1(0,1):y(0)=0\}$. On exactly these data, $A^\dagger y=y'$ and the series converges to $y'$ as $\alpha\downarrow0$. For arbitrary $L^2$ data outside that range, a finite regularized solution still exists, but a finite-norm unregularized solution need not exist. This is [Spectral Tikhonov differentiation for the Volterra operator](../../../../../../../spectral-tikhonov-differentiation-for-the-volterra-operator.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Paper 78](../../../../paper-78-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
