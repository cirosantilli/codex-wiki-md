# Paper 70

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_70.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_70.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 70](paper-70.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use the half-line [Fourier transform](../../../analysis.md#fourier-transform) and finite-time boundary transforms

$$
\widehat q(k,t)=\int_0^\infty e^{-ikx}q(x,t)\,dx,\qquad G_j(k,t)=\int_0^t e^{ik^2s}g_j(s)\,ds,\quad g_j(t)=\partial_x^jq(0,t),\quad j=0,1.
$$

The half-line [Fourier transform](../../../analysis.md#fourier-transform) is analytic for $\operatorname{Im}k<0$ under spatial decay. All spectral integrals below have their usual oscillatory, or vanishing Gaussian damping, interpretation until absolute convergence is established.

The [free Schrodinger equation](../../../physics.md#free-schrodinger-equation) has the local divergence identity

$$
\partial_t(e^{-ikx+ik^2t}q)=i\partial_x\left[e^{-ikx+ik^2t}(q_x+ikq)\right].
$$

Integrating in $x,t$ gives the [global relation for the half-line free Schrodinger equation](../../../integrable-systems.md#global-relation-for-the-half-line-free-schrodinger-equation)

$$
\boxed{e^{ik^2t}\widehat q(k,t)=\widehat q_0(k)+kG_0(k,t)-iG_1(k,t),\qquad\operatorname{Im}k\leq0.}
$$

Let $D_+=\{\operatorname{Re}k>0,\operatorname{Im}k>0\}$. Orient its boundary from $i\infty$ down to $0$, and then from $0$ to $+\infty$, so that $D_+$ lies on the left. [Fourier inversion](../../../fourier-analysis.md#fourier-inversion-theorem) followed by [contour integration](../../../complex-analysis.md#contour-integration) in the second quadrant yields

$$
\boxed{q(x,t)=\frac1{2\pi}\int_{\mathbb R}e^{ikx-ik^2t}\widehat q_0(k)\,dk+\frac1{2\pi}\int_{\partial D_+}e^{ikx-ik^2t}\left[kG_0(k,t)-iG_1(k,t)\right]dk.}
$$

This is a complex spectral representation involving the initial trace and both boundary traces. The contour deformation works because each boundary-time integrand contains $e^{-ik^2(t-s)}$ with $s\leq t$, which decays in the second quadrant, as well as $e^{ikx}$ for $x>0$. This fixes both the quadrant and the orientation; changing either without changing the signs would produce an incorrect representation.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The unknown [Neumann boundary condition](../../../differential-equation.md#neumann-boundary-condition) can be removed by the [Fokas method](../../../differential-equation.md#fokas-method). Evaluate the [global relation for the half-line free Schrodinger equation](../../../integrable-systems.md#global-relation-for-the-half-line-free-schrodinger-equation) at $-k$:

$$
e^{ik^2t}\widehat q(-k,t)=\widehat q_0(-k)-kG_0(k,t)-iG_1(k,t).
$$

Consequently $kG_0-iG_1=2kG_0-\widehat q_0(-k)+e^{ik^2t}\widehat q(-k,t)$. In the representation from part (a), the last term has integral $\int_{\partial D_+}e^{ikx}\widehat q(-k,t)dk=0$, by the [Cauchy integral theorem](../../../complex-analysis.md#cauchy-s-integral-theorem) and [Jordan lemma](../../../complex-analysis.md#jordan-s-lemma). It is analytic in the upper half-plane, and the exponential decays on the closing first-quadrant arc. Hence an expression involving only the given data is

$$
\boxed{q(x,t)=\frac1{2\pi}\int_{\mathbb R}e^{ikx-ik^2t}\widehat q_0(k)dk+\frac1{2\pi}\int_{\partial D_+}e^{ikx-ik^2t}\left[2kG_0(k,t)-\widehat q_0(-k)\right]dk.}
$$

One may replace $t$ by $T$ in the upper limit defining $G_0$: the contribution of boundary times $s>t$ closes to zero in $D_+$, since $e^{-ik^2(t-s)}$ then decays there. Using $t$ makes causality transparent.

For an explicit proof of [uniform convergence](../../../real-analysis.md#uniform-convergence), it is useful to apply [boundary lifting](../../../differential-equation.md#boundary-lifting) before inversion. Set $h(x)=e^{-x}$, $c=g_0(0)$, $w_0(x)=q_0(x)-ch(x)$, and

$$
S_0(k)=\int_0^\infty\sin(kx)w_0(x)dx,\qquad H(k)=\int_0^\infty\sin(kx)h(x)dx=\frac{k}{1+k^2},\qquad f(t)=ig_0(t)-g_0'(t).
$$

The compatibility condition gives $w_0(0)=0$. The [Fourier sine transform](../../../analysis.md#fourier-sine-transform) of $w=q-g_0h$ satisfies $S_t+ik^2S=Hf$, with initial value $S_0$. The [integrating factor](../../../differential-equation.md#integrating-factor) therefore gives the equivalent representation

$$
\boxed{q(x,t)=g_0(t)e^{-x}+\frac2\pi\int_0^\infty\sin(kx)\left[e^{-ik^2t}S_0(k)+\frac{k}{1+k^2}\int_0^t e^{-ik^2(t-s)}f(s)ds\right]dk.}
$$

This last integral is **absolutely and uniformly convergent for $x\geq0$, $0\leq t\leq T$** under concrete sufficient hypotheses $w_0,w_0',w_0''\in L^1$, decay of the boundary terms, and $g_0\in C^2[0,T]$. Indeed, two [integrations by parts](../../../calculus.md#integration-by-parts) give $|S_0(k)|\leq\|w_0''\|_1/k^2$ for $k\geq1$. Another [integration by parts](../../../calculus.md#integration-by-parts), this time in $s$, gives

$$
\left|\int_0^t e^{-ik^2(t-s)}f(s)ds\right|\leq\frac{2\|f\|_\infty+T\|f'\|_\infty}{k^2}.
$$

Thus the initial term is uniformly $O(k^{-2})$ and the forcing term uniformly $O(k^{-3})$. For $0<k<1$, use $|S_0(k)|\leq\|w_0\|_1$ and the bounded time integral. An integrable majorant proves the claimed [uniform convergence](../../../real-analysis.md#uniform-convergence) and permits evaluation at both boundaries.

At $t=0$, [Fourier sine inversion](../../../analysis.md#fourier-sine-inversion) gives $q(x,0)=ce^{-x}+w_0(x)=q_0(x)$. At $x=0$, the integral vanishes, giving $q(0,t)=g_0(t)$, including the compatible corner. To verify the equation, note that $h''=h$ and the transformed equation implies

$$
iw_t+w_{xx}=-(ig_0'+g_0)h.
$$

Adding the lifted part gives $iq_t+q_{xx}=0$. Under the stated smoothness, this holds classically in the interior; differentiated spectral integrals can first be Gaussian-regularized, or read in the sine-transform $L^2$ sense and then identified with the smooth solution. Uniform convergence of $q$ itself does not require claiming uniform convergence of every differentiated integral at the corner.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Splitting the [free Schrodinger equation](../../../physics.md#free-schrodinger-equation) into real and imaginary parts gives

$$
\boxed{u_t=-v_{xx},\qquad v_t=u_{xx}.}
$$

Differentiating the first relation in time and using the second yields the [Euler-Bernoulli beam equation](../../../continuum-mechanics.md#euler-bernoulli-beam-equation) $u_{tt}+u_{xxxx}=0$. This is the [Schrodinger factorization of the elastic beam equation](../../../continuum-mechanics.md#schrodinger-factorization-of-the-elastic-beam-equation).

Assume the initial velocity has an integrable first spatial moment, as allowed by sufficient decay, and define

$$
v_0(x)=-\int_x^\infty(s-x)u_1(s)ds,\qquad q_0(x)=u_0(x)+iv_0(x).
$$

Then $v_0''=-u_1$ and $v_0$ decays at infinity. To encode the second boundary datum, define

$$
v_b(t)=v_0(0)+\int_0^t\widetilde u_1(s)ds,\qquad g_0(t)=\widetilde u_0(t)+iv_b(t).
$$

The [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition) for the resulting [free Schrodinger equation](../../../physics.md#free-schrodinger-equation) is compatible at the corner, since $q_0(0)=g_0(0)$. Insert these explicit $q_0,g_0$ into the data-only complex integral in part (b), with $\widehat q_0$ and $G_0$ defined as in part (a). **The required displacement is the real part of that integral.** Equivalently, the uniformly convergent lifted integral in part (b) may be used with the same complex data.

The [Schrodinger factorization of the elastic beam equation](../../../continuum-mechanics.md#schrodinger-factorization-of-the-elastic-beam-equation) verifies every condition: $u(x,0)=u_0(x)$, $u_t(x,0)=-v_0''(x)=u_1(x)$, $u(0,t)=\widetilde u_0(t)$, and

$$
u_{xx}(0,t)=v_t(0,t)=v_b'(t)=\widetilde u_1(t).
$$

The corner requirements on $u_0''$ and $\widetilde u_0'$ ensure consistency of these derivative traces; the natural interpretation of the last printed compatibility is $\widetilde u_0'(0)=u_1(0)$. If its prime were instead imposed for every $t$, that would simply be an extra restriction on the data, and the same construction would still solve them.

## 2

↑ **Parent:** [Paper 70](paper-70.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Use the [Wirtinger derivative](../../../analysis.md#wirtinger-derivatives) $q_z=(q_x-iq_y)/2$ and write $z=x+iy$. Since $q$ solves the [Laplace equation](../../../partial-differential-equation.md#laplace-equation), $q_z$ is a [holomorphic function](../../../complex-analysis.md#holomorphic-function). The transforms in the question select solutions with sufficient decay at infinity. In this class the solution, when it exists, is unique; hence reflection of the symmetric data about $y=\ell/2$ gives

$$
q(x,\ell-y)=q(x,y),\qquad q(x,\ell)=q(x,0).
$$

For $\gamma>0$, this uniqueness follows directly from [Green's first identity](../../../partial-differential-equation.md#green-s-first-identity): the homogeneous problem has integral $\int|\nabla q|^2+\gamma\int_{y=0,\ell}q^2=0$. For arbitrary real $\gamma$, the decaying-class qualifications are explained in part (c). Without a condition at infinity, symmetry of the data alone would not force symmetry of every solution.

Put $c=q(0,0)$, $f(x)=q(x,0)$, and introduce a known transform

$$
\psi(s)=\frac12\int_0^\infty e^{sx}f(x)dx,\qquad H(k)=\frac12\int_0^\ell e^{ky}g(y)dy.
$$

The bottom [Robin boundary condition](../../../differential-equation.md#robin-boundary-condition) gives $q_y=\gamma f$, while the top one gives $q_y=-\gamma f$. The bottom side is traversed from infinity to zero. [Integration by parts](../../../calculus.md#integration-by-parts) therefore gives

$$
G_1=-\frac12\int_0^\infty e^{-ikx}(f'-i\gamma f)dx=\boxed{\frac c2-i(k-\gamma)\psi(-ik)}.
$$

The top side is traversed from $i\ell$ towards infinity, and its exponential supplies $e^{k\ell}$, giving

$$
\boxed{G_3=e^{k\ell}\left[-\frac c2+i(k+\gamma)\psi(-ik)\right].}
$$

On the vertical side, $dz=i\,dy$ and the prescribed [Neumann boundary condition](../../../differential-equation.md#neumann-boundary-condition) is $q_x=g$. Thus

$$
G_2=\frac12\int_0^\ell e^{ky}(q_y+ig)dy=\boxed{\phi(k)+iH(k)}.
$$

Both the side orientations and the factor $1/2$ from the [Wirtinger derivative](../../../analysis.md#wirtinger-derivatives) are essential to these signs.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [Cauchy integral theorem](../../../complex-analysis.md#cauchy-s-integral-theorem) applied to $e^{-ikz}q_z$ yields the [global relation](../../../differential-equation.md#global-relation-for-a-linear-boundary-value-problem)

$$
G_1(k)+G_2(k)+G_3(k)=0.
$$

Initially this follows for $\operatorname{Im}k\leq0$, where the far vertical closing segment vanishes. The identities below can be compared on the real axis, and then continued wherever the respective transforms are analytic.

Define the characteristic factor of the [symmetric Robin strip transform](../../../differential-equation.md#symmetric-robin-strip-transform)

$$
D(k)=(k-\gamma)-(k+\gamma)e^{k\ell}.
$$

Substituting part (a) into the [global relation](../../../differential-equation.md#global-relation-for-a-linear-boundary-value-problem) gives

$$
\phi(k)=iD(k)\psi(-ik)-iH(k)-\frac c2(1-e^{k\ell}).
$$

Reflection symmetry gives $H(-k)=e^{-k\ell}H(k)$ and $\phi(-k)=-e^{-k\ell}\phi(k)$, because $q_y(0,\ell-y)=-q_y(0,y)$. Also $D(-k)=e^{-k\ell}D(k)$. Use the [global relation](../../../differential-equation.md#global-relation-for-a-linear-boundary-value-problem) at $-k$ and multiply by $-e^{k\ell}$ to obtain

$$
\phi(k)=-iD(k)\psi(ik)+iH(k)-\frac c2(1-e^{k\ell}).
$$

Comparison therefore proves

$$
\boxed{\psi(-ik)=\frac{2H(k)}{D(k)}-\psi(ik),\qquad\phi(k)=iH(k)-iD(k)\psi(ik)-\frac c2(1-e^{k\ell}).}
$$

At a zero of $D$, this identity is interpreted through the necessary solvability condition and a removable limit when a decaying solution exists. For $\gamma>0$, $D$ has no real zeros, so no such qualification is needed on the two real integration rays.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Substitute part (b) into the spectral representation. The terms containing $\psi(ik)$ are

$$
\frac{i}{2\pi}\left[\left(\int_0^\infty-\int_0^{i\infty}\right)e^{ikz}(k-\gamma)\psi(ik)dk+\left(\int_0^{i\infty}-\int_0^{-\infty}\right)e^{ik(z-i\ell)}(k+\gamma)\psi(ik)dk\right].
$$

The transform $\psi(ik)$ is analytic for $\operatorname{Im}k>0$. Write $k=a+ib$. In the first quadrant,

$$
|e^{ikz}|=e^{-ay-bx},
$$

which decays since $x,y>0$. The [Cauchy integral theorem](../../../complex-analysis.md#cauchy-s-integral-theorem) in that quadrant equates the two integrals in the first parentheses. In the second quadrant,

$$
|e^{ik(z-i\ell)}|=e^{-a(y-\ell)-bx},
$$

which decays since $a<0$, $b>0$, and $y<\ell$. The same [contour integration](../../../complex-analysis.md#contour-integration) equates the two integrals in the second parentheses. Therefore **$\psi(ik)$ makes no contribution**. This is [upper-quadrant cancellation of reflected boundary transforms](../../../differential-equation.md#upper-quadrant-cancellation-of-reflected-boundary-transforms), and it uses the whole paired expression rather than attempting to discard an individual integral.

The terms involving $c$ cancel by the same two quadrant arguments with the analytic factors $k\pm\gamma$ and $\psi$ omitted. There is a sign defect in the printed reconstruction prefactor. The sides specified in part (a) form a clockwise boundary, so the [Cauchy integral theorem](../../../complex-analysis.md#cauchy-s-integral-theorem) gives a negative reconstruction sign. Indeed, integrating each spectral ray first yields $i/(z-\zeta)$, and hence the sum of the three ray integrals is $i\oint_{\mathrm{clockwise}}q_z(\zeta)/(z-\zeta)d\zeta=-2\pi q_z(z)$. Thus the printed positive prefactor reconstructs $-q_z$. The requested cancellation above holds with either overall sign, but the actual data-dependent derivative is

$$
\boxed{q_z=-\frac i\pi\left[-\int_0^\infty e^{ikz}(k-\gamma)\frac{H(k)}{D(k)}dk+\int_0^{i\infty}e^{ikz}H(k)dk+\int_0^{-\infty}e^{ikz+k\ell}(k+\gamma)\frac{H(k)}{D(k)}dk\right].}
$$

Decay at infinity fixes the integration constant when recovering $q$ from its [Wirtinger derivative](../../../analysis.md#wirtinger-derivatives).

For completeness, the missing condition at infinity and the unrestricted printed $\gamma$ deserve an explicit [solvability of a decaying Robin strip](../../../differential-equation.md#solvability-of-a-decaying-robin-strip) check. Let $Y_n$ be orthonormal [eigenfunctions](../../../linear-operator-theory.md#eigenfunction) from a [Sturm-Liouville problem](../../../analysis.md#sturm-liouville-problem) of $-d^2/dy^2$ with $Y_n'(0)=\gamma Y_n(0)$ and $Y_n'(\ell)=-\gamma Y_n(\ell)$, and eigenvalues $\lambda_n$. With $g_n=\int_0^\ell gY_n\,dy$, [separation of variables](../../../partial-differential-equation.md#separation-of-variables) gives

$$
q(x,y)=-\sum_{\lambda_n>0}\frac{g_n}{\sqrt{\lambda_n}}e^{-\sqrt{\lambda_n}x}Y_n(y),\qquad g_n=0\ \text{required whenever }\lambda_n\leq0.
$$

Indeed, each coefficient obeys $q_n''-\lambda_nq_n=0$ and $q_n'(0)=g_n$. A positive eigenvalue has one decaying exponential; a zero eigenvalue has only affine solutions and a negative eigenvalue only oscillatory solutions, neither of which decays unless its coefficient vanishes. This also proves uniqueness in the decay class and justifies reflection symmetry there. For $\gamma>0$, all eigenvalues are positive. For $\gamma=0$, the constant eigenfunction requires $\int_0^\ell g\,dy=0$; the apparent zero of $D$ at the origin is then removable. For $\gamma<0$, compatibility with every nonpositive eigenmode is necessary. These restrictions cannot be inferred from smoothness and reflection symmetry alone. The printed [boundary value problem](../../../differential-equation.md#boundary-value-problem) without any far-field condition permits additional growing or nondecaying homogeneous solutions, whereas the spectral transforms select the decaying branch.

## 3

↑ **Parent:** [Paper 70](paper-70.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Fix the convention $\Delta q-m^2q=0$, $m>0$, and let $c_m=m^2/4$. With $z=x+iy$, two families of [modified Helmholtz adjoint plane waves](../../../partial-differential-equation.md#modified-helmholtz-adjoint-plane-wave) are

$$
E_+(z,k)=e^{-ikz+ic_m\bar z/k},\qquad E_-(z,k)=e^{ik\bar z-ic_mz/k},\qquad k\ne0.
$$

Both satisfy $\Delta E_\pm=m^2E_\pm$, since the products of their $z$ and $\bar z$ exponents are $m^2/4$. They obey $E_-(z,k)=\overline{E_+(z,\bar k)}$. [Green second identity](../../../partial-differential-equation.md#green-second-identity) gives the two [conjugate global relations for the modified Helmholtz equation](../../../differential-equation.md#conjugate-global-relations-for-the-modified-helmholtz-equation)

$$
\boxed{\mathcal G_\pm(k)=\int_{\partial\Omega}\left(E_\pm\partial_nq-q\partial_nE_\pm\right)ds=0.}
$$

For real boundary traces, $\mathcal G_-(k)=\overline{\mathcal G_+(\bar k)}$. Thus the second identity is the conjugate spectral companion, rather than an unrelated extra boundary condition. In complex differential form the first relation is equivalently

$$
\int_{\partial\Omega}E_+\left[(q_z+ikq)dz-\left(q_{\bar z}-\frac{ic_m}{k}q\right)d\bar z\right]=0.
$$

Its integrand is a closed one-form: differentiating its coefficients gives $2E_+(q_{z\bar z}-c_mq)=0$. This supplies a direct derivation of the [global relation](../../../differential-equation.md#global-relation-for-a-linear-boundary-value-problem) as well as its outward-normal sign convention.

Write the known [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition) on side $j$ as $f_j(s)$ and the unknown outward [normal derivative](../../../differential-geometry.md#normal-derivative) as $h_j(s)$, with $-1<s<1$. For any linear combination $v$ of the adjoint waves, the [global relation](../../../differential-equation.md#global-relation-for-a-linear-boundary-value-problem) is

$$
\sum_j\int_{-1}^1v_j(s)h_j(s)ds=\sum_j\int_{-1}^1f_j(s)\partial_{n_j}v_j(s)ds.
$$

Expanding the $h_j$ in a finite basis and enforcing these identities at selected [collocation points for a global relation](../../../differential-equation.md#collocation-points-for-a-global-relation) gives a linear system with a known right side. The square permits especially simple paired tests.

Let $p_n=n\pi/2$, $\eta_n=\sqrt{m^2+p_n^2}$, and $\varphi_n(s)=\sin[p_n(s+1)]$ for $n\geq1$. Define four real adjoint solutions

$$
\begin{aligned}
v_{B,n}&=e^{-\eta_n(y+1)}\varphi_n(x),&v_{T,n}&=e^{\eta_n(y-1)}\varphi_n(x),\\
v_{L,n}&=e^{-\eta_n(x+1)}\varphi_n(y),&v_{R,n}&=e^{\eta_n(x-1)}\varphi_n(y).
\end{aligned}
$$

They satisfy the [modified Helmholtz equation](../../../partial-differential-equation.md#modified-helmholtz-equation) because $\eta_n^2-p_n^2=m^2$. Each is a linear combination of two adjoint exponentials, hence is obtained from the two spectral [global relations](../../../differential-equation.md#global-relation-for-a-linear-boundary-value-problem). More explicitly, put $\rho_n^\pm=(\eta_n\pm p_n)/2$, so $\rho_n^+\rho_n^-=c_m$. For the $E_+$ convention above, the required spectral pairs are

$$
\boxed{\{\rho_n^+,\rho_n^-\}\ (T),\quad\{-\rho_n^+,-\rho_n^-\}\ (B),\quad\{i\rho_n^+,i\rho_n^-\}\ (R),\quad\{-i\rho_n^+,-i\rho_n^-\}\ (L).}
$$

Appropriate phase-weighted differences produce $\sin[p_n(s+1)]$. For example the top test is $e^{-\eta_n}[e^{ip_n}E_+(\rho_n^-)-e^{-ip_n}E_+(\rho_n^+)]/(2i)$. The conjugate relation ensures a real system for real data. This is [sine collocation of square modified Helmholtz global relations](../../../differential-equation.md#sine-collocation-of-square-modified-helmholtz-global-relations).

The functions $\varphi_n$ are an orthonormal [Fourier sine basis](../../../fourier-series.md#fourier-sine-basis) on $[-1,1]$. Set $h_{j,n}=\int_{-1}^1h_j\varphi_n ds$ and compute the known quantity $R_{j,n}=\int_{\partial\Omega}f\partial_nv_{j,n}ds$ by numerical integration. Since $\varphi_n(\pm1)=0$, each adjoint test vanishes on both adjacent sides. On its own side it equals $\varphi_n$, and on the opposite side it equals $\delta_n\varphi_n$, where $\delta_n=e^{-2\eta_n}$. Thus the [square modified Helmholtz Dirichlet-to-Neumann coefficients](../../../differential-equation.md#square-modified-helmholtz-dirichlet-to-neumann-coefficients) obey

$$
\begin{pmatrix}1&\delta_n\\\delta_n&1\end{pmatrix}\begin{pmatrix}h_{B,n}\\h_{T,n}\end{pmatrix}=\begin{pmatrix}R_{B,n}\\R_{T,n}\end{pmatrix},\qquad
\begin{pmatrix}1&\delta_n\\\delta_n&1\end{pmatrix}\begin{pmatrix}h_{L,n}\\h_{R,n}\end{pmatrix}=\begin{pmatrix}R_{L,n}\\R_{R,n}\end{pmatrix}.
$$

Each block is inverted explicitly: for opposite sides $j,j'$,

$$
\boxed{h_{j,n}=\frac{R_{j,n}-\delta_nR_{j',n}}{1-\delta_n^2}.}
$$

Compute these coefficients for $1\leq n\leq N$ and reconstruct $h_j^{(N)}=\sum_{n=1}^Nh_{j,n}\varphi_n$. This is a semi-analytical scheme: the spectral basis integrals and two-by-two inverses are explicit, while the known boundary integrals are evaluated numerically. Increase $N$ and the quadrature resolution until the desired convergence is observed; compatible smooth side data have convergent normal-trace expansions, while corner singularities require the usual weaker trace interpretation and more careful quadrature.

The requested weak interaction between sides is particularly clear: **the adjacent-side unknown traces contribute exactly zero, and the opposite-side coefficient is $e^{-2\sqrt{m^2+(n\pi/2)^2}}\to0$**. The own-side coefficient stays equal to one. Thus [diagonal dominance of paired square global-relation collocation](../../../differential-equation.md#diagonal-dominance-of-paired-square-global-relation-collocation) is genuine after pairing; individual uncombined exponential samples need not have the same conditioning. The eigenvalues of each block are $1\pm\delta_n$, so its condition number is $(1+\delta_n)/(1-\delta_n)$.

There is also a direct localization check for an individual adjoint wave. On side $j$ with outward unit normal $n_j$ and tangent $t_j$, the normalized test $e^{\eta(n_j\cdot r-1)+ip\,t_j\cdot r}$ has $\eta=\sqrt{m^2+p^2}$. Its opposite-side magnitude is $e^{-2\eta}$, and its magnitude integrates to at most $1/\eta$ along either adjacent side. This [side localization of modified Helmholtz plane waves](../../../partial-differential-equation.md#side-localization-of-modified-helmholtz-plane-waves) explains why suitable large spectral parameters suppress remote-side effects even before the exact sine cancellation.

Finally the interior solution can be evaluated from the computed traces using the [two-dimensional modified Helmholtz fundamental solution](../../../partial-differential-equation.md#two-dimensional-modified-helmholtz-fundamental-solution)

$$
\Gamma_m(r,s)=\frac1{2\pi}K_0(m|r-s|),\qquad q(r)=\int_{\partial\Omega}\left[\Gamma_m(r,s)h(s)-f(s)\partial_{n_s}\Gamma_m(r,s)\right]ds.
$$

Here $K_0$ is the [Modified Bessel function of the second kind](../../../analysis.md#modified-bessel-function-of-the-second-kind), and $(-\Delta+m^2)\Gamma_m=\delta$. Replace $h$ by its computed finite [Fourier sine series](../../../fourier-series.md#fourier-sine-series) and use numerical integration; at interior points the boundary kernels are smooth. The sign follows from [Green second identity](../../../partial-differential-equation.md#green-second-identity) with this fundamental-solution convention. This completes the numerical integration of the [boundary value problem](../../../differential-equation.md#boundary-value-problem) with a [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition), rather than stopping at an equation for its unknown boundary derivatives.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
