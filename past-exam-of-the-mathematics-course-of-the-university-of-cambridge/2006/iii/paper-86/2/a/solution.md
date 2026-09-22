<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Wirtinger derivative](../../../../../../wirtinger-derivatives.md) $f=q_z=(q_x-iq_y)/2$. Since $q$ satisfies the [Laplace equation](../../../../../../laplace-equation.md), $\partial_{\bar z}f=\Delta q/4=0$, so $f$ is [holomorphic](../../../../../../complex-differentiability-at-a-point.md). The differential relation is understood as a [one-form](../../../../../../one-form.md) identity:

$$
d(\mu e^{-ikz})=e^{-ikz}f(z)\,dz.
$$

The differential $dz$ is needed on its right-hand side. Because this form is closed, its [integral](../../../../../../integral.md) is independent of path within the semistrip.

Three spectral primitives are obtained by integrating from the two finite corners and from the infinite end:

$$
\mu_0=e^{ikz}\int_0^ze^{-ikw}f(w)\,dw,\qquad
\mu_l=e^{ikz}\int_{il}^ze^{-ikw}f(w)\,dw,\qquad
\mu_\infty=-e^{ikz}\int_z^{\infty+i\,\operatorname{Im}z}e^{-ikw}f(w)\,dw.
$$

The last [integral](../../../../../../integral.md) is taken horizontally and defines the infinite-end primitive for $\operatorname{Im}k<0$. Their differences are $e^{ikz}$ times the three boundary spectral [functions](../../../../../../function-split.md). Using counterclockwise boundary orientation, define

$$
\rho_L(k)=\int_{il}^0e^{-ikw}f(w)\,dw,\qquad
\rho_B(k)=\int_0^\infty e^{-ikx}f(x)\,dx,\qquad
\rho_T(k)=-e^{kl}\int_0^\infty e^{-ikx}f(x+il)\,dx.
$$

Then $\mu_0-\mu_\infty=e^{ikz}\rho_B$, $\mu_\infty-\mu_l=e^{ikz}\rho_T$, and $\mu_l-\mu_0=e^{ikz}\rho_L$. Their sum gives the [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) $\rho_L+\rho_B+\rho_T=0$ for $\operatorname{Im}k\leq0$.

To express these spectra in boundary data, write $g_0(x)=q(x,0)$, $g_l(x)=q(x,l)$, $h(y)=q(0,y)$, $n_0(x)=q_y(x,0)$, $n_l(x)=q_y(x,l)$, and $v(y)=q_x(0,y)$. Direct substitution into $f$ gives

$$
\begin{aligned}
\rho_B(k)&=\frac12\int_0^\infty e^{-ikx}[g_0'(x)-in_0(x)]\,dx,\\
\rho_T(k)&=-\frac{e^{kl}}2\int_0^\infty e^{-ikx}[g_l'(x)-in_l(x)]\,dx,\\
\rho_L(k)&=-\frac12\int_0^le^{ky}[h'(y)+iv(y)]\,dy.
\end{aligned}
$$

These are transforms of tangential [derivatives](../../../../../../derivative.md) of [Dirichlet boundary data](../../../../../../dirichlet-boundary-data.md) and the corresponding [Neumann boundary data](../../../../../../neumann-boundary-data.md). The outward [derivatives](../../../../../../derivative.md) are $-n_0$ at the bottom, $n_l$ at the top, and $-v$ at the left.

The [boundary spectral representation of a holomorphic function on a semistrip](../../../../../../boundary-spectral-representation-of-a-holomorphic-function-on-a-semistrip.md) is

$$
\boxed{q_z(z)=\frac1{2\pi}\left[
\int_0^{i\infty}e^{ikz}\rho_L(k)\,dk
+\int_0^\infty e^{ikz}\rho_B(k)\,dk
+\int_0^{-\infty}e^{ikz}\rho_T(k)\,dk\right].}
$$

All three $k$-rays are oriented outward from zero. To verify the spectral inversion, use

$$
\int_0^{e^{i\theta}\infty}e^{ik(z-w)}\,dk=\frac{i}{z-w}
$$

whenever the exponential decays. The positive real ray works for the bottom, the negative real ray for the top, and the positive imaginary ray for the left. Substitution of the boundary spectra therefore turns the boxed formula into $(2\pi i)^{-1}\int_{\partial\Omega}f(w)/(w-z)\,dw=f(z)$ by the [Cauchy integral formula](../../../../../../cauchy-integral-formula.md). This also fixes all orientation signs.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 86](../../../paper-86-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
