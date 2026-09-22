<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With $h=\Delta x$, $\tau=\Delta t$, $r=\tau/h^2$ and $c=\alpha\tau/h$, the [Forward Euler method](../../../../../../euler-method.md) gives

$$
\boxed{u_m^{n+1}=(r-c/2)u_{m-1}^n+(1-2r)u_m^n+(r+c/2)u_{m+1}^n.}
$$

For a [Fourier mode](../../../../../../fourier-mode.md) $e^{im\theta}$, the amplification factor is $G(\theta)=1-4r\sin^2(\theta/2)+ic\sin\theta$. Set $s=\sin^2(\theta/2)$. Then

$$
|G|^2-1=4s\{c^2-2r+(4r^2-c^2)s\}.
$$

The expression in braces is an [affine function](../../../../../../affine-function.md) of $s$, so it is nonpositive for all $s\in[0,1]$ precisely when its two endpoint values are nonpositive. For $\tau>0$, these conditions are $c^2\leq2r$ and $r\leq1/2$. Thus [Forward Euler stability for centered advection-diffusion](../../../../../../forward-euler-stability-for-centered-advection-diffusion.md) requires exactly

$$
\boxed{\Delta t\leq\frac{(\Delta x)^2}{2},\qquad\alpha^2\Delta t\leq2.}
$$

For $\alpha=0$, only the first condition remains. If either bound fails, a band of [Fourier modes](../../../../../../fourier-mode.md) has $|G|>1$, giving instability under [von Neumann stability analysis](../../../../../../von-neumann-stability-analysis.md). At equality the amplification bound still holds, so the endpoints are included. This is discrete [L2 norm](../../../../../../l2-norm.md) stability; nonnegative stencil weights would impose the additional spatial restriction $|\alpha|\Delta x\leq2$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
