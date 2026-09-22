<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Subtract the constant [steady state](../../../../../../steady-state.md) profile: set $v=T-T_0$. Then

$$
v_t=\kappa v_{xx},\qquad v(0,t)=0,\qquad v_x(L,t)=0.
$$

The last equation follows from [Fourier's law](../../../../../../fourier-s-law.md) and zero [heat flux](../../../../../../heat-flux-density.md) at the insulated end. For a nonzero separated solution $v=X(x)H(t)$, [separation of variables](../../../../../../separation-of-variables.md) gives

$$
\frac{H'}{\kappa H}=\frac{X''}{X}=-\mu,\qquad
-X''=\mu X,\qquad X(0)=0,\quad X'(L)=0.
$$

To see that $\mu>0$ for a nonzero [eigenfunction](../../../../../../eigenfunction.md), multiply the spatial equation by $X$ and use [integration by parts](../../../../../../integration-by-parts.md):

$$
\mu\int_0^L X^2\,dx=\int_0^L(X')^2\,dx.
$$

Both boundary terms vanish. If the right side were zero, $X$ would be constant and $X(0)=0$ would make it zero. Thus write $\mu=\lambda^2$ with $\lambda>0$. Solving gives $X=A\sin(\lambda x)$, and $X'(L)=0$ requires $\cos(\lambda L)=0$. The [mixed Dirichlet-Neumann modes on an interval](../../../../../../mixed-dirichlet-neumann-modes-on-an-interval.md) therefore have

$$
\lambda_n=\frac{(2n-1)\pi}{2L},\qquad X_n(x)=\sin(\lambda_nx),\qquad
H_n(t)=e^{-\kappa\lambda_n^2t},\qquad n=1,2,\ldots.
$$

The [eigenvalues](../../../../../../eigenvalue.md) of $-d^2/dx^2$ are $\mu_n=\lambda_n^2$; $\lambda_n$ are their positive square roots. By [superposition](../../../../../../superposition-principle.md), with coefficients for which the resulting [series](../../../../../../series-mathematics.md) and its required [derivatives](../../../../../../derivative.md) converge at positive times,

$$
\boxed{T(x,t)=T_0+\sum_{n=1}^{\infty}b_n\sin\left(\frac{(2n-1)\pi x}{2L}\right)\exp\left[-\frac{\kappa(2n-1)^2\pi^2t}{4L^2}\right].}
$$

The [eigenfunctions](../../../../../../eigenfunction.md) are [orthogonal](../../../../../../orthogonal-vectors.md) on $[0,L]$ and have squared norm $L/2$. Expanding the initial excess [temperature](../../../../../../temperature-split.md) $v(x,0)=T_0x/L$ gives

$$
\begin{aligned}
b_n&=\frac2L\int_0^L\frac{T_0x}{L}\sin(\lambda_nx)\,dx\\
&=\frac{2T_0}{L^2}\left[-\frac{x\cos(\lambda_nx)}{\lambda_n}+\frac{\sin(\lambda_nx)}{\lambda_n^2}\right]_0^L\\
&=\frac{2T_0(-1)^{n-1}}{L^2\lambda_n^2}
=\boxed{\frac{8T_0(-1)^{n-1}}{(2n-1)^2\pi^2}}.
\end{aligned}
$$

Thus the requested [temperature](../../../../../../temperature-split.md) is

$$
\boxed{T(x,t)=T_0+\frac{8T_0}{\pi^2}\sum_{n=1}^{\infty}\frac{(-1)^{n-1}}{(2n-1)^2}\sin\left(\frac{(2n-1)\pi x}{2L}\right)e^{-\kappa(2n-1)^2\pi^2t/(4L^2)}.}
$$

At the insulated endpoint $\sin(\lambda_nL)=(-1)^{n-1}$ cancels the alternating coefficient sign, leaving

$$
\boxed{T(L,t)=T_0+\frac{8T_0}{\pi^2}\sum_{n=1}^{\infty}\frac{e^{-\kappa(2n-1)^2\pi^2t/(4L^2)}}{(2n-1)^2}>T_0\quad\text{for every finite }t\geq0.}
$$

Every summand is positive. **The endpoint temperature never drops below $T_0$**; it decreases towards $T_0$ as $t\to\infty$ and starts at $T(L,0)=2T_0$.

For completeness, the [Sturm-Liouville eigenfunction expansion](../../../../../../sturm-liouville-eigenfunction-expansion.md) gives the initial profile in the $L^2$ sense. Here the coefficients are absolutely summable, so the [Weierstrass M-test](../../../../../../weierstrass-m-test.md) also gives [uniform convergence](../../../../../../uniform-convergence.md) on $[0,L]\times[0,\infty)$, and the initial values are recovered everywhere. For positive times the exponential factors justify all required termwise [derivatives](../../../../../../derivative.md), giving a [classical solution](../../../../../../classical-solution.md). There is, however, an [initial incompatibility with a Neumann boundary condition](../../../../../../initial-incompatibility-with-a-neumann-boundary-condition.md) at $(L,0)$: the initial slope is $T_0/L$, while the insulated [Neumann boundary condition](../../../../../../neumann-boundary-condition.md) requires zero slope for $t>0$. The [temperature](../../../../../../temperature-split.md) is continuous to the initial edge, but $T_x$ cannot extend continuously to that corner. One must not differentiate the initial [series](../../../../../../series-mathematics.md) term by term at $x=L$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
