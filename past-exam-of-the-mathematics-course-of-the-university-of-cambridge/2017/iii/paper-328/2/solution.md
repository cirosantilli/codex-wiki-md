<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The drift makes the natural measure weighted. Let

$$
\mathcal A=\partial_x^2+\beta\partial_x
=e^{-\beta x}\partial_x(e^{\beta x}\partial_x),\qquad
w(x)=e^{\beta x}.
$$

Under homogeneous [Neumann boundary conditions](../../../../../neumann-boundary-condition.md), the [differential operator](../../../../../differential-operator.md) is [self-adjoint](../../../../../self-adjoint-operator.md) in the [weighted inner product](../../../../../weighted-inner-product.md) $\langle u,v\rangle_w=\int_0^Lw\overline u v\,dx$. Indeed [integration by parts](../../../../../integration-by-parts.md) gives

$$
\langle u,\mathcal Av\rangle_w
=-\int_0^L w\overline{u'}v'\,dx
$$

when the derivative boundary terms vanish. In particular its [eigenvalues](../../../../../eigenvalue.md) are nonpositive and it has the constant stationary [eigenfunction](../../../../../eigenfunction.md). We first construct the [weighted Neumann heat kernel with constant drift](../../../../../weighted-neumann-heat-kernel-with-constant-drift.md), then incorporate the two prescribed coordinate derivatives.

Put $b=\beta/2$. The [Robin gauge transform for constant drift](../../../../../robin-gauge-transform-for-constant-drift.md), $\phi=e^{-bx}\psi$, turns $\mathcal A\phi=-\lambda\phi$ into

$$
\psi''+(\lambda-b^2)\psi=0,\qquad
\psi'(0)=b\psi(0),\quad\psi'(L)=b\psi(L).
$$

These are coordinate-derivative [Robin boundary conditions](../../../../../robin-boundary-condition.md), with the same algebraic sign at both endpoints. The left condition for an oscillatory solution of wavenumber $k$ gives $\psi=\cos(kx)+(b/k)\sin(kx)$. The right condition then reduces to $(k+b^2/k)\sin(kL)=0$, giving $k_n=n\pi/L$. There is also a separate mode $\lambda=0$, $\psi=e^{bx}$, which must not be discarded by restricting to oscillatory $k$. For $0\le\lambda<b^2$, write $k=i\eta$: the endpoint determinant reduces to $\lambda\sinh(\eta L)=0$, leaving only that zero mode. At $\lambda=b^2$, the linear solution $\psi=A+Bx$ satisfies both endpoint conditions only if it vanishes, because $b>0$. The complete [Sturm-Liouville eigenfunction expansion](../../../../../sturm-liouville-eigenfunction-expansion.md) therefore uses

$$
\phi_0(x)=1,\quad\lambda_0=0,\qquad
\phi_n(x)=e^{-bx}\left[\cos(k_nx)+\frac b{k_n}\sin(k_nx)\right],\quad
\lambda_n=k_n^2+b^2,\quad n\ge1.
$$

Their squared [norms](../../../../../norm.md) in the weighted measure are

$$
N_0=\frac{e^{\beta L}-1}{\beta},\qquad
N_n=\frac L2\left(1+\frac{b^2}{k_n^2}\right),\quad n\ge1.
$$

The cancellation of the weight against $e^{-2bx}$ makes the latter formula an ordinary trigonometric integral. Define

$$
K_\beta(x,y,t)=\sum_{n=0}^\infty
\frac{e^{-\lambda_nt}\phi_n(x)\phi_n(y)}{N_n}.
$$

For $t>0$ this kernel is smooth in the interior. It integrates initial values against $w(y)dy$, not against unweighted [Lebesgue measure](../../../../../lebesgue-measure.md). It is symmetric in $x,y$ as a weighted kernel, even though the drift operator does not look symmetric in an unweighted inner product.

To determine the boundary forcing, set $a_n(t)=\langle\phi_n,q(\cdot,t)\rangle_w/N_n$. Two applications of [integration by parts](../../../../../integration-by-parts.md) leave

$$
N_na_n'(t)=-\lambda_nN_na_n(t)
+e^{\beta L}\phi_n(L)h_1(t)-\phi_n(0)g_1(t).
$$

The minus sign at the left endpoint is the sign of the boundary evaluation $[\cdot]_0^L$; the supplied $g_1$ is $q_x(0,t)$, not an outward normal derivative. Solving this [linear differential equation](../../../../../linear-differential-equation.md) by an [integrating factor](../../../../../integrating-factor.md) and recombining the modes gives the requested space-time [integral representation](../../../../../integral-representation.md):

$$
\boxed{q(x,t)=\int_0^L K_\beta(x,y,t)e^{\beta y}q_0(y)\,dy
+\int_0^t\left[e^{\beta L}K_\beta(x,L,t-s)h_1(s)
-K_\beta(x,0,t-s)g_1(s)\right]ds.}
$$

This is the [Neumann boundary-forcing formula](../../../../../neumann-boundary-forcing-formula.md). The zero mode also gives the useful consistency check

$$
\boxed{\frac d{dt}\int_0^L e^{\beta x}q(x,t)\,dx
=e^{\beta L}h_1(t)-g_1(t).}
$$

Ordinary unweighted mass instead obeys $d\int_0^Lq\,dx/dt=h_1-g_1+\beta[q(L,t)-q(0,t)]$. Replacing the weighted measure by $dy$ or deleting the constant mode would therefore give an incorrect solution.

There is a subtle point when checking nonzero derivative data: every homogeneous eigenfunction has zero endpoint derivative, but differentiating the boundary-forcing sum and its time integral term by term at an endpoint is not valid. The kernel is singular as $t-s\downarrow0$, and the prescribed derivatives are interior limits of the full solution. An explicit [Laplace transform](../../../../../laplace-transform.md) form verifies those limits without this interchange and gives an alternative purely contour-integral version.

For $\operatorname{Re}p>0$, set $\kappa=\sqrt{p+b^2}$ using the [principal square root](../../../../../principal-square-root-of-a-complex-number.md), and define

$$
u_p(x)=e^{-bx}\left[\cosh(\kappa x)+\frac b\kappa\sinh(\kappa x)\right],
$$



$$
v_p(x)=e^{-b(x-L)}\left[\cosh(\kappa(L-x))-\frac b\kappa\sinh(\kappa(L-x))\right].
$$

Both solve $(p-\mathcal A)f=0$, with $u_p(0)=v_p(L)=1$, $u_p'(0)=v_p'(L)=0$. Their weighted [Wronskian](../../../../../wronskian.md) is the nonzero constant

$$
D_p=e^{\beta x}(u_p'v_p-u_pv_p')
=e^{bL}\frac p\kappa\sinh(\kappa L).
$$

Hence the [resolvent kernel for Neumann advection-diffusion on an interval](../../../../../resolvent-kernel-for-neumann-advection-diffusion-on-an-interval.md) is

$$
\mathcal R_p(x,y)=\frac{u_p(\min(x,y))v_p(\max(x,y))}{D_p}.
$$

The first derivative in $x$ has jump $-e^{-\beta y}$, giving $(p-\mathcal A_x)\mathcal R_p=e^{-\beta y}\delta_y$ in the sense of [distributional derivatives](../../../../../distributional-derivative.md). If $G(p)=\int_0^T e^{-ps}g_1(s)ds$ and $H(p)=\int_0^T e^{-ps}h_1(s)ds$, an equivalent transformed solution is

$$
Q(x,p)=\int_0^L\mathcal R_p(x,y)e^{\beta y}q_0(y)\,dy
+\frac{e^{\beta L}u_p(x)H(p)-v_p(x)G(p)}{D_p}.
$$

In fact $v_p'(0)=-D_p$ and $u_p'(L)=e^{-\beta L}D_p$, so $Q_x(0,p)=G(p)$ and $Q_x(L,p)=H(p)$ exactly. The inverse [Bromwich contour](../../../../../bromwich-contour.md) integral of $e^{pt}Q(x,p)/(2\pi i)$ is an alternative final answer. Its poles at $p=0$ and $p=-\lambda_n$ reproduce the constant and decaying modes of $K_\beta$, respectively; apparent square-root singularities in the normalized hyperbolic factors are removable. This also independently checks the kernel normalization and boundary signs.

As in question 1, the printed dot on $q_0$ denotes its spatial [derivative](../../../../../derivative.md): the two corner conditions are $q_0'(0)=g_1(0)$ and $q_0'(L)=h_1(0)$. The initial [eigenfunction expansion](../../../../../eigenfunction-expansion.md) converges to $q_0$ in the weighted space and, for the stated smooth compatible data, has the appropriate classical initial and boundary limits. Differences of solutions with zero data satisfy $\frac12d\|q\|_w^2/dt=-\int_0^Lw|q_x|^2dx$, proving uniqueness in the usual regular solution class. In the limit $\beta\to0$, $N_0\to L$, $\phi_n\to\cos(n\pi x/L)$, and the ordinary [Neumann heat kernel on an interval](../../../../../neumann-heat-kernel-on-an-interval.md) and its boundary signs are recovered.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 328](../../paper-328-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
