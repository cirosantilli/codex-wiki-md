# Paper 2

↑ **Parent:** [2014](../2014.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2014/PaperNST_IB_2.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2014/PaperNST_IB_2.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
    - [a](#1/i/a)
      - [Solution](#1/i/a/solution)
    - [b](#1/i/b)
      - [Solution](#1/i/b/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
    - [a](#1/ii/a)
      - [Solution](#1/ii/a/solution)
    - [b](#1/ii/b)
      - [Solution](#1/ii/b/solution)
    - [c](#1/ii/c)
      - [Solution](#1/ii/c/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
    - [a](#3/ii/a)
      - [Solution](#3/ii/a/solution)
    - [b](#3/ii/b)
      - [Solution](#3/ii/b/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
- [5](#5)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
  - [iii](#5/iii)
    - [Solution](#5/iii/solution)
- [6](#6)
  - [i](#6/i)
    - [Solution](#6/i/solution)
  - [ii](#6/ii)
    - [Solution](#6/ii/solution)
  - [iii](#6/iii)
    - [Solution](#6/iii/solution)
  - [iv](#6/iv)
    - [Solution](#6/iv/solution)
  - [v](#6/v)
    - [Solution](#6/v/solution)
- [7](#7)
  - [i](#7/i)
    - [Solution](#7/i/solution)
  - [ii](#7/ii)
    - [Solution](#7/ii/solution)
- [8](#8)
  - [i](#8/i)
    - [Solution](#8/i/solution)
  - [ii](#8/ii)
    - [Solution](#8/ii/solution)
- [9](#9)
  - [i](#9/i)
    - [Solution](#9/i/solution)
  - [ii](#9/ii)
    - [Solution](#9/ii/solution)
    - [a](#9/ii/a)
      - [Solution](#9/ii/a/solution)
    - [b](#9/ii/b)
      - [Solution](#9/ii/b/solution)
    - [c](#9/ii/c)
      - [Solution](#9/ii/c/solution)
- [10](#10)
  - [i](#10/i)
    - [Solution](#10/i/solution)
  - [ii](#10/ii)
    - [Solution](#10/ii/solution)
  - [iii](#10/iii)
    - [Solution](#10/iii/solution)
  - [iv](#10/iv)
    - [Solution](#10/iv/solution)

## 1

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

For the [weighted inner product](../../inner-product.md#weighted-inner-product), the factor $w$ cancels the $w^{-1}$ in the [Sturm-Liouville operator](../../sturm-liouville-theory.md#sturm-liouville-operator). Assuming the coefficients are real, two applications of [integration by parts](../../calculus.md#integration-by-parts) give

$$
\begin{aligned}
\langle f,Lg\rangle_w-\langle Lf,g\rangle_w
&=\int_a^b[-f^*(pg')'+(pf'^*)'g]dx\\
&=\left[p(f'^*g-f^*g')\right]_a^b.
\end{aligned}
$$

This is the boundary form in the [Lagrange identity for a Sturm-Liouville operator](../../sturm-liouville-theory.md#lagrange-identity-for-a-sturm-liouville-operator). The potential terms cancel; if $q$ were complex, an additional integral of $(q-q^*)f^*g$ would remain, so suitable real coefficients are part of formal self-adjointness. The endpoint restrictions in part (a) eliminate the displayed form for every pair of functions in the domain.

<h4 id="1/i/a">a</h4>

↑ **Parent:** [I](#1/i)

<h5 id="1/i/a/solution">Solution</h5>

↑ **Parent:** [A](#1/i/a)

The necessary boundary identity for a [self-adjoint operator](../../linear-operator-theory.md#self-adjoint-operator) is

$$
\boxed{\left[p(f'^*g-f^*g')\right]_a^b=0\quad\text{for every admissible }f,g.}
$$

At regular endpoints, a standard full family of separated self-adjoint conditions is

$$
\boxed{\alpha_a y(a)+\beta_a p(a)y'(a)=0,\qquad\alpha_b y(b)+\beta_b p(b)y'(b)=0,}
$$

with real coefficients and neither pair $(\alpha_a,\beta_a)$, $(\alpha_b,\beta_b)$ zero. For example, if $\beta_a\ne0$, both functions obey $pf'=-\alpha_a f/\beta_a$ at $a$, so $pf'^*g-pf^*g'=0$ there. The cases $\beta_a=0$ and the endpoint $b$ follow directly. These include [Dirichlet boundary conditions](../../differential-equation.md#dirichlet-boundary-condition), [Neumann boundary conditions](../../differential-equation.md#neumann-boundary-condition) and [Robin boundary conditions](../../differential-equation.md#robin-boundary-condition).

Separate vanishing at each endpoint is sufficient but not necessary. Coupled conditions such as $y(b)=e^{i\chi}y(a)$ and $p(b)y'(b)=e^{i\chi}p(a)y'(a)$, with real $\chi$, make the two endpoint forms equal and hence their difference zero. More generally the allowed endpoint data must be a maximal subspace on which the boundary form vanishes; this ensures that the adjoint has the same domain. Merely imposing extra endpoint restrictions until the boundary term vanishes proves symmetry, but can overrestrict the domain and fail to give self-adjointness.

<h4 id="1/i/b">b</h4>

↑ **Parent:** [I](#1/i)

<h5 id="1/i/b/solution">Solution</h5>

↑ **Parent:** [B](#1/i/b)

Let $Ly_n=\lambda_ny_n$. By self-adjointness,

$$
\lambda_n\langle y_m,y_n\rangle_w=\langle y_m,Ly_n\rangle_w=\langle Ly_m,y_n\rangle_w=\lambda_m^*\langle y_m,y_n\rangle_w.
$$

Taking $m=n$ first shows that each [eigenvalue](../../linear-operator-theory.md#eigenvalue) is real: $\langle y_n,y_n\rangle_w>0$ for a nonzero [eigenfunction](../../linear-operator-theory.md#eigenfunction), since $w>0$. Therefore

$$
(\lambda_n-\lambda_m)\langle y_m,y_n\rangle_w=0.
$$

For distinct eigenvalues this proves [orthogonality of Sturm-Liouville eigenfunctions](../../sturm-liouville-theory.md#orthogonality-of-sturm-liouville-eigenfunctions):

$$
\boxed{\int_a^b y_m^*(x)y_n(x)w(x)\,dx=0\quad(\lambda_m\ne\lambda_n).}
$$

The weight is essential: this need not be orthogonality under the unweighted integral.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The useful coordinate for this scale-dependent differential operator is $t=\ln x$. With $Y(t)=y(e^t)$, the [chain rule](../../calculus.md#chain-rule) gives

$$
xy'=Y_t,\qquad x^2y''=Y_{tt}-Y_t,\qquad Ly=-Y_{tt}-Y.
$$

The interval becomes $0\leq t\leq1$, and the endpoint values become $Y(0)=Y(1)=0$. This [logarithmic change of variable in a Sturm-Liouville problem](../../linear-ordinary-differential-equation.md#logarithmic-change-of-variable-in-a-sturm-liouville-problem) reduces the calculation to a constant-coefficient Dirichlet problem. Also $dx/x=dt$, so the transformation preserves the appropriate [weighted inner product](../../inner-product.md#weighted-inner-product).

<h4 id="1/ii/a">a</h4>

↑ **Parent:** [Ii](#1/ii)

<h5 id="1/ii/a/solution">Solution</h5>

↑ **Parent:** [A](#1/ii/a)

Divide the eigenvalue equation by $x$ and collect the first two derivative terms into a single derivative:

$$
-(xy')'-\frac yx=\lambda\frac yx.
$$

Thus one choice of [Sturm-Liouville form](../../sturm-liouville-theory.md#sturm-liouville-form) is

$$
\boxed{p(x)=x,\qquad q(x)=-\frac1x,\qquad w(x)=\frac1x,\qquad 1\leq x\leq e.}
$$

Indeed $w^{-1}[-(py')'+qy]=-x^2y''-xy'-y$. Both $p$ and $w$ are positive and regular throughout this interval. The zero endpoint values make the boundary form vanish.

<h4 id="1/ii/b">b</h4>

↑ **Parent:** [Ii](#1/ii)

<h5 id="1/ii/b/solution">Solution</h5>

↑ **Parent:** [B](#1/ii/b)

In logarithmic coordinates the [eigenvalue problem](../../linear-operator-theory.md#eigenvalue-problem) becomes $-Y''=(\lambda+1)Y$. A nonzero function with zero values at both ends requires $\lambda+1>0$: multiplying by $Y^*$ and integrating gives $(\lambda+1)\int_0^1|Y|^2dt=\int_0^1|Y'|^2dt>0$. Write $\kappa=\sqrt{\lambda+1}$. The first endpoint gives $Y=A\sin\kappa t$, and the second requires $\kappa=n\pi$, $n=1,2,\ldots$.

For [vector normalization](../../vector-space.md#vector-normalization), $\int_1^e|y|^2dx/x=|A|^2\int_0^1\sin^2(n\pi t)dt=|A|^2/2$. A positive real normalization constant therefore gives

$$
\boxed{\lambda_n=n^2\pi^2-1,\qquad y_n(x)=\sqrt2\sin(n\pi\ln x),\quad n\geq1.}
$$

The sine [orthogonality](../../inner-product.md#orthogonal-vectors) identity also gives $\int_1^ey_m y_n\,dx/x=\delta_{mn}$. Completeness is the usual completeness of the [Fourier sine series](../../fourier-series.md#fourier-sine-series) on $(0,1)$ under the logarithmic coordinate transformation.

<h4 id="1/ii/c">c</h4>

↑ **Parent:** [Ii](#1/ii)

<h5 id="1/ii/c/solution">Solution</h5>

↑ **Parent:** [C](#1/ii/c)

Expand the forcing and the solution in the normalized [eigenfunctions](../../linear-operator-theory.md#eigenfunction): $1=\sum_n b_ny_n$ and $y=\sum_n c_ny_n$. Their coefficients are

$$
b_n=\int_1^e y_n(x)\frac{dx}{x}=\sqrt2\int_0^1\sin(n\pi t)dt=\frac{\sqrt2[1-(-1)^n]}{n\pi}.
$$

Since all $\lambda_n=n^2\pi^2-1$ are nonzero, the equation gives $c_n=b_n/\lambda_n$. Hence the required [Sturm-Liouville eigenfunction expansion](../../sturm-liouville-theory.md#sturm-liouville-eigenfunction-expansion) is

$$
\boxed{y(x)=\sum_{\substack{n\geq1\\n\text{ odd}}}\frac{4\sin(n\pi\ln x)}{n\pi(n^2\pi^2-1)}.}
$$

This is [constant forcing in a logarithmic Dirichlet Sturm-Liouville problem](../../linear-ordinary-differential-equation.md#constant-forcing-in-a-logarithmic-dirichlet-sturm-liouville-problem). The coefficients are $O(n^{-3})$, so the solution series converges uniformly and has zero endpoint values. Applying $L$ is justified in the weighted square-integrable sense; the forcing sine series equals one at interior points, while its endpoint sums are zero. The equation is imposed in the interior, so this does not contradict the boundary conditions.

As an independent check, solving $-Y''-Y=1$ directly gives

$$
y(x)=\frac{\cos(\ln x-1/2)}{\cos(1/2)}-1.
$$

It has both zero endpoint values and satisfies $Ly=1$. The invertibility of the Dirichlet operator makes it the same solution as the expansion.

## 2

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Use [separation of variables](../../partial-differential-equation.md#separation-of-variables), writing $\Psi=F(r)\Theta(\theta)$. After multiplication by $r^2/(F\Theta)$, the radial and angular terms are functions of independent variables, so set

$$
\frac{(r^2F')'}F=-\frac{(\sin\theta\,\Theta')'}{\sin\theta\,\Theta}=\lambda.
$$

With $x=\cos\theta$, the angular equation is

$$
\frac d{dx}\left[(1-x^2)\frac{d\Theta}{dx}\right]+\lambda\Theta=0.
$$

Regularity at both poles selects $\lambda=\ell(\ell+1)$, $\ell=0,1,\ldots$, and the [Legendre polynomials](../../linear-ordinary-differential-equation.md#legendre-polynomial) $P_\ell(x)$; the other angular branch is singular at a pole. The radial [Euler-Cauchy equation](../../linear-ordinary-differential-equation.md#euler-cauchy-equation) is $r^2F''+2rF'-\ell(\ell+1)F=0$. A power $r^s$ gives $(s-\ell)(s+\ell+1)=0$, hence $F=a_\ell r^\ell+b_\ell r^{-\ell-1}$.

Superposing these axisymmetric [spherical harmonics](../../analysis.md#spherical-harmonic) gives

$$
\boxed{\Psi(r,\theta)=\sum_{\ell=0}^\infty\left(a_\ell r^\ell+\frac{b_\ell}{r^{\ell+1}}\right)P_\ell(\cos\theta).}
$$

The coefficients must give convergence appropriate to the domain. In a region containing the origin, regularity removes the negative powers; in an exterior region with zero potential at infinity, it removes the growing powers and the constant. No such radial restriction is needed for a general annular region.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Resolve the angular [surface charge density](../../electrostatics.md#surface-charge-density) into [Legendre polynomials](../../linear-ordinary-differential-equation.md#legendre-polynomial):

$$
\sin^2\theta=\frac23[1-P_2(\cos\theta)],\qquad \sigma_0=\frac{2A}{3},\quad\sigma_2=-\frac{2A}{3}.
$$

For a single degree $\ell$, write the common surface potential as $V_\ell P_\ell$. Regularity and decay require radial factors $(r/R)^\ell$ inside and $(R/r)^{\ell+1}$ outside. Their exterior-minus-interior radial derivative at $R$ is $-(2\ell+1)V_\ell P_\ell/R$. Thus [spherical harmonic matching with a derivative jump](../../partial-differential-equation.md#spherical-harmonic-matching-with-a-derivative-jump) gives $V_\ell=R\sigma_\ell/(2\ell+1)$.

Only degrees zero and two occur, yielding

$$
\boxed{\begin{aligned}
\Psi_{\rm in}(r,\theta)&=\frac{2AR}{3}-\frac{2A}{15R}r^2P_2(\cos\theta),&&r<R,\\
\Psi_{\rm out}(r,\theta)&=\frac{2AR^2}{3r}-\frac{2AR^4}{15r^3}P_2(\cos\theta),&&r>R.
\end{aligned}}
$$

Both expressions have surface value $2AR/3-2AR P_2/15$, and their derivative difference is $-2A/3+(2A/3)P_2=-A\sin^2\theta$, checking both interface conditions. The interior quadratic is regular at the origin, and the exterior potential tends to zero.

The leading far-field term is the monopole term. Indeed the total charge is $Q=R^2\int\sigma\,d\Omega=8\pi AR^2/3$, and the normalization of the specified jump gives $Q/(4\pi r)=2AR^2/(3r)$. No extra permittivity factor is inserted into the supplied normalization. Regularity here means finite piecewise smooth potential; its normal derivative necessarily jumps at the charged surface.

## 3

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

For the [vector field](../../multivariable-calculus.md#vector-field) $F=\phi\nabla\psi-\psi\nabla\phi$, the [product rule](../../calculus.md#product-rule) gives

$$
\nabla\cdot F=\nabla\phi\cdot\nabla\psi+\phi\nabla^2\psi-\nabla\psi\cdot\nabla\phi-\psi\nabla^2\phi=\phi\nabla^2\psi-\psi\nabla^2\phi.
$$

The mixed [dot products](../../inner-product.md#dot-product) cancel. The [divergence theorem](../../multivariable-calculus.md#divergence-theorem) therefore yields [Green's second identity](../../partial-differential-equation.md#green-second-identity),

$$
\boxed{\int_V(\phi\nabla^2\psi-\psi\nabla^2\phi)dV=\int_S(\phi\,\hat n\cdot\nabla\psi-\psi\,\hat n\cdot\nabla\phi)dS.}
$$

The fields and boundary are assumed sufficiently regular. A singular [Green function](../../green-s-function.md) can be treated by excising a small ball around its source and taking the radius to zero, or using [distributions](../../distribution-theory.md#distribution-mathematical-analysis).

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Fix the evaluation point $r'$ inside $V$ and put $\psi(r)=G(r,r')$ in [Green's second identity](../../partial-differential-equation.md#green-second-identity). The two $k^2$ terms cancel because $\nabla^2\phi=-k^2\phi$ and $\nabla^2G=\delta^{(3)}-k^2G$. The remaining volume integral is $\int\phi(r)\delta^{(3)}(r-r')dV=\phi(r')$. Thus

$$
\phi(r')=\int_S[\phi(r)\partial_{n_r}G(r,r')-G(r,r')\partial_n\phi(r)]dS.
$$

The [Dirac delta](../../distribution-theory.md#dirac-delta-function) has a positive sign in this problem's Green-function equation, fixing the order of the two terms. All boundary derivatives act on the integration variable $r$.

<h4 id="3/ii/a">a</h4>

↑ **Parent:** [Ii](#3/ii)

<h5 id="3/ii/a/solution">Solution</h5>

↑ **Parent:** [A](#3/ii/a)

Impose a homogeneous [Dirichlet boundary condition](../../differential-equation.md#dirichlet-boundary-condition) on the Green function in its first variable, $G(r,r')=0$ for $r\in S$. The second boundary term then vanishes, giving

$$
\boxed{\phi(r')=\int_S\phi(r)\partial_{n_r}G(r,r')\,dS.}
$$

In a bounded domain, a Dirichlet Green function requires $k^2$ not to be a Dirichlet eigenvalue of $-\Delta$; otherwise a resonance can obstruct its existence. The representation assumes such a Green function exists.

In all space, put $\rho=|r-r'|$ and try $G=Ae^{ik\rho}/\rho$. For $\rho>0$, direct differentiation gives $(\rho^2G')'+k^2\rho^2G=0$, so the [Helmholtz equation](../../partial-differential-equation.md#helmholtz-equation) holds away from the source. Integrate its inhomogeneous version over a small source-centred ball. The $k^2G$ volume integral tends to zero, while the flux is

$$
\lim_{\varepsilon\downarrow0}4\pi\varepsilon^2G'(\varepsilon)=-4\pi A.
$$

It must equal the integrated delta, one. Therefore

$$
\boxed{A=-\frac1{4\pi},\qquad G(r,r')=-\frac{e^{ik|r-r'|}}{4\pi|r-r'|}.}
$$

This is the negative of the convention used in the [outgoing Green function for the three-dimensional Helmholtz equation](../../partial-differential-equation.md#outgoing-green-function-for-the-three-dimensional-helmholtz-equation), where the source is $-\delta$. The sign here follows the present $+\delta$ convention. The factor $e^{ik\rho}$ chooses the outgoing solution, with time convention $e^{-i\omega t}$ and the [Sommerfeld radiation condition](../../inverse-problem.md#sommerfeld-radiation-condition); one could add homogeneous solutions without a radiation prescription.

<h4 id="3/ii/b">b</h4>

↑ **Parent:** [Ii](#3/ii)

<h5 id="3/ii/b/solution">Solution</h5>

↑ **Parent:** [B](#3/ii/b)

Reflect $r'=(x',y',z')$ to $r'^*=(x',y',-z')$. The [method of images](../../mathematics.md#method-of-images) gives the [Dirichlet image kernel for the three-dimensional Helmholtz equation](../../partial-differential-equation.md#dirichlet-image-kernel-for-the-three-dimensional-helmholtz-equation):

$$
\boxed{G_D(r,r')=-\frac1{4\pi}\left[\frac{e^{ik|r-r'|}}{|r-r'|}-\frac{e^{ik|r-r'^*|}}{|r-r'^*|}\right].}
$$

The two distances coincide on the plane, so its boundary value is zero; the image source is outside the domain. It therefore has the required positive delta source inside and the selected outgoing behaviour.

Let $h(R)=e^{ikR}/R$. At a boundary point $r=(\xi,\eta,0)$, the distances to the real and reflected sources have $z$ derivatives $-z'/R$ and $+z'/R$. Thus

$$
\partial_zG_D=\frac{z'}{2\pi R}h'(R),\qquad h'(R)=\frac{e^{ikR}}R\left(ik-\frac1R\right).
$$

The outward [unit normal](../../differential-geometry.md#unit-normal) of the upper half-space is $-e_z$, and $z'/R=\cos\theta$. Hence

$$
\partial_nG_D=-\frac{ik}{2\pi}\frac{e^{ikR}}R\left(1+\frac{i}{kR}\right)\cos\theta.
$$

Using the decay assumption to discard the distant hemisphere in the boundary representation gives

$$
\boxed{\phi(r')=-\frac{ik}{2\pi}\int_{z=0}\frac{e^{ikR}}R\left(1+\frac{i}{kR}\right)\cos\theta\,\phi(r)\,dS.}
$$

The qualification at infinity concerns the whole Green boundary term, not just the pointwise limit of $\phi$. Sufficient decay of the field and its derivatives, as assumed, makes it vanish; compatible radiation conditions can also do so. As a sign check, taking $k\to0$ in the kernel gives $z'/(2\pi R^3)$, the positive [Poisson kernel for the upper half-space](../../partial-differential-equation.md#poisson-kernel-for-the-upper-half-space).

## 4

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Put $d=\sqrt{a^2-b^2}>0$. The two roots are

$$
z_{\rm in}=-i\frac{a-d}{b},\qquad z_{\rm out}=-i\frac{a+d}{b}.
$$

Since $(a-d)(a+d)=b^2$, their moduli are $b/(a+d)<1$ and $(a+d)/b>1$. Thus exactly one root is inside the unit circle, and neither lies on it.

For the real integral use $z=e^{i\theta}$, so $\sin\theta=(z-z^{-1})/(2i)$ and $d\theta=dz/(iz)$. The [change of variables](../../multivariable-calculus.md#change-of-variables-formula) gives

$$
\int_0^{2\pi}\frac{d\theta}{a+b\sin\theta}=\oint_{|z|=1}\frac{2\,dz}{bz^2+2iaz-b}.
$$

The contour is counterclockwise. At its single interior [simple pole](../../isolated-singularity.md#simple-pole), the [residue](../../analysis.md#residue) is

$$
\frac{2}{2bz_{\rm in}+2ia}=\frac1{id}.
$$

By the [residue theorem](../../analysis.md#residue-theorem), the [reciprocal affine sine integral](../../complex-analysis.md#reciprocal-affine-sine-integral) is therefore

$$
\boxed{\int_0^{2\pi}\frac{d\theta}{a+b\sin\theta}=2\pi i\frac1{id}=\frac{2\pi}{\sqrt{a^2-b^2}}.}
$$

The condition $a>b>0$ also makes the real denominator strictly positive, consistent with the positive answer and the absence of contour poles on the unit circle.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Use the principal [branch of the complex logarithm](../../analysis.md#branch-of-the-complex-logarithm) for $\operatorname{Log}(z+i)$. Its [branch cut](../../analysis.md#branch-cut) is the ray $z=-i-s$, $s\geq0$, lying below the real axis. Thus it is analytic in the upper half-plane, where the only [pole](../../isolated-singularity.md#pole) of the integrand is $z=i$.

Close the real interval by a large upper semicircle. The [estimation lemma](../../complex-analysis.md#estimation-lemma) bounds the arc integral by $O(\ln R/R)$, so it vanishes. The simple-pole [residue](../../analysis.md#residue) is

$$
\operatorname{Res}_{z=i}\frac{\operatorname{Log}(z+i)}{z^2+1}=\frac{\operatorname{Log}(2i)}{2i}=\frac{\ln2+i\pi/2}{2i}.
$$

The [residue theorem](../../analysis.md#residue-theorem) then gives

$$
\int_{-\infty}^{\infty}\frac{\operatorname{Log}(x+i)}{x^2+1}dx=\pi\ln2+\frac{i\pi^2}{2}.
$$

For real $x$, $\operatorname{Re}\operatorname{Log}(x+i)=\tfrac12\ln(x^2+1)$. Taking real parts and then using evenness of the real integrand yields

$$
\boxed{\int_0^\infty\frac{\ln(x^2+1)}{x^2+1}dx=\pi\ln2.}
$$

Both endpoints converge: the integrand is $O(x^2)$ near zero and $O(\ln x/x^2)$ at infinity. This also agrees with the [logarithmic parameter integral with Cauchy weight](../../analysis.md#logarithmic-parameter-integral-with-cauchy-weight) at parameter one.

## 5

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

The [Fourier transform](../../fourier-transform.md) of $u_{xx}$ is $-k^2\widetilde u$: two [integrations by parts](../../calculus.md#integration-by-parts) have no boundary terms under the stated decay assumption. Time differentiation commutes with the spatial transform. Therefore

$$
\boxed{\widetilde u_{tt}+2\gamma\widetilde u_t+(\gamma^2+c^2k^2)\widetilde u=0.}
$$

For every fixed spatial [wavenumber](../../wave-equation.md#wavenumber) $k$, this is a constant-coefficient [ordinary differential equation](../../differential-equation.md#ordinary-differential-equation) in time.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

The characteristic polynomial is $(r+\gamma)^2+c^2k^2$, with roots $r=-\gamma\pm ick$. For $ck\ne0$, the transformed general solution is

$$
\boxed{\widetilde u(k,t)=e^{-\gamma t}\big[A(k)e^{-ickt}+B(k)e^{ickt}\big].}
$$

The repeated-root case $ck=0$ is $e^{-\gamma t}[A_0+B_0t]$, rather than two independent copies of the same exponential. An alternative basis regular at $k=0$ is $e^{-\gamma t}[C(k)\cos(ckt)+D(k)\sin(ckt)/(ck)]$, using the limit $t$ for the last factor at zero.

For $c\ne0$, the [Fourier shift theorem](../../fourier-transform.md#fourier-shift-theorem) turns the two exponential factors into translations. Equivalently, set $v=e^{\gamma t}u$; then $v_{tt}=c^2v_{xx}$. The [D'Alembert formula](../../wave-equation.md#d-alembert-s-formula) gives the general form

$$
\boxed{u(x,t)=e^{-\gamma t}[F(x-|c|t)+G(x+|c|t)],\qquad c\ne0,}
$$

where $F,G$ are arbitrary functions with the required regularity and decay. The arbitrary profiles can accommodate a spatially transformed zero-frequency velocity by their integral components; the isolated repeated root must not be used to discard that degree of freedom. If $c=0$, the equation instead has $u=e^{-\gamma t}[F(x)+tG(x)]$.

This is the [exponentially conjugated wave equation](../../wave-equation.md#exponentially-conjugated-wave-equation). Positive $\gamma$ produces damping, but the algebra also covers negative $\gamma$, which gives exponential amplification. The sign of $c$ is immaterial because the differential equation contains only $c^2$.

<h3 id="5/iii">iii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5/iii)

The initial profile is $f(x)=e^{-|x|}$, with the absolute value confirmed in the original PDF. Its [Fourier transform](../../fourier-transform.md) is

$$
\widetilde f(k)=\int_0^\infty e^{-x}(e^{-ikx}+e^{ikx})dx=\frac{2}{1+k^2}.
$$

Using $\widetilde u_t(k,0)=0$ in the regular cosine-sine form gives

$$
\widetilde u(k,t)=\frac{2e^{-\gamma t}}{1+k^2}\left[\cos(ckt)+\gamma\frac{\sin(ckt)}{ck}\right],
$$

with the quotient interpreted as $t$ when $ck=0$. Put $v_0=|c|>0$. Inverting, or applying the [D'Alembert formula](../../wave-equation.md#d-alembert-s-formula) to $e^{\gamma t}u$, whose initial velocity is $\gamma f$, gives

$$
\boxed{u(x,t)=\frac{e^{-\gamma t}}2\left[e^{-|x-v_0t|}+e^{-|x+v_0t|}+\frac{\gamma}{v_0}\int_{x-v_0t}^{x+v_0t}e^{-|s|}ds\right].}
$$

For an explicit expression at $t\geq0$, let $r=|x|$ and $s=v_0t$. The integral is $2e^{-r}\sinh s$ for $r\geq s$ and $2(1-e^{-s}\cosh r)$ for $r\leq s$. Therefore

$$
\boxed{u(x,t)=e^{-\gamma t}\begin{cases}
e^{-r}\left[\cosh(v_0t)+\dfrac{\gamma}{v_0}\sinh(v_0t)\right],&r\geq v_0t,\\[3pt]
e^{-v_0t}\cosh r+\dfrac{\gamma}{v_0}\left[1-e^{-v_0t}\cosh r\right],&r\leq v_0t.
\end{cases}}
$$

The branches agree at $r=v_0t$. At zero time, the integral vanishes and the translated profiles coincide, recovering $f$. Their time derivatives cancel, while the integral contributes $\gamma f$, cancelling the derivative of the prefactor, so $u_t(x,0)=0$.

For $c=0$ the limiting answer is $u=(1+\gamma t)e^{-\gamma t}e^{-|x|}$. The cusp in $f$ means the solution is understood as a [weak solution](../../partial-differential-equation.md#weak-solution), classically smooth away from the characteristic fronts $x=\pm v_0t$; it is not globally twice differentiable. No assumption that $\gamma$ is positive is needed for this initial-value solution.

## 6

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6/i">i</h3>

↑ **Parent:** [6](#6)

<h4 id="6/i/solution">Solution</h4>

↑ **Parent:** [I](#6/i)

For a constant orthogonal Cartesian change of coordinates $x'_i=Q_{ij}x_j$, the [tensor component transformation law](../../general-relativity.md#tensor-component-transformation-law) for order $n$ is

$$
\boxed{T'_{i_1\cdots i_n}=Q_{i_1j_1}\cdots Q_{i_nj_n}T_{j_1\cdots j_n}.}
$$

Repeated indices are summed. In Cartesian orthonormal coordinates the metric identifies upper and lower indices, so the same orthogonal matrix acts on every index.

An [isotropic tensor](../../multilinear-algebra.md#isotropic-tensor) has the same numerical components after every proper orthogonal change of axes: $Q^{\otimes n}T=T$ for every $Q$ with $Q^TQ=I$ and $\det Q=1$. For example, $\delta_{ij}$ is isotropic because $Q_{ik}Q_{jk}=\delta_{ij}$. Some conventions require invariance under all orthogonal transformations, including reflections; this stronger convention must be distinguished for odd-order tensors, notably the [Levi-Civita symbol](../../multivariable-calculus.md#levi-civita-symbol), which is invariant under proper rotations but changes sign under its ordinary three-index transformation for a reflection.

<h3 id="6/ii">ii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6/ii)

Under the same Cartesian change, a [vector field](../../multivariable-calculus.md#vector-field) has $u'_i(x')=Q_{ip}u_p(x)$ with $x=Q^Tx'$. The [chain rule](../../calculus.md#chain-rule) gives $\partial/\partial x'_j=Q_{jq}\partial/\partial x_q$. Since $Q$ is constant,

$$
\boxed{\frac{\partial u'_i}{\partial x'_j}=Q_{ip}Q_{jq}\frac{\partial u_p}{\partial x_q}.}
$$

This is exactly the order-two [tensor component transformation law](../../general-relativity.md#tensor-component-transformation-law). Thus the Cartesian vector gradient is a [Cartesian second-rank tensor](../../multilinear-algebra.md#cartesian-second-rank-tensor), as in the [velocity gradient tensor](../../fluid-mechanics.md#velocity-gradient-tensor) when $u$ is a velocity field.

The restriction to Cartesian transformations matters. In a general position-dependent basis, differentiating the basis contributes extra terms, so the tensorial derivative is the [covariant derivative](../../general-relativity.md#covariant-derivative), not an arbitrary array of partial derivatives.

<h3 id="6/iii">iii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#6/iii)

An [axial vector](../../vector-space.md#pseudovector) transforms under an orthogonal matrix $Q$ as

$$
\boxed{a'_i=(\det Q)Q_{ij}a_j.}
$$

For a proper rotation, $\det Q=1$, so this is the usual [polar vector](../../vector-space.md#polar-vector) rule. Under an orientation-reversing change, the extra sign distinguishes the two. In particular, spatial inversion leaves an axial vector unchanged while reversing a polar vector.

Let $C_i=(\nabla\times u)_i=\epsilon_{ijk}\partial_j u_k$. The determinant identity for the [Levi-Civita symbol](../../multivariable-calculus.md#levi-civita-symbol) is

$$
\epsilon_{ijk}Q_{jp}Q_{kq}=(\det Q)Q_{ir}\epsilon_{rpq}.
$$

It follows by multiplying the three-index determinant identity by $Q_{ir}$ and using orthogonality. The derivative transformation from part (ii) then gives

$$
\boxed{C'_i=\epsilon_{ijk}Q_{jp}Q_{kq}\partial_pu_q=(\det Q)Q_{ir}C_r.}
$$

Hence the [curl](../../multivariable-calculus.md#curl) of a polar vector field is an axial vector field. The Levi-Civita determinant factor is exactly the extra sign required under reflections.

<h3 id="6/iv">iv</h3>

↑ **Parent:** [6](#6)

<h4 id="6/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#6/iv)

Write $A_{ij}=\partial_j u_i$. The trace fixes the isotropic part, and splitting the remaining matrix into its symmetric and antisymmetric parts gives the [scalar, symmetric-traceless and axial tensor decomposition](../../multilinear-algebra.md#scalar-symmetric-traceless-and-axial-tensor-decomposition):

$$
\boxed{p=\frac13\partial_i u_i,\qquad s_{ij}=\frac12(\partial_j u_i+\partial_i u_j)-\frac13(\partial_k u_k)\delta_{ij}.}
$$

Here $s_{ij}=s_{ji}$ and $s_{ii}=0$. The antisymmetric part is $a_{ij}=(\partial_j u_i-\partial_i u_j)/2$. Its associated axial vector is

$$
\boxed{\omega_k=\frac12\epsilon_{kij}\partial_j u_i=-\frac12(\nabla\times u)_k.}
$$

Indeed the contraction identity $\epsilon_{ijk}\epsilon_{k\ell m}=\delta_{i\ell}\delta_{jm}-\delta_{im}\delta_{j\ell}$ gives $\epsilon_{ijk}\omega_k=(\partial_j u_i-\partial_i u_j)/2$. Adding the three parts reconstructs $A_{ij}$.

**The minus sign is required by the index order** $A_{ij}=\partial_j u_i$. The [symmetric gradient and curl decomposition](../../multilinear-algebra.md#symmetric-gradient-and-curl-decomposition) written instead for $\partial_i u_j$ has the opposite axial sign. The [divergence](../../multivariable-calculus.md#divergence) supplies $3p$, the trace-free symmetric part describes shape change, and the antisymmetric part describes local rotation.

<h3 id="6/v">v</h3>

↑ **Parent:** [6](#6)

<h4 id="6/v/solution">Solution</h4>

↑ **Parent:** [V](#6/v)

Direct differentiation gives

$$
A=\begin{pmatrix}0&a&0\\b&0&0\\0&0&0\end{pmatrix},\qquad p=0,\qquad s=\begin{pmatrix}0&(a+b)/2&0\\(a+b)/2&0&0\\0&0&0\end{pmatrix}.
$$

The [curl](../../multivariable-calculus.md#curl) is $(0,0,b-a)$, so the preceding convention gives

$$
\boxed{\omega=(0,0,(a-b)/2).}
$$

Put $h=(a+b)/2$. The normalized [principal axes](../../rigid-body-dynamics.md#principal-axis) and [eigenvalues](../../linear-operator-theory.md#eigenvalue) of the [symmetric tensor](../../multilinear-algebra.md#symmetric-tensor) $s$ are

$$
\boxed{\begin{array}{c|c}
\text{axis}&\text{principal value}\\\hline
(1,1,0)/\sqrt2&h\\
(1,-1,0)/\sqrt2&-h\\
(0,0,1)&0
\end{array}.}
$$

The planar axes lie along the two angle bisectors of the coordinate axes. If $h\ne0$, one planar direction extends and the perpendicular direction contracts, with no change along the third axis. The labels need not be ordered by size when $h<0$. If $a+b=0$, then $s=0$, all principal values vanish and any orthonormal frame is a principal frame; the flow is pure local rotation in the plane.

## 7

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7/i">i</h3>

↑ **Parent:** [7](#7)

<h4 id="7/i/solution">Solution</h4>

↑ **Parent:** [I](#7/i)

The [kinetic energy](../../energy.md#kinetic-energy) is $T=m\sum_i\dot z_i^2/2$. Differentiating the quadratic [potential energy](../../energy.md#potential-energy) gives the equations for [small oscillations](../../lagrangian-mechanics.md#small-oscillation),

$$
m\ddot z+\frac\tau\ell Kz=0,\qquad K=\begin{pmatrix}2&-1&0\\-1&2&-1\\0&-1&2\end{pmatrix}.
$$

Put $z=v\cos(\omega t+\varphi)$ and $\lambda=m\ell\omega^2/\tau$. The [eigenvalue problem](../../linear-operator-theory.md#eigenvalue-problem) is $Kv=\lambda v$. Its characteristic polynomial is

$$
\det(K-\lambda I)=(2-\lambda)[(2-\lambda)^2-2].
$$

Thus a convenient set of [normal modes](../../wave-equation.md#normal-mode) is

$$
\boxed{\begin{array}{c|c|c}
\text{mode}&\text{relative bead displacements}&\omega^2\\\hline
1&(1,\sqrt2,1)&\dfrac\tau{m\ell}(2-\sqrt2)\\[2pt]
2&(1,0,-1)&\dfrac{2\tau}{m\ell}\\[2pt]
3&(1,-\sqrt2,1)&\dfrac\tau{m\ell}(2+\sqrt2)
\end{array}.}
$$

Each shape can be multiplied by an arbitrary sinusoidal time amplitude. In the lowest mode all beads move in phase. In the middle mode the central bead is fixed and the outer beads move oppositely. In the highest mode the two outer beads move together against the centre. These vectors are mutually orthogonal and span the three displacement coordinates.

<a id="7/i/image-the-three-transverse-string-modes-the-dashed-line-is-equilibrium-and-bead-displacements-share-one-arbitrary-scale"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2-2014-ib-string-modes.png)

**[Figure 1](#7/i/image-the-three-transverse-string-modes-the-dashed-line-is-equilibrium-and-bead-displacements-share-one-arbitrary-scale). The three transverse string modes; the dashed line is equilibrium and bead displacements share one arbitrary scale**.

These are the three-mass case of the [normal modes of a uniformly loaded finite string](../../wave-equation.md#normal-modes-of-a-uniformly-loaded-finite-string), with discrete sine shapes $v_i^{(j)}=\sin(ij\pi/4)$. The sketches use straight string segments between masses and fixed zero displacements at the walls. The small-slope and constant-tension assumptions justify the quadratic energy and linear equations.

<h3 id="7/ii">ii</h3>

↑ **Parent:** [7](#7)

<h4 id="7/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#7/ii)

Resolve the initial displacement into the mode shapes from part (i):

$$
(0,a,0)^T=\frac{a}{2\sqrt2}(1,\sqrt2,1)^T-\frac{a}{2\sqrt2}(1,-\sqrt2,1)^T.
$$

There is no component along $(1,0,-1)$: the initial displacement is invariant under exchanging beads 1 and 3, whereas that mode is antisymmetric. Zero initial velocities select cosine time dependence. Therefore

$$
\boxed{\begin{aligned}
z_1(t)=z_3(t)&=\frac{a}{2\sqrt2}[\cos(\omega_1t)-\cos(\omega_3t)],\\
z_2(t)&=\frac a2[\cos(\omega_1t)+\cos(\omega_3t)].
\end{aligned}}
$$

Here $\omega_1=\sqrt{\tau(2-\sqrt2)/(m\ell)}$ and $\omega_3=\sqrt{\tau(2+\sqrt2)/(m\ell)}$. At zero time these expressions give $(0,a,0)$ and all three velocities vanish.

The motion is a superposition of the two symmetric [normal modes](../../wave-equation.md#normal-mode), with opposite signed modal amplitudes. The outer beads always move together. Equivalently, $z_2=a\cos[(\omega_1+\omega_3)t/2]\cos[(\omega_3-\omega_1)t/2]$, displaying the modulation from the two frequencies. The result describes the linearized string while the initial amplitude and subsequent slopes remain small compared with the bead spacing.

## 8

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8/i">i</h3>

↑ **Parent:** [8](#8)

<h4 id="8/i/solution">Solution</h4>

↑ **Parent:** [I](#8/i)

The identity commutes with every group element, so it lies in the [center of a group](../../group-theory.md#center-of-a-group). If $z,w$ are central and $g\in G$, then $gw=wg$ implies $gw^{-1}=w^{-1}g$. Consequently

$$
g(zw^{-1})=zg w^{-1}=zw^{-1}g.
$$

Thus $zw^{-1}$ is central. The [subgroup test](../../group.md#subgroup-test) proves

$$
\boxed{Z(G)\leq G.}
$$

Equivalently, the centre is nonempty, closed under products, and closed under inverses. This proof does not require finiteness. In fact the centre is an [Abelian subgroup](../../group.md#abelian-subgroup), and it is normal because $gzg^{-1}=z$ for each central element.

<h3 id="8/ii">ii</h3>

↑ **Parent:** [8](#8)

<h4 id="8/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#8/ii)

Write the cyclic factors additively. The [order of a group element](../../group-theory.md#order-of-a-group-element) $(r,s)$ in a [direct product of groups](../../group-theory.md#direct-product-of-groups) is the least common multiple of its component orders, since a power is the identity exactly when it is the identity in both coordinates.

In $C_2\times C_3$, $(1,1)$ has order $\operatorname{lcm}(2,3)=6$, so it generates all six pairs. An explicit [group isomorphism](../../algebra.md#group-isomorphism) is

$$
\boxed{C_6\longrightarrow C_2\times C_3,\qquad[k]_6\longmapsto([k]_2,[k]_3).}
$$

It is well defined and multiplicative in additive notation; its kernel is zero because an integer divisible by both two and three is divisible by six. Equal finite orders then give bijectivity.

In $C_2\times C_4$, every element has order dividing four. A generator of $C_8$ has order eight, and isomorphisms preserve element orders, so

$$
\boxed{C_2\times C_4\not\cong C_8.}
$$

For positive integers $n,m$, the maximum element order in $C_n\times C_m$ is $\operatorname{lcm}(n,m)=nm/\gcd(n,m)$, attained by a pair of generators. The product is cyclic of order $nm$ exactly when that number is $nm$. Thus [cyclicity of a product of two finite cyclic groups](../../group-theory.md#cyclicity-of-a-product-of-two-finite-cyclic-groups) gives

$$
\boxed{C_n\times C_m\cong C_{nm}\quad\Longleftrightarrow\quad\gcd(n,m)=1.}
$$

For coprime factors the map $[k]_{nm}\mapsto([k]_n,[k]_m)$ gives the isomorphism, the group form of the [Chinese remainder theorem](../../mathematics.md#chinese-remainder-theorem).

## 9

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9/i">i</h3>

↑ **Parent:** [9](#9)

<h4 id="9/i/solution">Solution</h4>

↑ **Parent:** [I](#9/i)

For a [subgroup](../../group.md#subgroup) $H$ of a finite [group](../../group.md) $G$, [Lagrange's theorem](../../group-theory.md#lagrange-s-theorem) states

$$
\boxed{|G|=[G:H]|H|.}
$$

Here $[G:H]$ is the number of distinct left [cosets](../../group-theory.md#coset). Every coset has $|H|$ members, and the cosets partition $G$, proving the identity. In particular **the order of a subgroup divides the order of the group**. Divisibility is generally necessary, not sufficient, for a subgroup of a given order to exist.

<h3 id="9/ii">ii</h3>

↑ **Parent:** [9](#9)

<h4 id="9/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#9/ii)

The relation $Rm=mR^{-1}$ implies $mR^j=R^{-j}m$. Move each reflection generator to the right in any word, cancel pairs using $m^2=I$, and reduce exponents modulo $N$. Every element then has a normal form $R^j$ or $R^jm$, $0\leq j<N$.

For the actual [symmetry group](../../group-action.md#symmetry-group) of a regular polygon these are $N$ distinct rotations and $N$ distinct reflections. The determinant distinguishes rotations from reflections in the planar action. Hence the source's [dihedral group](../../finite-group-theory.md#dihedral-group) $D_N$ has order $2N$, with its subscript counting polygon vertices. The calculations below use that convention.

<h4 id="9/ii/a">a</h4>

↑ **Parent:** [Ii](#9/ii)

<h5 id="9/ii/a/solution">Solution</h5>

↑ **Parent:** [A](#9/ii/a)

For a regular [pentagon](../../euclidean-geometry.md#pentagon), take $R$ as rotation through $2\pi/5$ and $m$ as reflection in the horizontal axis through vertex zero. The distinct elements are

$$
\boxed{I,R,R^2,R^3,R^4,\qquad m,Rm,R^2m,R^3m,R^4m.}
$$

Every nonidentity rotation has order five. The reflections are the five order-two elements, since $(R^jm)^2=R^jR^{-j}=I$.

The reflection $R^jm$ has axis at angle $j\pi/5$ to the horizontal, understood modulo $\pi$. If vertices have angles $2k\pi/5$, it sends vertex $k$ to vertex $j-k\pmod5$. Each axis passes through one vertex and the midpoint of the opposite edge; that vertex stays fixed and the other four vertices exchange in two pairs.

<a id="9/ii/a/image-the-five-order-two-pentagon-symmetries-each-dashed-reflection-axis-fixes-one-vertex-and-exchanges-the-two-indicated-pairs"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2-2014-ib-pentagon-reflections.png)

**[Figure 2](#9/ii/a/image-the-five-order-two-pentagon-symmetries-each-dashed-reflection-axis-fixes-one-vertex-and-exchanges-the-two-indicated-pairs). The five order-two pentagon symmetries; each dashed reflection axis fixes one vertex and exchanges the two indicated pairs**.

<h4 id="9/ii/b">b</h4>

↑ **Parent:** [Ii](#9/ii)

<h5 id="9/ii/b/solution">Solution</h5>

↑ **Parent:** [B](#9/ii/b)

Since $|D_5|=10$, [Lagrange's theorem](../../group-theory.md#lagrange-s-theorem) permits proper subgroup orders only $1,2,5$. The complete list is

$$
\boxed{\{I\},\qquad\langle R\rangle=\{I,R,R^2,R^3,R^4\},\qquad\{I,R^jm\}\quad(j=0,1,2,3,4).}
$$

To show completeness, an order-two subgroup must be generated by its unique nonidentity element, necessarily one of the five reflections. An order-five subgroup is cyclic, since its order is prime; its generator cannot be a reflection, and every nonidentity rotation generates the same rotation subgroup. There is only one order-one subgroup.

Thus there are seven proper subgroups when the trivial subgroup is included, or six nontrivial proper subgroups. These are the prime-sided case of the [classification of subgroups of a dihedral group](../../finite-group-theory.md#classification-of-subgroups-of-a-dihedral-group).

<h4 id="9/ii/c">c</h4>

↑ **Parent:** [Ii](#9/ii)

<h5 id="9/ii/c/solution">Solution</h5>

↑ **Parent:** [C](#9/ii/c)

The [conjugacy class](../../group-action.md#conjugacy-class) of $g$ is $\{hgh^{-1}:h\in G\}$. Rotations commute with one another, while conjugation by a reflection changes $R^j$ to $R^{-j}$. Thus the rotation classes are $\{I\}$, $\{R,R^4\}$ and $\{R^2,R^3\}$.

For reflections,

$$
R^a(R^jm)R^{-a}=R^{j+2a}m.
$$

Because multiplication by two permutes the residues modulo five, these conjugates exhaust all five reflections. Consequently the complete class partition is

$$
\boxed{\{I\},\qquad\{R,R^4\},\qquad\{R^2,R^3\},\qquad\{m,Rm,R^2m,R^3m,R^4m\}.}
$$

Their sizes $1+2+2+5=10$ account for every element, as in the [conjugacy classes of a finite dihedral group](../../finite-group-theory.md#conjugacy-classes-of-a-finite-dihedral-group).

A [normal subgroup](../../group-theory.md#normal-subgroup) is a union of complete conjugacy classes. The trivial subgroup is normal, and the rotation subgroup is normal because conjugation preserves it; equivalently it has index two. None of the five order-two subgroups is normal, because it contains just one member of the five-element reflection class. Thus the proper normal subgroups are exactly

$$
\boxed{\{I\}\quad\text{and}\quad\langle R\rangle.}
$$

## 10

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10/i">i</h3>

↑ **Parent:** [10](#10)

<h4 id="10/i/solution">Solution</h4>

↑ **Parent:** [I](#10/i)

A [group representation](../../representation-theory.md#group-representation) assigns each $g\in G$ an invertible linear map $D(g)$ on a fixed vector space, preserving multiplication:

$$
D(gh)=D(g)D(h),\qquad D(e)=I.
$$

Choosing a basis turns those maps into matrices. A [faithful representation](../../representation-theory.md#faithful-representation) is injective, equivalently its kernel is $\{e\}$, so distinct elements have distinct matrices.

Two [group representations](../../representation-theory.md#group-representation) on spaces of the same dimension are called [equivalent representations](../../representation-theory.md#equivalence-of-group-representations) if one fixed invertible change of basis conjugates every representing matrix: $E(g)=S^{-1}D(g)S$ for all $g$. Choosing a different $S$ separately for each element does not establish equivalence.

The [character of a representation](../../representation-theory.md#character-of-a-representation) is

$$
\boxed{\chi_D(g)=\operatorname{tr}D(g).}
$$

The [cyclic property of the trace](../../linear-algebra.md#cyclic-property-of-the-trace) makes it invariant under a change of basis and constant on conjugacy classes. Thus different characters at even one group element prove inequivalence.

<h3 id="10/ii">ii</h3>

↑ **Parent:** [10](#10)

<h4 id="10/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#10/ii)

Since $a^4=I$, multiplication adds exponents modulo four: $a^ja^k=a^{j+k\bmod4}$. Hence the [Cayley table](../../algebraic-operation.md#cayley-table) of the [cyclic group of order four](../../group.md#cyclic-group-of-order-four), with the left factor indexing rows, is

$$
\boxed{\begin{array}{c|cccc}
\cdot&I&a&a^2&a^3\\\hline
I&I&a&a^2&a^3\\
a&a&a^2&a^3&I\\
a^2&a^2&a^3&I&a\\
a^3&a^3&I&a&a^2
\end{array}.}
$$

The table is symmetric because the group is Abelian. Its row for each element permutes all four members, as cancellation requires.

<h3 id="10/iii">iii</h3>

↑ **Parent:** [10](#10)

<h4 id="10/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#10/iii)

The matrices are listed in the order $I,a,a^2,a^3$. In the first representation, $D(a)$ is the clockwise quarter-turn matrix and $D(a)^2=-I_2$. In the second, $E(a)=iI_2$, whose successive powers give the listed scalar matrices. Both therefore obey the group table and distinguish all four elements.

Taking traces gives the [characters of a representation](../../representation-theory.md#character-of-a-representation):

$$
\boxed{\chi_D=(2,0,-2,0),\qquad\chi_E=(2,2i,-2,-2i).}
$$

In particular $\chi_D(a)=0$ but $\chi_E(a)=2i$. Since trace is invariant under similarity, **the representations are inequivalent**, even after allowing complex changes of basis for the real matrices of $D$.

One can also see the obstruction directly: conjugating the scalar matrix $iI_2$ leaves it unchanged, whereas $D(a)$ is not scalar. Over the complex numbers, $D(a)$ has eigenvalues $i,-i$, while $E(a)$ has $i,i$; those different multiplicities cannot be removed by changing basis.

<h3 id="10/iv">iv</h3>

↑ **Parent:** [10](#10)

<h4 id="10/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#10/iv)

Write the lower block of $T(a)$ as $B=\left(\begin{smallmatrix}0&b\\c&0\end{smallmatrix}\right)$. Then

$$
B^2=bcI_2,\qquad T(a)^2=\operatorname{diag}(1,bc,bc),\qquad T(a)^4=\operatorname{diag}(1,(bc)^2,(bc)^2).
$$

A representation of $C_4$ must satisfy its defining relation $T(a)^4=I_3$, so $(bc)^2=1$. For real $b,c$, this means $bc=1$ or $bc=-1$; it also ensures invertibility.

If $bc=-1$, then $T(a)^2\ne I_3$ while $T(a)^4=I_3$. The image of the generator has order four, so its four powers are distinct and the representation is faithful. If $bc=1$, then $T(a)^2=I_3$ but $T(a)\ne I_3$, since the lower block has zero diagonal. The image has order two and the kernel is $\{I,a^2\}$. Hence

$$
\boxed{\text{faithful exactly when }bc=-1;\qquad\text{unfaithful representation exactly when }bc=1.}
$$

For other values there is **no representation of $C_4$**, rather than an additional unfaithful case; in particular $bc=0$ would make the assigned matrix singular. These conclusions are the [faithfulness criterion for a block representation of the cyclic group of order four](../../group.md#faithfulness-criterion-for-a-block-representation-of-the-cyclic-group-of-order-four). There is no requirement that the proposed representation be orthogonal, so no separate conditions $|b|=|c|=1$ should be imposed.

## ↑ Ancestors (10)

1. [2014](../2014.md)
2. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
3. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
4. [Year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
