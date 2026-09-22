<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With $x=2z-1$, the [chain rule](../../../../../../chain-rule.md) gives $T_{xx}=V_{zz}/4$. Thus

$$
V_t=\frac14V_{zz},\quad0<z<1,\qquad V(0,t)=V(1,t)=0,\qquad V(z,0)=T_0.
$$

[Separation of variables](../../../../../../separation-of-variables.md) gives the [eigenfunctions](../../../../../../eigenfunction.md) $\sin(n\pi z)$ with time factors $e^{-n^2\pi^2t/4}$. The [Fourier sine coefficients](../../../../../../fourier-sine-coefficient.md) of the initial constant are

$$
b_n=2\int_0^1T_0\sin(n\pi z)\,dz=\frac{2T_0(1-(-1)^n)}{n\pi}.
$$

Only odd modes survive, so

$$
\boxed{V(z,t)=\frac{4T_0}{\pi}\sum_{k=0}^\infty\frac{\sin((2k+1)\pi z)}{2k+1}e^{-(2k+1)^2\pi^2t/4}.}
$$

Returning to $x$, $\sin((2k+1)\pi(x+1)/2)=(-1)^k\cos((2k+1)\pi x/2)$, hence

$$
\boxed{T(x,t)=\frac{4T_0}{\pi}\sum_{k=0}^\infty\frac{(-1)^k}{2k+1}\cos\!\left(\frac{(2k+1)\pi x}{2}\right)e^{-(2k+1)^2\pi^2t/4}.}
$$

For every $t>0$ the exponential coefficients give [uniform convergence](../../../../../../uniform-convergence.md) of the differentiated series on later-time compact sets, verifying the PDE and [boundary conditions](../../../../../../boundary-condition.md). As $t\downarrow0$, the solution tends to $T_0$ at every interior point and in [L2 norm](../../../../../../l2-norm.md), while remaining zero at the endpoints. The expression is visibly even in $x$, consistent with the corrected symmetry argument for $b=0$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
