# Paper 2

↑ **Parent:** [2025](../2025.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2025/papernst_ib_2_2025.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2025/papernst_ib_2_2025.pdf)

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
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [i](#6/c/i)
      - [Solution](#6/c/i/solution)
    - [ii](#6/c/ii)
      - [Solution](#6/c/ii/solution)
    - [iii](#6/c/iii)
      - [Solution](#6/c/iii/solution)
  - [d](#6/d)
    - [Solution](#6/d/solution)
- [7](#7)
  - [a](#7/a)
    - [Solution](#7/a/solution)
  - [b](#7/b)
    - [Solution](#7/b/solution)
  - [c](#7/c)
    - [Solution](#7/c/solution)
- [8](#8)
  - [a](#8/a)
    - [Solution](#8/a/solution)
  - [b](#8/b)
    - [Solution](#8/b/solution)
  - [c](#8/c)
    - [Solution](#8/c/solution)
- [9](#9)
  - [a](#9/a)
    - [Solution](#9/a/solution)
  - [b](#9/b)
    - [Solution](#9/b/solution)
  - [c](#9/c)
    - [Solution](#9/c/solution)
  - [d](#9/d)
    - [Solution](#9/d/solution)
- [10](#10)
  - [a](#10/a)
    - [Solution](#10/a/solution)
  - [b](#10/b)
    - [Solution](#10/b/solution)
  - [c](#10/c)
    - [Solution](#10/c/solution)

## 1

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Multiplication by $x^2$ gives the [Sturm-Liouville form](../../sturm-liouville-theory.md#sturm-liouville-form)

$$
-(x^2u')'=\lambda x^2u,
$$

so the weight is $w(x)=x^2$. Use the weighted [inner product](../../inner-product.md) $\langle f,g\rangle_w=\int_0^{\pi/2}x^2\overline f g\,dx$ and the [Sturm-Liouville operator](../../sturm-liouville-theory.md#sturm-liouville-operator) $L=-x^{-2}(x^2d/dx)'$. [Integration by parts](../../calculus.md#integration-by-parts) gives its boundary form:

$$
\langle f,Lg\rangle_w-\langle Lf,g\rangle_w
=\left[x^2(\overline {f'}g-\overline f g')\right]_0^{\pi/2}=0.
$$

The upper endpoint term vanishes by the [Dirichlet boundary conditions](../../differential-equation.md#dirichlet-boundary-condition), and the lower one vanishes for the regular solutions. More precisely, the [radial Dirichlet spectrum in three dimensions](../../sturm-liouville-theory.md#radial-dirichlet-spectrum-in-three-dimensions) identifies $L$ under the [unitary transformation](../../vector-space.md#unitary-operator) $v=xu$ with $-v''$ on $(0,\pi/2)$ with zero endpoint values; this specifies the [self-adjoint](../../linear-operator-theory.md#self-adjoint-operator) realization at the singular endpoint as well as proving the formal identity.

For [eigenfunctions](../../linear-operator-theory.md#eigenfunction) $u_a,u_b$ with different [eigenvalues](../../linear-operator-theory.md#eigenvalue), the same identity gives $(\lambda_b-\lambda_a)\langle u_a,u_b\rangle_w=0$. Taking real [eigenfunctions](../../linear-operator-theory.md#eigenfunction) proves the required [orthogonality of Sturm-Liouville eigenfunctions](../../sturm-liouville-theory.md#orthogonality-of-sturm-liouville-eigenfunctions).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Set $v=xu$. Direct [differentiation](../../calculus.md#differentiation) gives $u''+2u'/x=v''/x$, so $-v''=\lambda v$. Finiteness of $u$ at zero requires $v(0)=0$, and the other endpoint gives $v(\pi/2)=0$. The [Dirichlet eigenvalues](../../sturm-liouville-theory.md#dirichlet-eigenvalue) are positive: [integration by parts](../../calculus.md#integration-by-parts) gives $\lambda\int|v|^2=\int|v'|^2$, and a nonzero $v$ cannot have zero right-hand side. Thus $v=C\sin(\sqrt\lambda x)$, and the second endpoint gives

$$
\boxed{\lambda_n=4n^2,\qquad u_n(x)=\frac{\sin(2nx)}x,\qquad n=1,2,\ldots.}
$$

Define $u_n(0)=2n$ by its [limit](../../calculus.md#limit-of-a-function). This is the [radial Dirichlet spectrum in three dimensions](../../sturm-liouville-theory.md#radial-dirichlet-spectrum-in-three-dimensions) with radius $\pi/2$. Its weighted squared [norm](../../normed-vector-space.md#norm) is $\int_0^{\pi/2}x^2u_n^2dx=\pi/4$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Write the equation as $(L+\beta)y=-\cos x/x$ with the positive [Sturm-Liouville operator](../../sturm-liouville-theory.md#sturm-liouville-operator) from part (a). A [Sturm-Liouville eigenfunction expansion](../../sturm-liouville-theory.md#sturm-liouville-eigenfunction-expansion) therefore gives $a_n=-f_n/(4n^2+\beta)$, where weighted [orthogonal projection](../../hilbert-space.md#orthogonal-projection) gives

$$
f_n=\frac4\pi\int_0^{\pi/2}\sin(2nx)\cos x\,dx
=\frac{8n}{\pi(4n^2-1)}.
$$

Here the [product-to-sum formulas](../../geometry-and-topology.md#product-to-sum-formula) reduce the [integral](../../integral.md) to half the sum of the integrals of $\sin((2n+1)x)$ and $\sin((2n-1)x)$. Consequently

$$
\boxed{y(x)=-\sum_{n=1}^\infty\frac{8n}{\pi(4n^2-1)(4n^2+\beta)}\frac{\sin(2nx)}x.}
$$

At $x=0$, use the continuous limits of the terms. The coefficients are $O(n^{-3})$, so the resulting endpoint series converges. Completeness is the ordinary [Fourier sine series](../../fourier-series.md#fourier-sine-series) completeness after $v=xy$. For an independent check, solving $v''-\beta v=\cos x$ with zero endpoint values gives

$$
y(x)=\frac{\sinh(\sqrt\beta(\pi/2-x))/\sinh(\sqrt\beta\pi/2)-\cos x}{(1+\beta)x}.
$$

Its numerator vanishes at zero, and it has the same [orthogonal projection](../../hilbert-space.md#orthogonal-projection) coefficients. Positivity of $L+\beta$ proves [uniqueness](../../mathematical-logic.md#uniqueness).

## 2

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For an [axisymmetric harmonic function](../../partial-differential-equation.md#axisymmetric-harmonic-function), put $\Psi=R(r)\Theta(\theta)$ in the [Laplacian in spherical coordinates](../../partial-differential-equation.md#laplacian-in-spherical-coordinates) and multiply by $r^2/(R\Theta)$. [Separation of variables](../../partial-differential-equation.md#separation-of-variables) gives

$$
\frac{(r^2R')'}R=-\frac{(\sin\theta\,\Theta')'}{\sin\theta\,\Theta}=\ell(\ell+1).
$$

With $u=\cos\theta$, the angular equation becomes the [Legendre differential equation](../../linear-ordinary-differential-equation.md#legendre-differential-equation). Regularity at both poles selects the [Legendre polynomials](../../linear-ordinary-differential-equation.md#legendre-polynomial) $P_\ell(u)$ with integer $\ell\ge0$; the singular second solutions are excluded. The radial [Euler-Cauchy equation](../../linear-ordinary-differential-equation.md#euler-cauchy-equation) has solutions $r^\ell$ and $r^{-\ell-1}$. [Superposition](../../vector-space.md#superposition-principle) therefore gives

$$
\Psi=\sum_{\ell=0}^\infty(A_\ell r^\ell+B_\ell r^{-\ell-1})P_\ell(\cos\theta),
$$

with coefficients chosen to ensure convergence and the required boundary regularity. The [axisymmetric harmonic extension from a sphere](../../partial-differential-equation.md#axisymmetric-harmonic-extension-from-a-sphere) gives these coefficients directly from boundary data.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Set $u=\cos\theta$. The boundary data simplify to $u+2u^2=\frac23P_0(u)+P_1(u)+\frac43P_2(u)$. The [axisymmetric harmonic extension from a sphere](../../partial-differential-equation.md#axisymmetric-harmonic-extension-from-a-sphere) keeps only decaying radial powers outside and regular powers inside. Hence

$$
\boxed{\Psi_{\rm out}=\frac{2a}{3r}+\frac{a^2}{r^2}\cos\theta+\frac{4a^3}{3r^3}P_2(\cos\theta),\quad r\ge a,}
$$

and

$$
\boxed{\Psi_{\rm in}=\frac23+\frac ra\cos\theta+\frac{4r^2}{3a^2}P_2(\cos\theta),\quad r\le a.}
$$

Each [Legendre polynomial](../../linear-ordinary-differential-equation.md#legendre-polynomial) coefficient agrees at $r=a$. The exterior solution tends to zero, and the interior solution is finite at $r=0$. The [maximum principle for harmonic functions](../../partial-differential-equation.md#maximum-principle-for-harmonic-functions) proves [uniqueness](../../mathematical-logic.md#uniqueness) in these respective classes.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The plane separates the exterior into two half-domains. Use an [odd Legendre extension for an equatorial Dirichlet plane](../../partial-differential-equation.md#odd-legendre-extension-for-an-equatorial-dirichlet-plane) in each. On the upper hemisphere, extend $u+2u^2$ to the odd function $u+2u|u|$ on the whole sphere. On the lower hemisphere, the appropriate odd extension is $u-2u|u|$. Define, for odd $\ell$,

$$
b_\ell=2(2\ell+1)\int_0^1t^2P_\ell(t)\,dt.
$$

The [orthogonality](../../inner-product.md#orthogonal-vectors) and parity of the [Legendre polynomials](../../linear-ordinary-differential-equation.md#legendre-polynomial) give the solution in both half-domains as

$$
\boxed{\Psi(r,\theta)=\frac{a^2}{r^2}u+\operatorname{sgn}(u)\sum_{\ell=1,3,5,\ldots}b_\ell\left(\frac ar\right)^{\ell+1}P_\ell(u),\quad u=\cos\theta.}
$$

Set its value on $u=0$ to zero. The first coefficients are $b_1=3/2$ and $b_3=7/12$. All odd [Legendre polynomials](../../linear-ordinary-differential-equation.md#legendre-polynomial) vanish at zero, so the plane condition holds. On the sphere the sum is $2u|u|$, and multiplication by $\operatorname{sgn}(u)$ recovers $2u^2$ on either side. Thus the original sphere data and decay at infinity both hold. A jump of the normal [derivative](../../calculus.md#derivative) at the sheet is permitted; the sheet can support induced [surface charge density](../../electrostatics.md#surface-charge-density).

## 3

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Since the [electric field](../../electric-field.md) is [irrotational](../../multivariable-calculus.md#irrotational-vector-field), introduce an [electrostatic potential](../../electric-field.md#electric-potential) with $\mathbf E=-\nabla\varphi$. [Gauss's law](../../maxwell-equations.md#gauss-s-law) becomes the [Poisson equation](../../partial-differential-equation.md#poisson-s-equation)

$$
\boxed{(\partial_x^2+\partial_y^2)\varphi=-\rho/\epsilon_0,\qquad\mathbf E=-\nabla\varphi.}
$$

The curl equation is automatic because the [curl of a gradient](../../multivariable-calculus.md#curl-of-a-gradient) vanishes. Independence of $z$ makes $E_z$ constant, and its required decay forces it to be zero, so a $z$-independent potential suffices.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For the rotationally invariant free-space [fundamental solution of the Laplace equation](../../partial-differential-equation.md#fundamental-solution-of-the-laplace-equation), put $s=\sqrt{(x-x')^2+(y-y')^2}$. Away from the source, the [radial Laplacian](../../partial-differential-equation.md#radial-laplacian) gives $(sG')'=0$, hence $G=A\log s^2+C$. Integrate its [Poisson equation](../../partial-differential-equation.md#poisson-s-equation) over a disk of radius $r$ about the source. The [divergence theorem](../../multivariable-calculus.md#divergence-theorem) gives $2\pi r(2A/r)=-1/\epsilon_0$, so

$$
\boxed{G=-\frac{1}{4\pi\epsilon_0}\log\big((x-x')^2+(y-y')^2\big)+C.}
$$

A fixed reference length can be inserted inside the [logarithm](../../calculus.md#logarithm) and absorbed into $C$. The resulting [electric field](../../electric-field.md) decays like $1/s$.

Strictly, the stated pointwise decay as $y\to\pm\infty$ alone does not justify “most general”: one can also add the [harmonic function](../../partial-differential-equation.md#harmonic-function) $\operatorname{Re}e^{(x+iy)^2}$, whose [gradient](../../multivariable-calculus.md#gradient) has that decay for every fixed $x$. This is the same growth issue as a [zero-boundary harmonic function with pointwise vertical decay](../../partial-differential-equation.md#zero-boundary-harmonic-function-with-pointwise-vertical-decay). The displayed answer is the usual isotropic free-space choice; requiring the field to vanish uniformly in every direction at spatial infinity removes these extra harmonic additions. An additive constant remains undetermined.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Use the [Green-function representation](../../green-s-function.md#green-function-representation) to integrate over the charged segment:

$$
\varphi(x,y)=-\frac1{4\pi\epsilon_0}\int_0^L\log((x-s)^2+y^2)\,ds+C_0.
$$

For $y\ne0$, a primitive with respect to $u$ is

$$
F(u,y)=u\log(u^2+y^2)-2u+2y\arctan(u/y),
$$

as direct [differentiation](../../calculus.md#differentiation) verifies using the [derivative](../../calculus.md#derivative) of [inverse tangent](../../geometry-and-topology.md#inverse-tangent). Therefore

$$
\boxed{\varphi(x,y)=-\frac{F(x,y)-F(x-L,y)}{4\pi\epsilon_0}+C_0.}
$$

This expression is even in $y$, since $y\arctan(u/y)$ is even. On $y=0$, take the continuous limit $F(u,0)=u\log u^2-2u$, with $u\log u^2=0$ at $u=0$. The finite segment has a logarithmically growing potential at large distance, but its [electric field](../../electric-field.md) decays; the boundary condition constrains the field rather than the potential.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Differentiate the [Green-function representation](../../green-s-function.md#green-function-representation), valid away from the charged sheet:

$$
E_y=\frac1{2\pi\epsilon_0}\int_0^L\frac{y\,ds}{(x-s)^2+y^2}
=\frac{\arctan(x/y)-\arctan((x-L)/y)}{2\pi\epsilon_0}.
$$

For $0<x<L$, the two [inverse tangent](../../geometry-and-topology.md#inverse-tangent) limits at $y\downarrow0$ are $\pi/2$ and $-\pi/2$; approaching from below reverses both signs. Thus

$$
\boxed{E_y(x,0^+)=\frac1{2\epsilon_0},\quad E_y(x,0^-)=-\frac1{2\epsilon_0},\quad |\Delta E_y|=\frac1{\epsilon_0}.}
$$

This agrees with the normal [electric field](../../electric-field.md) jump obtained by applying [Gauss's law](../../maxwell-equations.md#gauss-s-law) to a thin pillbox enclosing unit [surface charge density](../../electrostatics.md#surface-charge-density).

## 4

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The function $e^{-z^2}$ is [entire](../../holomorphic-function.md#entire-function), so [Cauchy's integral theorem](../../complex-analysis.md#cauchy-s-integral-theorem) makes its [contour integral](../../complex-analysis.md#contour-integral) around the rectangle vanish. The lower horizontal integral tends to $\sqrt\pi$ by the [Gaussian integral](../../integral.md#gaussian-integral). On a vertical side $z=\pm R+it$, with $t$ between $0$ and $b$, its modulus is $e^{-R^2+t^2}\le e^{-R^2+b^2}$; hence both vertical integrals tend to zero. The upper side has the opposite orientation and contributes

$$
-e^{b^2}\int_{-\infty}^{\infty}e^{-x^2}e^{-2ibx}\,dx.
$$

Consequently the integral in this expression is $\sqrt\pi e^{-b^2}$. Its imaginary part vanishes because $e^{-x^2}\sin(2bx)$ is [odd](../../calculus.md#odd-function), and its real part is twice the positive-half-line integral because the integrand there is [even](../../calculus.md#even-function). Therefore

$$
\boxed{\int_0^\infty e^{-x^2}\cos(2bx)\,dx=\frac{\sqrt\pi}{2}e^{-b^2}.}
$$

For negative $b$ the rectangle lies below the real axis and the same cancellation holds; alternatively use the even dependence on $b$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let $B=|b|>0$. For $a>0$, integrate $e^{iaz}/(z^2+B^2)$ over the upper semicircle. [Jordan's lemma](../../complex-analysis.md#jordan-s-lemma) removes the arc, and the [residue theorem](../../analysis.md#residue-theorem) at $z=iB$ gives

$$
\int_{-\infty}^{\infty}\frac{e^{iax}}{x^2+B^2}\,dx
=2\pi i\frac{e^{-aB}}{2iB}=\frac\pi B e^{-aB}.
$$

Taking the real part and using [evenness](../../calculus.md#even-function) in both $x$ and $a$ yields

$$
\boxed{I_1(a)=\frac{\pi}{2B}e^{-B|a|}.}
$$

The case $a=0$ follows directly from an [inverse tangent](../../geometry-and-topology.md#inverse-tangent) primitive. The complex exponential is essential on the contour: the cosine alone has a growing exponential component.

For $a>0$, [differentiation under the integral sign](../../analysis.md#differentiation-under-the-integral-sign) gives $-I_1'(a)=\int_0^\infty x\sin(ax)/(x^2+B^2)\,dx$. This derivative is a conditionally convergent [improper integral](../../real-analysis.md#improper-integral); the [Dirichlet test](../../sequence-and-series.md#dirichlet-test) makes its tails uniform on compact subintervals of $a>0$, justifying the differentiation. Setting $a=1$ gives

$$
\boxed{I_2=\frac\pi2e^{-B}.}
$$

Finally let $J(a)=\int_0^\infty\sin(ax)/[x(x^2+B^2)]\,dx$. Its differentiated integrand is absolutely integrable, so $J'(a)=I_1(a)$ and $J(0)=0$. Hence

$$
\boxed{I_3=J(1)=\frac{\pi}{2B^2}(1-e^{-B}).}
$$

If $b=0$, $I_1$ and $I_3$ diverge at the origin, whereas $I_2=\int_0^\infty\sin x/x\,dx=\pi/2$ is the corresponding [Dirichlet integral](../../fourier-analysis.md#dirichlet-integral).

## 5

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The [Fourier transform of a derivative](../../fourier-analysis.md#fourier-transform-of-a-derivative) is $i\omega$ times the transform under the stated convention. Transforming the [linear ordinary differential equation](../../linear-ordinary-differential-equation.md) gives

$$
(-\omega^2+5i\omega+6)\widetilde x=\widetilde F,
\qquad\boxed{R(\omega)=\frac1{(i\omega+2)(i\omega+3)}.}
$$

The applied [force](../../force.md) is $F(t)=H(t)e^{-t}$, with $H$ the [Heaviside step function](../../integral-transform.md#heaviside-step-function), so $\widetilde F=(1+i\omega)^{-1}$. Partial fractions give

$$
\widetilde x=\frac{1/2}{1+i\omega}-\frac1{2+i\omega}+\frac{1/2}{3+i\omega}.
$$

Using the transform pair $H(t)e^{-ct}\leftrightarrow(c+i\omega)^{-1}$ yields

$$
\boxed{x(t)=H(t)\left(\tfrac12e^{-t}-e^{-2t}+\tfrac12e^{-3t}\right).}
$$

Its value and first [derivative](../../calculus.md#derivative) both vanish at $t=0^+$, so the joining introduces no spurious [Dirac delta](../../distribution-theory.md#dirac-delta-function) terms. Equivalently, this is the [convolution](../../fourier-analysis.md#convolution) of the [force](../../force.md) with the causal [impulse response](../../green-s-function.md#impulse-response) $H(t)(e^{-2t}-e^{-3t})$.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Write $q=i\omega$. A constant-coefficient [linear ordinary differential equation](../../linear-ordinary-differential-equation.md) has [transfer function](../../control-theory.md#transfer-function) $1/P(q)$, where $P(q)=\sum_{n=1}^c a_nq^n$. The specified simple [poles](../../isolated-singularity.md#pole) correspond to $q=0,-2,1$. A minimal-order choice is therefore

$$
P(q)=q(q+2)(q-1)=q^3+q^2-2q.
$$

Thus one possible system is

$$
\boxed{x'''+x''-2x'=F,\qquad c=3,\quad(a_1,a_2,a_3)=(-2,1,1),}
$$

up to a common nonzero multiplicative constant. The root $q=1$ permits an exponentially growing homogeneous solution; the pole data therefore describe an unstable system. This does not prevent the requested algebraic reconstruction of its [transfer function](../../control-theory.md#transfer-function).

## 6

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

For a [rotation matrix](../../linear-algebra.md#rotation-matrix) $R\in SO(3)$, the Cartesian [tensor component transformation law](../../general-relativity.md#tensor-component-transformation-law) is

$$
\boxed{T'_{ijkl}=R_{ia}R_{jb}R_{kc}R_{ld}T_{abcd}.}
$$

An [isotropic tensor](../../multilinear-algebra.md#isotropic-tensor) is unchanged under every such rotation, so its components satisfy $T_{ijkl}=R_{ia}R_{jb}R_{kc}R_{ld}T_{abcd}$ for every $R\in SO(3)$. The repeated indices are summed by the [Einstein summation convention](../../multilinear-algebra.md#einstein-notation).

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Take the [trace](../../linear-algebra.md#matrix-trace) first: the [antisymmetric tensor](../../multilinear-algebra.md#antisymmetric-tensor) has zero diagonal and $X$ is traceless, so $T_{ii}=3t$. Taking symmetric and antisymmetric parts then gives the [scalar, symmetric-traceless and axial tensor decomposition](../../multilinear-algebra.md#scalar-symmetric-traceless-and-axial-tensor-decomposition):

$$
\boxed{t=\frac13T_{kk},\quad A_{ij}=\frac12(T_{ij}-T_{ji}),\quad X_{ij}=\frac12(T_{ij}+T_{ji})-\frac13T_{kk}\delta_{ij}.}
$$

The [Kronecker delta](../../multilinear-algebra.md#kronecker-delta) satisfies $\delta_{ii}=3$, which verifies $X_{ii}=0$. Substitution verifies the original decomposition and also proves its [uniqueness](../../mathematical-logic.md#uniqueness).

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/i">i</h4>

↑ **Parent:** [C](#6/c)

<h5 id="6/c/i/solution">Solution</h5>

↑ **Parent:** [I](#6/c/i)

Relabel the two [dummy indices](../../multilinear-algebra.md#dummy-index) and use the respective symmetries:

$$
X_{ij}A_{ij}=X_{ji}A_{ji}=-X_{ij}A_{ij}=0.
$$

Thus the [symmetric tensor](../../multilinear-algebra.md#symmetric-tensor) and [antisymmetric tensor](../../multilinear-algebra.md#antisymmetric-tensor) subspaces are [orthogonal](../../inner-product.md#orthogonal-vectors) in the [Frobenius inner product](../../inner-product.md#frobenius-inner-product).

<h4 id="6/c/ii">ii</h4>

↑ **Parent:** [C](#6/c)

<h5 id="6/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/c/ii)

The contraction is $\operatorname{tr}(A^3)$. Since $A^T=-A$, [transpose](../../vector-space.md#transpose) and invariance of the [trace](../../linear-algebra.md#matrix-trace) give

$$
\operatorname{tr}(A^3)=\operatorname{tr}((A^3)^T)=\operatorname{tr}((-A)^3)=-\operatorname{tr}(A^3)=0.
$$

This is the odd-power case of [vanishing odd complete contractions of an antisymmetric matrix](../../multilinear-algebra.md#vanishing-odd-complete-contractions-of-an-antisymmetric-matrix).

<h4 id="6/c/iii">iii</h4>

↑ **Parent:** [C](#6/c)

<h5 id="6/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#6/c/iii)

A complete pairwise [tensor contraction](../../multilinear-algebra.md#tensor-contraction) of copies of $A$ is represented by closed index cycles. Each cycle is a [trace](../../linear-algebra.md#matrix-trace) $\operatorname{tr}(A^r)$, possibly with a sign from reversing an index pair. If a contraction is internal to one copy, it contains the already vanishing $\operatorname{tr}A$. Otherwise an odd total number of copies forces at least one cycle of odd length, since a sum of even lengths is even. That trace vanishes by the transposition argument in part (ii). Therefore **every such complete contraction is zero**. This proves [vanishing odd complete contractions of an antisymmetric matrix](../../multilinear-algebra.md#vanishing-odd-complete-contractions-of-an-antisymmetric-matrix) without assuming that all contractions form a single trace.

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

Let $J_{ij}=\int_B x_ix_j\,d^3x$. Rotational symmetry makes $J$ an [isotropic second-rank tensor](../../multilinear-algebra.md#isotropic-second-rank-tensor), so $J_{ij}=C\delta_{ij}$. Contracting the indices and integrating in [spherical coordinates](../../multivariable-calculus.md#spherical-coordinate-system) gives

$$
3C=\int_Br^2\,d^3x=4\pi\int_0^1r^4dr=\frac{4\pi}5.
$$

The [isotropic second moment of a ball](../../multilinear-algebra.md#isotropic-second-moment-of-a-ball) therefore gives

$$
\boxed{I=M_{ij}J_{ij}=\frac{4\pi}{15}\operatorname{tr}M.}
$$

Only the scalar part of $M$ contributes; its [antisymmetric tensor](../../multilinear-algebra.md#antisymmetric-tensor) and symmetric-traceless parts give zero.

## 7

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

Let $\mathbf q=(x,y)$ be the centre displacement and $\theta$ the small disk rotation. Put $d=l-l_0>0$. The [moment of inertia of a uniform disc](../../rigid-body-dynamics.md#moment-of-inertia-of-a-uniform-disc) is $I=ma^2/2$, obtained from $I=\int_0^a\rho r^2(2\pi r\,dr)$ and $m=\rho\pi a^2$. Thus the [kinetic energy](../../energy.md#kinetic-energy) is $T=m|\dot{\mathbf q}|^2/2+ma^2\dot\theta^2/4$.

For one spring, let $\mathbf n_j$ point radially towards its fixed anchor and let $\mathbf t_j$ be the perpendicular unit [vector](../../vector-space.md#vector). The moving attachment is $\mathbf q+aR(\theta)\mathbf n_j$, while the anchor is $(a+l)\mathbf n_j$. Expanding their separation to second order gives the spring extension beyond natural length:

$$
s_j-l_0=d-\mathbf n_j\cdot\mathbf q+\frac a2\theta^2+
\frac{(\mathbf t_j\cdot\mathbf q+a\theta)^2}{2l}+O((|\mathbf q|+|\theta|)^3).
$$

Insert this in the [elastic potential energy](../../elasticity-physics.md#elastic-energy) $V=(k/2)\sum_j(s_j-l_0)^2$. For the three symmetric directions, $\sum_j\mathbf n_j=\sum_j\mathbf t_j=0$ and $\sum_j(\mathbf n_j\cdot\mathbf q)^2=\sum_j(\mathbf t_j\cdot\mathbf q)^2=3|\mathbf q|^2/2$. Dropping the constant equilibrium energy gives

$$
V_2=\frac{3k}{4}\left(1+\frac dl\right)(x^2+y^2)+\frac{3kda(a+l)}{2l}\theta^2.
$$

Therefore the quadratic [Lagrangian](../../calculus-of-variations.md#lagrangian) is

$$
\boxed{\mathcal L_2=\frac m2(\dot x^2+\dot y^2)+\frac{ma^2}4\dot\theta^2-\frac{3k}{4}\left(1+\frac dl\right)(x^2+y^2)-\frac{3kda(a+l)}{2l}\theta^2.}
$$

The prestretch terms cannot be omitted: they supply transverse spring stiffness and the entire rotational restoring torque, as derived generally in [small oscillations of a disk attached to prestretched radial springs](../../lagrangian-mechanics.md#small-oscillations-of-a-disk-attached-to-prestretched-radial-springs).

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/solution">Solution</h4>

↑ **Parent:** [B](#7/b)

The quadratic [Lagrangian](../../calculus-of-variations.md#lagrangian) is diagonal in $x,y,\theta$, so the [Euler-Lagrange equations](../../analysis.md#euler-lagrange-equation) give two pure translations and one pure rotation. Their [angular frequencies](../../lagrangian-mechanics.md#angular-frequency) are

$$
\boxed{\omega_x^2=\omega_y^2=\frac{3k}{2m}\left(1+\frac{l-l_0}{l}\right),\qquad
\omega_\theta^2=\frac{6k(l-l_0)(a+l)}{mal}.}
$$

A horizontal translation has $(x,y,\theta)=(A\cos\omega_xt,0,0)$; a vertical translation has $(0,A\cos\omega_yt,0)$; and the rotational mode has $(0,0,A\cos\omega_\theta t)$. Any fixed-direction translation is another choice in the same two-dimensional degenerate [normal mode](../../wave-equation.md#normal-mode) space. The rotation keeps the centre fixed.

<a id="7/b/image-two-degenerate-translations-and-a-separate-rotation-of-a-disk-on-symmetric-radial-springs"></a>
![](../../radially-sprung-disk-normal-modes.png)

**[Figure 1](#7/b/image-two-degenerate-translations-and-a-separate-rotation-of-a-disk-on-symmetric-radial-springs). Two degenerate translations and a separate rotation of a disk on symmetric radial springs**. Original schematic of the three [normal modes](../../wave-equation.md#normal-mode); arrows indicate the independent motions, and the dashed disk marks the equilibrium position.

<h3 id="7/c">c</h3>

↑ **Parent:** [7](#7)

<h4 id="7/c/solution">Solution</h4>

↑ **Parent:** [C](#7/c)

The disk still has only **three degrees of freedom and hence three normal modes**: two centre coordinates and one in-plane rotation. Five springs alter the restoring [quadratic form](../../quadratic-form.md) but add no disk coordinates. The fivefold [rotational symmetry](../../linear-algebra.md#rotational-symmetry) makes the translational stiffness proportional to the two-dimensional [identity matrix](../../vector-space.md#identity-matrix), and makes translation-rotation coupling vanish. Therefore **the two translation modes are always degenerate**; the rotational mode is separate, with possible accidental equality of its frequency for particular parameters. The general formulas in [small oscillations of a disk attached to prestretched radial springs](../../lagrangian-mechanics.md#small-oscillations-of-a-disk-attached-to-prestretched-radial-springs) apply with $N=5$.

## 8

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8/a">a</h3>

↑ **Parent:** [8](#8)

<h4 id="8/a/solution">Solution</h4>

↑ **Parent:** [A](#8/a)

For the first [Cayley table](../../algebraic-operation.md#cayley-table), [associativity](../../algebraic-operation.md#associative-property) fails: $(a\ast a)\ast b=1\ast b=b$, whereas $a\ast(a\ast b)=a\ast c=d$. It therefore **does not define a group**.

For the second table, assign the residues $0,1,2,3,4$ to $1,a,c,b,d$, respectively. Every table entry agrees with [addition modulo an integer](../../modular-arithmetic.md#addition-modulo-an-integer) modulo five. Thus this table **defines the cyclic group of order five**, with identity $1$ and inverses $a^{-1}=d$, $c^{-1}=b$. The identification with a known [group](../../group.md) verifies [associativity](../../algebraic-operation.md#associative-property) as well as closure and the inverse axioms; inspecting only the identity row and inverses would not suffice.

<h3 id="8/b">b</h3>

↑ **Parent:** [8](#8)

<h4 id="8/b/solution">Solution</h4>

↑ **Parent:** [B](#8/b)

Use [group axioms from two-sided local inverse identities](../../group.md#group-axioms-from-two-sided-local-inverse-identities). Choose any $a$ in the nonempty [semigroup](../../algebraic-operation.md#semigroup) and put $e_R=a_L^{-1}a$, $e_L=aa_R^{-1}$. The given identities say $be_R=b$ and $e_Lb=b$ for every $b$. Therefore $e_Le_R=e_L$ by the right-identity property, and $e_Le_R=e_R$ by the left-identity property. Thus $e_L=e_R=e$ is a two-sided [identity element](../../algebraic-operation.md#identity-element).

For an arbitrary $a$, set $b=a_L^{-1}$ and $c=a_R^{-1}$. Inserting $e$ into the original identities gives $ba=e$ and $ac=e$. By [associativity](../../algebraic-operation.md#associative-property),

$$
b=be=b(ac)=(ba)c=ec=c.
$$

Thus every element has a two-sided [inverse element](../../algebraic-operation.md#inverse-element). Closure and [associativity](../../algebraic-operation.md#associative-property) were assumed, so **all the group axioms hold**. No cancellation or identity was used before it had been established.

<h3 id="8/c">c</h3>

↑ **Parent:** [8](#8)

<h4 id="8/c/solution">Solution</h4>

↑ **Parent:** [C](#8/c)

Write the [dihedral group](../../finite-group-theory.md#dihedral-group) as $D_6=\langle r,s\mid r^6=s^2=1,\ srs=r^{-1}\rangle$, where $r$ rotates through $\pi/3$. There are six rotations and six reflections, so **the order is 12**. Conjugation by $s$ reverses a rotation, and conjugation by $r$ sends $r^js$ to $r^{j+2}s$. Consequently the [conjugacy classes](../../group-action.md#conjugacy-class) and their sizes are

$$
\boxed{\{1\}\ (1),\quad\{r^3\}\ (1),\quad\{r,r^5\}\ (2),\quad\{r^2,r^4\}\ (2),\quad\{s,r^2s,r^4s\}\ (3),\quad\{rs,r^3s,r^5s\}\ (3).}
$$

The last two classes distinguish the reflection axes through opposite vertices and through opposite edge midpoints. Their sizes sum to 12.

## 9

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9/a">a</h3>

↑ **Parent:** [9](#9)

<h4 id="9/a/solution">Solution</h4>

↑ **Parent:** [A](#9/a)

A [group homomorphism](../../group-theory.md#group-homomorphism) $f:G\to H$ preserves the operation: $f(ab)=f(a)f(b)$ for all $a,b\in G$. A [group isomorphism](../../algebra.md#group-isomorphism) is a bijective [group homomorphism](../../group-theory.md#group-homomorphism); its inverse also preserves the operation. The [kernel of a group homomorphism](../../group-theory.md#kernel-of-a-group-homomorphism) is $\ker f=\{g\in G:f(g)=e_H\}$, a [normal subgroup](../../group-theory.md#normal-subgroup) of $G$.

<h3 id="9/b">b</h3>

↑ **Parent:** [9](#9)

<h4 id="9/b/solution">Solution</h4>

↑ **Parent:** [B](#9/b)

Choose $g\ne e$. By [Lagrange's theorem](../../group-theory.md#lagrange-s-theorem), its cyclic [subgroup](../../group.md#subgroup) has order dividing the prime 101. It is not of order one, so $\langle g\rangle=G$. Thus **the group is cyclic, and hence abelian**. In particular, every pair of elements is $g^i,g^j$, and $g^ig^j=g^{i+j}=g^{j+i}=g^jg^i$.

<h3 id="9/c">c</h3>

↑ **Parent:** [9](#9)

<h4 id="9/c/solution">Solution</h4>

↑ **Parent:** [C](#9/c)

A [group homomorphism](../../group-theory.md#group-homomorphism) from the additive [cyclic group](../../group.md#cyclic-group) $\mathbb Z_6$ is determined by the image $t$ of its generator $1$, with the consistency condition $6t=0$ in the target. Every element of either target satisfies this condition. Therefore

$$
\boxed{\mathbb Z_6\to\mathbb Z_2:\quad f_t([n]_6)=[tn]_2,\quad t=0,1,}
$$

and

$$
\boxed{\mathbb Z_6\to\mathbb Z_3:\quad f_t([n]_6)=[tn]_3,\quad t=0,1,2.}
$$

These formulas are well-defined because changing $n$ by six changes $tn$ by a target multiple of its modulus. They list respectively two and three maps.

<h3 id="9/d">d</h3>

↑ **Parent:** [9](#9)

<h4 id="9/d/solution">Solution</h4>

↑ **Parent:** [D](#9/d)

The [symmetric group](../../finite-group-theory.md#symmetric-group) $S_3$ is generated by transpositions, each of order two. A [group homomorphism](../../group-theory.md#group-homomorphism) to $\mathbb Z_3$ must map every transposition to zero, because the only target element annihilated by two is zero. Hence **the map to $\mathbb Z_3$ is necessarily trivial**.

For $S_3\to\mathbb Z_2$, the 3-cycles map to zero because their order divides three. All transpositions are [conjugate group elements](../../group-action.md#conjugate-group-elements), and a map to an [abelian group](../../group.md#abelian-group) takes conjugate elements to the same value. That common value is either zero or one. Both choices work: they give **the trivial map and the sign homomorphism**, with an odd permutation sent to $1$ and an even permutation sent to $0$.

## 10

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10/a">a</h3>

↑ **Parent:** [10](#10)

<h4 id="10/a/solution">Solution</h4>

↑ **Parent:** [A](#10/a)

The printed wording calls $\Sigma_3$ cyclic, but its meaning in question 9 is the [symmetric group](../../finite-group-theory.md#symmetric-group) $S_3$. Under that interpretation, take its planar [dihedral group](../../finite-group-theory.md#dihedral-group) representation, with

$$
D(r)=\begin{pmatrix}-1/2&-\sqrt3/2\\\sqrt3/2&-1/2\end{pmatrix},\qquad
D(s)=\begin{pmatrix}1&0\\0&-1\end{pmatrix}.
$$

Here $r^3=s^2=1$ and $srs=r^{-1}$. This [representation](../../representation-theory.md#group-representation) is [irreducible](../../representation-theory.md#irreducible-representation) over the complex numbers: the two distinct rotation [eigenspaces](../../linear-operator-theory.md#eigenspace) are exchanged by the reflection, so neither is invariant under the whole group. Its [character](../../representation-theory.md#character-of-a-representation) is $2$ on the identity, $-1$ on the two 3-cycles and $0$ on the three transpositions. Squaring maps each transposition to the identity and permutes the 3-cycles. Its [Frobenius-Schur indicator](../../representation-theory.md#frobenius-schur-indicator) is therefore

$$
\boxed{\nu=\frac{2+3(2)+2(-1)}6=1.}
$$

If “cyclic” were intended literally, no two-dimensional complex [irreducible representation](../../representation-theory.md#irreducible-representation) would exist, since an [irreducible representation of a finite abelian group](../../representation-theory.md#irreducible-representation-of-a-finite-abelian-group) is one-dimensional.

<h3 id="10/b">b</h3>

↑ **Parent:** [10](#10)

<h4 id="10/b/solution">Solution</h4>

↑ **Parent:** [B](#10/b)

**The requested two-dimensional irreducible representation does not exist for the Vierergruppe.** The [Klein four-group](../../finite-group-theory.md#klein-four-group) $V_4$ is an [abelian group](../../group.md#abelian-group) in which every nonidentity element has order two. Its complex [irreducible representations](../../representation-theory.md#irreducible-representation) are all one-dimensional. The same holds over the real numbers here: the commuting representing involutions are simultaneously diagonalizable with real eigenvalues $\pm1$, so every two-dimensional representation has an invariant line. Each genuine irreducible character satisfies $\chi(g^2)=\chi(1)=1$, and hence has [Frobenius-Schur indicator](../../representation-theory.md#frobenius-schur-indicator) $\nu=1$.

The printed notation $C_4$ suggests a different possible interpretation, which must not be conflated with the [Klein four-group](../../finite-group-theory.md#klein-four-group). For the [cyclic group of order four](../../group.md#cyclic-group-of-order-four), a real two-dimensional [irreducible representation](../../representation-theory.md#irreducible-representation) is generated by

$$
J=\begin{pmatrix}0&-1\\1&0\end{pmatrix}.
$$

Its character on $1,J,-I,-J$ is $(2,0,-2,0)$, giving $\nu=(2-2+2-2)/4=0$. Over the complex numbers this representation splits into two conjugate one-dimensional characters, so it is not a two-dimensional complex irreducible representation. These alternatives explain what can be computed without silently changing the printed group or the ground field.

<h3 id="10/c">c</h3>

↑ **Parent:** [10](#10)

<h4 id="10/c/solution">Solution</h4>

↑ **Parent:** [C](#10/c)

For the [symmetric group](../../finite-group-theory.md#symmetric-group) representation in part (a), the identity and three transpositions contribute $4I$ to $A=\sum_gD(g^2)$. The two 3-cycles contribute $D(r)+D(r^2)=-I$. Thus

$$
\boxed{A=3I=\frac{6\cdot1}{2}I.}
$$

More generally, the [central average of representation matrices at squares](../../representation-theory.md#central-average-of-representation-matrices-at-squares) commutes with the representation, because conjugation permutes the summands. For a complex [irreducible representation](../../representation-theory.md#irreducible-representation), [Schur's lemma](../../representation-theory.md#schur-s-lemma) therefore gives $A=cI$. Taking the [trace](../../linear-algebra.md#matrix-trace) yields $c\dim D=|G|\nu$, proving the claimed formula under its correct hypotheses.

For the [Klein four-group](../../finite-group-theory.md#klein-four-group) there is no two-dimensional irreducible representation, as established in part (b). Its genuine one-dimensional irreducibles have $A=4$ and $\nu=1$, so $A=(4\cdot1/1)I$.

If the intended alternative is the real quarter-turn representation of the [cyclic group of order four](../../group.md#cyclic-group-of-order-four), its squared matrices sum to $I-I+I-I=0$. Thus $A=0=(4\cdot0/2)I$ in that example. This equality is a direct calculation; the complex version of [Schur's lemma](../../representation-theory.md#schur-s-lemma) cannot be applied to its reducible complexification.

## ↑ Ancestors (10)

1. [2025](../2025.md)
2. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
3. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
4. [Year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
