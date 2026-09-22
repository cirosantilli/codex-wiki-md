<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use a time [Laplace transform](../../../../../laplace-transform.md) and a spatial [Green function](../../../../../green-s-function.md). The first-order transport term must be retained: the [Airy resolvent kernel](../../../../../airy-resolvent-kernel.md) for $\partial_x^3+p$ alone would solve a different equation. The governing [linear partial differential equation](../../../../../linear-partial-differential-equation.md) is the [linear dispersive Stokes equation](../../../../../linear-dispersive-stokes-equation.md), distinct from the viscous-fluid [Stokes equation](../../../../../stokes-equation.md).

For the time interval of interest, extend the given boundary signal by zero after $T$ and put

$$
G(p)=\int_0^T e^{-ps}g_1(s)\,ds,\qquad \operatorname{Re}p>0.
$$

The possible discontinuity at $T$ does not affect a solution at $t<T$. Equivalently, use any sufficiently regular continuation beyond $T$: the resulting [causal Green function](../../../../../causal-green-function.md) produces the same earlier solution. We seek the usual solution with spatial decay and a time transform, rather than an unrestricted spatially growing solution on the half-line.

Writing $Q(x,p)$ for the time [Laplace transform](../../../../../laplace-transform.md), the [Laplace transform of a derivative](../../../../../laplace-transform-of-a-derivative.md) gives

$$
Q_{xxx}+Q_x+pQ=q_0(x),\qquad Q_x(0,p)=G(p).
$$

The corresponding [characteristic roots](../../../../../characteristic-root-of-a-constant-coefficient-differential-equation.md) are the three [roots of a polynomial](../../../../../root-of-a-polynomial.md)

$$
P_p(r)=r^3+r+p.
$$

For $\operatorname{Re}p>0$, label the unique root of negative [real part](../../../../../real-part.md) by $r_-(p)$, and the two roots of positive [real part](../../../../../real-part.md) by $r_1(p),r_2(p)$. This [spatial root splitting for the dispersive Stokes resolvent](../../../../../spatial-root-splitting-for-the-dispersive-stokes-resolvent.md) is easily checked: if $r=ik$, then $p=-i(k-k^3)$ is imaginary, so no root crosses the imaginary axis as $p$ varies in the right half-plane. For real $p>0$ the cubic is strictly increasing on the real line and has one negative real root, while its conjugate pair has positive [real parts](../../../../../real-part.md). The root count remains the same throughout that connected half-plane. A repeated root would satisfy $3r^2+1=0$ and again put $p$ on the imaginary axis. All roots are therefore simple there, and $r_-(p)$ is a nonzero [holomorphic function](../../../../../holomorphic-function.md).

Set $d_j=3r_j^2+1$, including $j=-$. Define the [Stokes resolvent kernel with advection](../../../../../stokes-resolvent-kernel-with-advection.md)

$$
R_p(s)=
\begin{cases}
e^{r_-s}/d_-,&s\ge0,\\
-\displaystyle\sum_{j=1}^2 e^{r_js}/d_j,&s<0.
\end{cases}
$$

The sign on the negative half-line is essential. To verify the [Green function](../../../../../green-s-function.md), use the [partial fraction decomposition](../../../../../partial-fraction-decomposition.md)

$$
\frac1{P_p(r)}=\sum_{j\in\{-,1,2\}}\frac1{d_j(r-r_j)}.
$$

Its expansion at infinity yields the [reciprocal-polynomial root identities](../../../../../reciprocal-polynomial-root-identities.md)

$$
\sum_j\frac1{d_j}=0,\qquad
\sum_j\frac{r_j}{d_j}=0,\qquad
\sum_j\frac{r_j^2}{d_j}=1.
$$

Consequently $R_p$ and $R_p'$ are continuous at zero, and $R_p''$ has jump one. Each piece solves the homogeneous [ordinary differential equation](../../../../../ordinary-differential-equation.md), so the [jump conditions for a third-order Green function](../../../../../jump-conditions-for-a-third-order-green-function.md) imply, in the sense of [distributional derivatives](../../../../../distributional-derivative.md),

$$
(p+\partial_s+\partial_s^3)R_p=\delta_0.
$$

Both pieces decay in their respective spatial directions.

Now define

$$
V(x,p)=\int_0^\infty R_p(x-y)q_0(y)\,dy.
$$

It satisfies the transformed inhomogeneous equation. The difference $Q-V$ solves the homogeneous [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation.md); spatial decay leaves only $e^{r_-x}$. Imposing the [Neumann boundary condition](../../../../../neumann-boundary-condition.md) fixes its coefficient, giving the [half-line Stokes solution with a boundary derivative](../../../../../half-line-stokes-solution-with-a-boundary-derivative.md)

$$
Q(x,p)=V(x,p)+\frac{e^{r_-x}}{r_-}\bigl[G(p)-V_x(0,p)\bigr].
$$

No division by a vanishing root is involved, since $r_-=0$ would require $p=0$. Moreover the remaining boundary trace is explicitly known from $q_0$:

$$
V_x(0,p)=-\sum_{j=1}^2\frac{r_j}{d_j}
\int_0^\infty e^{-r_jy}q_0(y)\,dy.
$$

Thus introduce the completely explicit initial-data kernel

$$
K_p(x,y)=R_p(x-y)-\frac{e^{r_-x}}{r_-}R_p'(-y)
=R_p(x-y)+\frac{e^{r_-x}}{r_-}
\sum_{j=1}^2\frac{r_j e^{-r_jy}}{d_j}.
$$

For any upward [Bromwich contour](../../../../../bromwich-contour.md) $\operatorname{Re}p=\sigma>0$ to the right of any transform singularities, the requested [integral representation](../../../../../integral-representation.md) is

$$
\boxed{q(x,t)=\frac1{2\pi i}\int_{\sigma-i\infty}^{\sigma+i\infty}
e^{pt}\left[\int_0^\infty K_p(x,y)q_0(y)\,dy
+\frac{e^{r_-(p)x}}{r_-(p)}\int_0^T e^{-ps}g_1(s)\,ds\right]dp.}
$$

The contour integral is understood in the standard [Bromwich inversion formula](../../../../../bromwich-inversion-formula.md) sense, with truncation limits if it is not absolutely convergent. Every term is expressed in the supplied data and algebraic [characteristic roots](../../../../../characteristic-root-of-a-constant-coefficient-differential-equation.md); there are no unknown Dirichlet or second-derivative boundary traces.

The transformed equation verifies the [linear partial differential equation](../../../../../linear-partial-differential-equation.md) and the initial term, while taking the spatial [derivative](../../../../../derivative.md) gives $Q_x(0,p)=G(p)$. [Bromwich inversion formula](../../../../../bromwich-inversion-formula.md) therefore supplies the prescribed derivative for $0<t<T$ and the initial value for $x>0$. For zero initial and boundary data, the transformed solution is a decaying homogeneous mode with zero boundary derivative, hence vanishes; this proves uniqueness in the stated transform/decay class. A change of the boundary continuation after $T$ has transform $e^{-pT}$ times another causal transform and contributes only after $T$, by the [Laplace transform time-shift rule](../../../../../laplace-transform-time-shift-rule.md). The printed dot on $q_0$ is interpreted as its derivative in its sole variable $x$, so the stated corner compatibility is $q_0'(0)=g_1(0)$. Additional differentiability at the corner requires the corresponding higher-order compatibility, but is not needed for the representation at positive $x,t$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 328](../../paper-328-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
