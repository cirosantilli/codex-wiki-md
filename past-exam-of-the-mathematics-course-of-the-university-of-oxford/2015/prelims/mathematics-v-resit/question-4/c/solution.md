<h1 id="question-4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For [separation of variables](../../../../../../separation-of-variables.md), put $U=X(x)H(t)$ and set $X''/X=H'/(\kappa H)=-\lambda$. The [boundary conditions](../../../../../../boundary-condition.md) are $X(0)=0$, $X'(L)=0$. Multiplying $-X''=\lambda X$ by $X$ and using [integration by parts](../../../../../../integration-by-parts.md) gives

$$
\lambda\int_0^L X^2\,dx=\int_0^L(X')^2\,dx.
$$

A nonzero solution therefore has $\lambda>0$: the zero case forces $X$ constant, and then $X(0)=0$ forces $X=0$. Writing $\lambda=\mu^2$, the [eigenfunctions](../../../../../../eigenfunction.md) and their temporal factors are

$$
X_n(x)=\sin(\mu_nx),\qquad
\mu_n=\frac{(n+1/2)\pi}{L},\qquad
H_n(t)=e^{-\kappa\mu_n^2t},\qquad n=0,1,\ldots.
$$

These [sine](../../../../../../sine.md) functions are [orthogonal](../../../../../../orthogonal-vectors.md) on $[0,L]$, with squared [norm](../../../../../../norm.md) $L/2$. Expanding the [initial condition](../../../../../../initial-condition.md) and multiplying by $\sin(\mu_mx)$ gives, using the permitted interchange of the [sum](../../../../../../sum.md) and [integral](../../../../../../integral-split.md),

$$
\begin{aligned}
b_n
&=\frac2L\int_0^L\left(-\frac{T_0x}{L}\right)\sin(\mu_nx)\,dx\\
&=-\frac{2T_0}{L^2}
\left[-\frac{x\cos(\mu_nx)}{\mu_n}
+\frac{\sin(\mu_nx)}{\mu_n^2}\right]_0^L\\
&=-\frac{2T_0(-1)^n}{L^2\mu_n^2}
=-\frac{8T_0(-1)^n}{\pi^2(2n+1)^2}.
\end{aligned}
$$

Here $\cos(\mu_nL)=0$ and $\sin(\mu_nL)=(-1)^n$. Thus the [Fourier series](../../../../../../fourier-series-split.md) solution is

$$
\boxed{U(x,t)=-\frac{8T_0}{\pi^2}\sum_{n=0}^\infty
\frac{(-1)^n}{(2n+1)^2}
\sin\left(\frac{(2n+1)\pi x}{2L}\right)
\exp\left(-\frac{\kappa(2n+1)^2\pi^2t}{4L^2}\right),\qquad T=T_0+U.}
$$

The [exponential decay](../../../../../../exponential-decay.md) permits differentiation of the [series](../../../../../../series-mathematics.md) for $t>0$, and each term satisfies both [boundary conditions](../../../../../../boundary-condition.md). At $t=0$ it is the mixed-end [Fourier expansion](../../../../../../fourier-series-split.md) of $-T_0x/L$.

The gained [heat](../../../../../../heat-split.md) is the increase in [internal energy](../../../../../../internal-energy-split.md). Since the paper specifies no [cross-sectional area](../../../../../../cross-sectional-area.md), first give the answer per unit [cross-sectional area](../../../../../../cross-sectional-area.md); multiply by $A$ for a rod of [cross-sectional area](../../../../../../cross-sectional-area.md) $A$. The initial [temperature](../../../../../../temperature-split.md) has [integral](../../../../../../integral-split.md) $T_0L/2$, whereas $\int_0^L\sin(\mu_nx)\,dx=1/\mu_n$. At $t_*=L^2/\kappa$ this gives

$$
\boxed{\frac{\Delta Q}{A}
=\rho cT_0L\left[
\frac12-\frac{16}{\pi^3}\sum_{n=0}^\infty
\frac{(-1)^n}{(2n+1)^3}
\exp\left(-\frac{(2n+1)^2\pi^2}{4}\right)
\right].}
$$

Numerically $\Delta Q/A\simeq0.45623855\,\rho cT_0L$. This is positive and less than the eventual gain $\rho cT_0L/2$, as expected from relaxation towards the uniform [steady state](../../../../../../steady-state.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [Question 4](../../question-4.md)
3. [Mathematics V resit](../../../mathematics-v-resit-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
