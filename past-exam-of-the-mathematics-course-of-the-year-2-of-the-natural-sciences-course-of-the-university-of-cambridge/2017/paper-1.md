# Paper 1

↑ **Parent:** [2017](../2017.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2017/papernst_ib_1_0.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2017/papernst_ib_1_0.pdf)

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
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
- [6](#6)
  - [a](#6/a)
    - [i](#6/a/i)
      - [Solution](#6/a/i/solution)
    - [ii](#6/a/ii)
      - [Solution](#6/a/ii/solution)
    - [iii](#6/a/iii)
      - [Solution](#6/a/iii/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
- [7](#7)
  - [a](#7/a)
    - [Solution](#7/a/solution)
  - [b](#7/b)
    - [Solution](#7/b/solution)
  - [c](#7/c)
    - [i](#7/c/i)
      - [Solution](#7/c/i/solution)
    - [ii](#7/c/ii)
      - [Solution](#7/c/ii/solution)
- [8](#8)
  - [a](#8/a)
    - [Solution](#8/a/solution)
  - [b](#8/b)
    - [Solution](#8/b/solution)
- [9](#9)
  - [a](#9/a)
    - [Solution](#9/a/solution)
  - [b](#9/b)
    - [i](#9/b/i)
      - [Solution](#9/b/i/solution)
    - [ii](#9/b/ii)
      - [Solution](#9/b/ii/solution)
    - [iii](#9/b/iii)
      - [Solution](#9/b/iii/solution)
- [10](#10)
  - [Solution](#10/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a continuously differentiable [vector field](../../multivariable-calculus.md#vector-field) $\mathbf G$ on a bounded volume $V$ with piecewise smooth closed boundary $\partial V$, the [divergence theorem](../../multivariable-calculus.md#divergence-theorem) states

$$
\boxed{\int_{\partial V}\mathbf G\cdot\mathbf n\,dS=\int_V\nabla\cdot\mathbf G\,dV,}
$$

where $\mathbf n$ is the outward [unit normal vector](../../differential-geometry.md#unit-normal). Thus total outward [flux](../../mathematical-physics.md#flux) through a closed surface equals the integral of the local [divergence](../../multivariable-calculus.md#divergence) inside it. A nonclosed surface first needs a suitable closure, with the added surface's [flux](../../mathematical-physics.md#flux) accounted for separately.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

In [cylindrical coordinates](../../multivariable-calculus.md#cylindrical-coordinate-system), the surface has radius $r=\sqrt2z$. It is the lateral surface of a [right circular cone](../../euclidean-geometry.md#right-circular-cone), with vertex at the origin and axis along positive $z$. Its height is $h$ and the limiting upper rim has radius $\sqrt2h$; the horizontal disk at that rim is absent. The half-angle from the vertical satisfies

$$
\boxed{\tan\alpha=\sqrt2,\qquad \alpha\simeq54.7^\circ.}
$$

The upper rim is excluded by $z<h$, which does not affect any convergent [surface integral](../../multivariable-calculus.md#surface-integral). The vertex likewise contributes no area.

<a id="1/b/image-the-open-lateral-cone-and-its-auxiliary-closing-cap"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-1-q1-conical-flux.png)

**[Figure 1](#1/b/image-the-open-lateral-cone-and-its-auxiliary-closing-cap). The open lateral cone and its auxiliary closing cap**. Original sketch in units of $h$. The dashed upper rim bounds an auxiliary disk used only to apply the divergence theorem. The arrow shows the outward lateral normal, which has a downward component.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Close the cone with the horizontal disk $D$ at height $h$, and let $V$ be the enclosed solid. The [divergence](../../multivariable-calculus.md#divergence) is

$$
\nabla\cdot\mathbf G=3x^2+2y+3y^2+1=3r^2+2y+1.
$$

The term $2y$ integrates to zero by reflection symmetry of each circular cross-section. Using the [divergence theorem](../../multivariable-calculus.md#divergence-theorem) and [cylindrical coordinates](../../multivariable-calculus.md#cylindrical-coordinate-system), the closed-surface [flux](../../mathematical-physics.md#flux) is

$$
\int_V\nabla\cdot\mathbf G\,dV
=\int_0^h\int_0^{2\pi}\int_0^{\sqrt2z}(3r^2+1)r\,dr\,d\varphi\,dz
=\int_0^h(6\pi z^4+2\pi z^2)\,dz
=\frac{6\pi h^5}{5}+\frac{2\pi h^3}{3}.
$$

The outward normal on $D$ is $+\widehat{\mathbf z}$, so its [flux](../../mathematical-physics.md#flux) is its area times $G_z=h$:

$$
\int_D\mathbf G\cdot\mathbf n\,dS=h\,\pi(\sqrt2h)^2=2\pi h^3.
$$

Subtracting this cap contribution gives the required lateral [flux](../../mathematical-physics.md#flux):

$$
\boxed{\int_A\mathbf G\cdot d\mathbf A=\frac{6\pi h^5}{5}-\frac{4\pi h^3}{3}.}
$$

This is [conical flux by closing with a cap](../../multivariable-calculus.md#conical-flux-by-closing-with-a-cap). The normal convention matters: on the lateral cone the outward normal points radially outwards and partly downwards, so the $G_z$ contribution to the lateral [flux](../../mathematical-physics.md#flux) is negative. To justify applying the theorem at the vertex, truncate a small tip and take its size to zero; the extra [flux](../../mathematical-physics.md#flux) vanishes because $\mathbf G$ is regular there.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For $v=(t+1)^2u$, the derivatives are

$$
v_t=2(t+1)u+(t+1)^2u_t,\qquad v_{xx}=(t+1)^2u_{xx}.
$$

Substitution cancels the two terms $2(t+1)u$, giving the [diffusion equation](../../diffusion-equation.md)

$$
\boxed{u_t=u_{xx},\qquad u(0,t)=0,\quad u(\pi,t)=\frac{f(t)}{(t+1)^2},\quad u(x,0)=h(x).}
$$

This is a [scalar integrating factor for a reaction-diffusion equation](../../diffusion-equation.md#scalar-integrating-factor-for-a-reaction-diffusion-equation), since $\exp[\int2\,dt/(t+1)]=(t+1)^2$ up to a constant. We use $t\geq0$, so the factor never vanishes. A classical solution at the initial corners additionally requires compatible data, $h(0)=0$ and $h(\pi)=f(0)$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The transformed endpoint values are $u(0,t)=0$ and $u(\pi,t)=3$. Apply [boundary lifting](../../boundary-value-problem.md#boundary-lifting) with $u=3x/\pi+w$. The lifted profile is linear, so $w_t=w_{xx}$ with homogeneous [Dirichlet boundary conditions](../../differential-equation.md#dirichlet-boundary-condition) and

$$
w(x,0)=\frac{\sin2x}{\pi}.
$$

For [separation of variables](../../partial-differential-equation.md#separation-of-variables), put $w=X(x)T(t)$. Then $X''/X=T'/T=-\lambda$. The endpoint conditions give nonzero spatial modes only for $\lambda=n^2$, $n=1,2,\ldots$, with $X_n=\sin nx$ and $T_n=e^{-n^2t}$. Hence

$$
w(x,t)=\sum_{n=1}^{\infty}b_ne^{-n^2t}\sin nx,\qquad
b_n=\frac2\pi\int_0^\pi\frac{\sin2x}{\pi}\sin nx\,dx=\frac{\delta_{n2}}\pi,
$$

by [orthogonality](../../inner-product.md#orthogonal-vectors) of the sine modes. Only the $n=2$ mode is present. Undoing both substitutions gives

$$
\boxed{v(x,t)=\frac{(t+1)^2}{\pi}\left(3x+e^{-4t}\sin2x\right).}
$$

At $t=0$ this has the prescribed initial profile, and at $x=\pi$ it is $3(t+1)^2$. Differentiating also verifies the original evolution equation directly.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The nonstationary part of $u$ decays exponentially, whereas the integrating factor grows quadratically. For fixed $x>0$,

$$
\frac{v(x,t)}{3xt^2/\pi}
=\left(1+\frac1t\right)^2\left(1+\frac{e^{-4t}\sin2x}{3x}\right)\longrightarrow1.
$$

Consequently

$$
\boxed{v(x,t)\sim\frac{3xt^2}{\pi}\qquad(t\to\infty).}
$$

At $x=0$, both expressions are identically zero; the ratio formulation is understood for $x>0$. The diffusion modes have died away, leaving the lifted linear profile multiplied by the reaction-induced amplitude factor.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [causal Green function](../../green-s-function.md#causal-green-function) vanishes before the impulse. For $t>\tau$ it solves the homogeneous [linear ordinary differential equation](../../linear-ordinary-differential-equation.md), whose characteristic roots are $-q\pm2i$. Thus it has the form

$$
G(t,\tau)=e^{-q(t-\tau)}[A\cos2(t-\tau)+B\sin2(t-\tau)].
$$

Continuity at $t=\tau$ is necessary to avoid a delta derivative in $G_{tt}$, so $A=0$. Integrating its forced equation across the impulse gives the [jump condition for an impulse](../../linear-ordinary-differential-equation.md#jump-condition-for-an-impulse), $G_t(\tau^+,\tau)-G_t(\tau^-,\tau)=1$. The derivative from below is zero and the derivative from above is $2B$, giving

$$
\boxed{G(t,\tau)=\frac12\Theta(t-\tau)e^{-q(t-\tau)}\sin[2(t-\tau)].}
$$

Here $\Theta$ is the [Heaviside step function](../../integral-transform.md#heaviside-step-function). The zero initial data exclude any additional homogeneous response. By the [superposition principle](../../vector-space.md#superposition-principle), the output for a general locally integrable input is

$$
\boxed{x(t)=\int_0^tG(t,\tau)f(\tau)\,d\tau
=\frac12\int_0^te^{-q(t-\tau)}\sin[2(t-\tau)]f(\tau)\,d\tau.}
$$

The upper endpoint causes no unwanted term in the first derivative because $G(t,t)=0$; in the second derivative its unit derivative jump reproduces the input.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The pulse height is the constant $t_0$, not the time variable. In the undamped case the [convolution](../../fourier-analysis.md#convolution) therefore reduces to

$$
x(t)=\frac{t_0}{2}\int_0^{\min(t,t_0)}\sin[2(t-\tau)]\,d\tau.
$$

Integration gives the continuous displacement and velocity

$$
\boxed{x(t)=\begin{cases}
\displaystyle\frac{t_0}{4}(1-\cos2t),&0\leq t<t_0,\\
\displaystyle\frac{t_0}{4}\left[\cos2(t-t_0)-\cos2t\right],&t\geq t_0.
\end{cases}}
$$

The post-pulse expression is equivalently $x(t)=(t_0/2)\sin t_0\sin(2t-t_0)$. Since $t_0>0$, it vanishes for every subsequent time precisely when $\sin t_0=0$. Thus

$$
\boxed{t_0=n\pi,\qquad n=1,2,3,\ldots.}
$$

These are integer multiples of the oscillator's natural period $\pi$. At such switch-off times both $x(t_0)$ and $x'(t_0)$ are zero. Vanishing displacement alone would not suffice: a nonzero switch-off velocity would restart an oscillation. This is [rectangular-pulse cancellation of an undamped oscillator](../../classical-mechanics.md#rectangular-pulse-cancellation-of-an-undamped-oscillator).

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For the stated forward [Fourier transform](../../fourier-transform.md), the inverse has the opposite exponential sign and a factor $1/(2\pi)$:

$$
\boxed{f(t)=\frac1{2\pi}\int_{-\infty}^{\infty}\widetilde f(\omega)e^{i\omega t}\,d\omega.}
$$

This holds under the usual hypotheses for [Fourier inversion](../../fourier-analysis.md#fourier-inversion-theorem), or in the sense of [distributions](../../distribution-theory.md#distribution-mathematical-analysis) when appropriate.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Suppose initially that $f,g$ are absolutely integrable, so [Fubini's theorem](../../measure-theory.md#fubini-s-theorem) justifies exchanging the integrations. The transform of their [convolution](../../fourier-analysis.md#convolution) is

$$
\widetilde h(\omega)=\int_{-\infty}^{\infty}\int_{-\infty}^{\infty}f(t)g(z-t)e^{-i\omega z}\,dt\,dz.
$$

Set $s=z-t$, so $z=s+t$ and $dz=ds$. The exponential separates:

$$
\widetilde h(\omega)=\left[\int_{-\infty}^{\infty}f(t)e^{-i\omega t}\,dt\right]
\left[\int_{-\infty}^{\infty}g(s)e^{-i\omega s}\,ds\right].
$$

Therefore the [convolution theorem](../../fourier-analysis.md#convolution-theorem) is

$$
\boxed{\widetilde{f*g}(\omega)=\widetilde f(\omega)\widetilde g(\omega).}
$$

No extra $2\pi$ occurs in this direction with the specified normalization.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Since $\gamma>0$, the causal damped sine has an absolutely convergent [Fourier transform](../../fourier-transform.md) for real $\omega$. Resolving the sine into complex exponentials gives

$$
\widetilde f(\gamma,p,\omega)
=\frac1{2i}\int_0^\infty\left[e^{-[\gamma+i(\omega-p)]t}-e^{-[\gamma+i(\omega+p)]t}\right]dt
=\frac1{2i}\left[\frac1{\gamma+i(\omega-p)}-\frac1{\gamma+i(\omega+p)}\right].
$$

Combining the two fractions yields

$$
\boxed{\widetilde f(\gamma,p,\omega)=\frac{p}{(\gamma+i\omega)^2+p^2}.}
$$

The formula also includes $p=0$, for which both the original function and its transform vanish. Its sign reverses when the real parameter $p$ reverses.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

For an integrable applied voltage, the [convolution theorem](../../fourier-analysis.md#convolution-theorem) gives

$$
\widetilde I(\omega)=\left[\frac{a_1p_1}{(\gamma_1+i\omega)^2+p_1^2}
+\frac{a_2p_2}{(\gamma_2+i\omega)^2+p_2^2}\right]\widetilde V(\omega).
$$

The integrated [electric current](../../electric-charge.md#electric-current) is the zero-frequency transform, $Q=\widetilde I(0)$. Since $\widetilde V(0)$ can be arbitrary, zero total [electric charge](../../electric-charge.md) for every such input is equivalent to

$$
\boxed{\frac{a_1p_1}{\gamma_1^2+p_1^2}+\frac{a_2p_2}{\gamma_2^2+p_2^2}=0.}
$$

For nonzero $p_1,p_2$, this can be written

$$
\boxed{\frac{a_1}{a_2}=-\frac{p_2(\gamma_1^2+p_1^2)}{p_1(\gamma_2^2+p_2^2)}.}
$$

Because both amplitudes are positive, nonzero $p_1,p_2$ must have opposite signs. If exactly one $p_i$ is zero there is no cancellation with positive amplitudes; if both vanish the kernel is identically zero and any amplitudes work. In particular, if both frequency parameters were additionally required to be positive, no such nontrivial system would exist. The PDF requires positivity of $a_i,\gamma_i$, but allows real fixed $p_i$.

This is [zero-frequency cancellation of a causal response kernel](../../statistical-physics.md#zero-frequency-cancellation-of-a-causal-response-kernel). The phrase arbitrary voltage is understood within a class for which the net-charge integrals exist; a permanent DC input need not have finite total charge.

## 5

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

An $n\times n$ [matrix](../../vector-space.md#matrix) is [diagonalizable](../../linear-operator-theory.md#diagonalizable-matrix) over a chosen field exactly when it has a basis of $n$ linearly independent [eigenvectors](../../linear-operator-theory.md#eigenvector). Equivalently, $P^{-1}AP$ is diagonal for some invertible $P$. Distinct [eigenvalues](../../linear-operator-theory.md#eigenvalue) suffice but are not necessary. For example,

$$
J=\begin{pmatrix}1&1\\0&1\end{pmatrix}
$$

is not diagonalizable: its only [eigenvalue](../../linear-operator-theory.md#eigenvalue) is $1$ and its [eigenspace](../../linear-operator-theory.md#eigenspace) is the one-dimensional span of $(1,0)^T$. It is a nontrivial [Jordan block](../../linear-operator-theory.md#jordan-block).

A [Hermitian matrix](../../hilbert-space.md#hermitian-operator) satisfies $A^\dagger=A$, where the dagger denotes [conjugate transpose](../../linear-operator-theory.md#conjugate-transpose). If $Av=\lambda v$ with $v\ne0$, then

$$
\lambda=\frac{v^\dagger Av}{v^\dagger v},\qquad
(v^\dagger Av)^*=v^\dagger A^\dagger v=v^\dagger Av.
$$

The denominator is positive real, so

$$
\boxed{\lambda\in\mathbb R.}
$$

For $Av=\lambda v$ and $Aw=\mu w$, Hermiticity also gives

$$
\mu v^\dagger w=v^\dagger Aw=(Av)^\dagger w=\lambda v^\dagger w.
$$

Thus

$$
\boxed{\lambda\ne\mu\quad\Longrightarrow\quad v^\dagger w=0.}
$$

This is the necessary qualification to the PDF's [orthogonality](../../inner-product.md#orthogonal-vectors) wording: arbitrary [eigenvectors](../../linear-operator-theory.md#eigenvector) belonging to a repeated [eigenvalue](../../linear-operator-theory.md#eigenvalue) need not be orthogonal. Within each repeated [eigenspace](../../linear-operator-theory.md#eigenspace), [Gram-Schmidt orthogonalization](../../inner-product.md#gram-schmidt-process) produces an orthonormal basis; together the [eigenspaces](../../linear-operator-theory.md#eigenspace) give an [orthonormal eigenbasis](../../linear-operator-theory.md#orthonormal-eigenbasis) by the [finite-dimensional spectral theorem](../../linear-operator-theory.md#finite-dimensional-spectral-theorem). For example, $(1,0)^T$ and $(1,1)^T$ are nonorthogonal [eigenvectors](../../linear-operator-theory.md#eigenvector) of the identity [matrix](../../vector-space.md#matrix).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

The $xy$ block has characteristic [polynomial](../../polynomial.md) $(2-\lambda)^2-a^2$. A convenient [orthonormal eigenbasis](../../linear-operator-theory.md#orthonormal-eigenbasis) for the full real [symmetric matrix](../../linear-algebra.md#symmetric-matrix) is

$$
e_+=\frac1{\sqrt2}(1,1,0)^T,\qquad e_-=\frac1{\sqrt2}(1,-1,0)^T,\qquad e_z=(0,0,1)^T,
$$

with [eigenvalues](../../linear-operator-theory.md#eigenvalue) $2-a$, $2+a$, and $c$, respectively. Hence its [orthogonal diagonalization](../../linear-algebra.md#orthogonal-diagonalization-of-a-real-symmetric-matrix) is

$$
\boxed{P^TAP=\operatorname{diag}(2-a,2+a,c),\qquad
P=\begin{pmatrix}1/\sqrt2&1/\sqrt2&0\\1/\sqrt2&-1/\sqrt2&0\\0&0&1\end{pmatrix}.}
$$

For repeated [eigenvalues](../../linear-operator-theory.md#eigenvalue), every nonzero combination within the corresponding [eigenspace](../../linear-operator-theory.md#eigenspace) is also an [eigenvector](../../linear-operator-theory.md#eigenvector); the displayed basis remains valid. Introduce [principal axes](../../rigid-body-dynamics.md#principal-axis) coordinates

$$
X=\frac{x+y}{\sqrt2},\qquad Y=\frac{x-y}{\sqrt2},\qquad Z=z.
$$

The [quadratic form](../../quadratic-form.md) becomes

$$
(2-a)X^2+(2+a)Y^2+cZ^2=1.
$$

The [principal-axis reduction of a quadric](../../quadratic-form.md#principal-axis-reduction-of-a-quadric) therefore has three regimes.

For $0<a<2$, all coefficients are positive: the surface is an [ellipsoid](../../euclidean-geometry.md#ellipsoid) centred at the origin, with

$$
\boxed{\text{semiaxes }\frac1{\sqrt{2-a}},\quad\frac1{\sqrt{2+a}},\quad\frac1{\sqrt c}
\quad\text{along }e_+,e_-,e_z.}
$$

For $a=2$, the $X$ term disappears. The surface is an [elliptic cylinder](../../euclidean-geometry.md#elliptic-cylinder), unbounded along $e_+$, whose cross-section is $4Y^2+cZ^2=1$:

$$
\boxed{\text{cylinder axis }e_+,\qquad\text{cross-section semiaxes }\frac12,\ \frac1{\sqrt c}.}
$$

For $a>2$, there is one negative coefficient, so the surface is a one-sheet [hyperboloid](../../differential-geometry.md#hyperboloid):

$$
\boxed{(a+2)Y^2+cZ^2-(a-2)X^2=1,\qquad\text{axis }e_+.}
$$

Its waist at $X=0$ is an ellipse with semiaxes $(a+2)^{-1/2}$ and $c^{-1/2}$. At other $X$, both waist radii are multiplied by $\sqrt{1+(a-2)X^2}$. There is no intercept on its longitudinal axis. Its asymptotic cone is $(a+2)Y^2+cZ^2=(a-2)X^2$. If positive [eigenvalues](../../linear-operator-theory.md#eigenvalue) coincide, the corresponding choice of [principal axes](../../rigid-body-dynamics.md#principal-axis) is not unique, reflecting a rotational symmetry of the surface.

<a id="5/b/image-ellipsoid-elliptic-cylinder-and-one-sheet-hyperboloid-in-principal-coordinates"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-1-q5-principal-quadrics.png)

**[Figure 2](#5/b/image-ellipsoid-elliptic-cylinder-and-one-sheet-hyperboloid-in-principal-coordinates). Ellipsoid, elliptic cylinder, and one-sheet hyperboloid in principal coordinates**. Original calculated examples with $c=1$ and $a=1,2,3$. The horizontal longitudinal coordinate $X$ is directed along $(1,1,0)/\sqrt2$ in the original coordinates. Cylinder and hyperboloid plots show finite portions of unbounded surfaces.

## 6

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/i">i</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/i/solution">Solution</h5>

↑ **Parent:** [I](#6/a/i)

Using $(AB)^\dagger=B^\dagger A^\dagger$, the [conjugate transpose](../../linear-operator-theory.md#conjugate-transpose) of the proposed [matrix](../../vector-space.md#matrix) is

$$
H^\dagger=-i(B^\dagger A^\dagger-A^\dagger B^\dagger)
=-i(BA-AB)=i(AB-BA)=H.
$$

Thus

$$
\boxed{i[A,B]\ \text{is Hermitian}.}
$$

The [commutator](../../lie-algebra.md#commutator) of two [Hermitian matrices](../../hilbert-space.md#hermitian-operator) is skew-Hermitian, and multiplication by $i$ changes it into a [Hermitian matrix](../../hilbert-space.md#hermitian-operator). No simplicity assumption on the spectra is needed for this part.

<h4 id="6/a/ii">ii</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/a/ii)

Suppose first that $AB=BA$, and take an [eigenvector](../../linear-operator-theory.md#eigenvector) $v_j$ of $A$, with $Av_j=a_jv_j$. Commutation gives

$$
A(Bv_j)=BAv_j=a_jBv_j.
$$

Since the [eigenvalue](../../linear-operator-theory.md#eigenvalue) $a_j$ is simple, its [eigenspace](../../linear-operator-theory.md#eigenspace) is one-dimensional, so $Bv_j=b_jv_j$ for some scalar $b_j$. Thus every vector in an [eigenbasis](../../linear-operator-theory.md#eigenbasis) of $A$ is also an [eigenvector](../../linear-operator-theory.md#eigenvector) of $B$. The simple spectrum of $B$ ensures these account for its [eigenvector](../../linear-operator-theory.md#eigenvector) directions as well. [Eigenvectors](../../linear-operator-theory.md#eigenvector) are understood up to nonzero scaling and permutation, rather than as literally identical numerical vectors.

Conversely, if $v_1,\ldots,v_n$ are a common [eigenbasis](../../linear-operator-theory.md#eigenbasis) with $Av_j=a_jv_j$ and $Bv_j=b_jv_j$, then

$$
(AB-BA)v_j=(a_jb_j-b_ja_j)v_j=0
$$

for every basis vector. Hence $AB-BA=0$. Therefore

$$
\boxed{\text{common eigenvector directions}\quad\Longleftrightarrow\quad AB=BA.}
$$

This is [simple spectrum gives simultaneous diagonalization](../../mathematics.md#simple-spectrum-gives-simultaneous-diagonalization). Without simple spectra, commuting [Hermitian matrices](../../hilbert-space.md#hermitian-operator) still possess a common [orthonormal eigenbasis](../../linear-operator-theory.md#orthonormal-eigenbasis), but not every arbitrary [eigenvector](../../linear-operator-theory.md#eigenvector) of one [matrix](../../vector-space.md#matrix) must be an [eigenvector](../../linear-operator-theory.md#eigenvector) of the other.

<h4 id="6/a/iii">iii</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#6/a/iii)

Choose the common [orthonormal eigenbasis](../../linear-operator-theory.md#orthonormal-eigenbasis) established in part (ii), and let $U$ be the [unitary matrix](../../linear-operator-theory.md#unitary-matrix) of its columns. Then

$$
U^\dagger AU=\operatorname{diag}(a_1,\ldots,a_n),\qquad
U^\dagger BU=\operatorname{diag}(b_1,\ldots,b_n).
$$

Consequently

$$
\boxed{U^\dagger(A+iB)U=\operatorname{diag}(a_1+ib_1,\ldots,a_n+ib_n).}
$$

Thus $N$ is unitarily diagonalizable, even though it need not be Hermitian. As a consistency check, commutation also gives $NN^\dagger=N^\dagger N=A^2+B^2$, so $N$ is a [normal matrix](../../linear-operator-theory.md#normal-matrix), as also follows from [unitary diagonalization of a normal matrix](../../linear-operator-theory.md#unitary-diagonalization-of-a-normal-matrix).

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Since $C$ is unitary, $C^{-1}=C^\dagger$. Hence $B=C^{-1}AC=C^\dagger AC$ is Hermitian, and so is its positive integer power:

$$
(B^p)^\dagger=(B^\dagger)^p=B^p.
$$

It follows that $B^p$ has real [eigenvalues](../../linear-operator-theory.md#eigenvalue). More explicitly, cancellation of adjacent $CC^{-1}$ factors gives the [similarity transformation](../../linear-algebra.md#similarity-transformation)

$$
(C^{-1}AC)^p=C^{-1}A^pC.
$$

If the real [eigenvalues](../../linear-operator-theory.md#eigenvalue) of $A$ are $\lambda_j$, the [eigenvalues](../../linear-operator-theory.md#eigenvalue) in question are therefore

$$
\boxed{\lambda_1^p,\ldots,\lambda_n^p\in\mathbb R.}
$$

For even $p$ they are nonnegative; for odd $p$ their signs can be either. The similarity argument actually works for every invertible $C$, although the Hermiticity argument uses its unitarity.

## 7

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

The [Cauchy-Riemann equations](../../analysis.md#cauchy-riemann-equations) give $u_x=v_y$ and $u_y=-v_x$. Therefore

$$
|\nabla u|^2=u_x^2+u_y^2=v_y^2+v_x^2=|\nabla v|^2.
$$

Taking the nonnegative square root yields

$$
\boxed{|\nabla u|=|\nabla v|.}
$$

The two [gradients](../../multivariable-calculus.md#gradient) are also orthogonal, since $\nabla u\cdot\nabla v=v_yv_x-v_xv_y=0$, although equality of their lengths alone is the requested result.

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/solution">Solution</h4>

↑ **Parent:** [B](#7/b)

Differentiate the prescribed imaginary part with respect to $y$:

$$
v_y=e^x[(1+x)\cos y-y\sin y].
$$

The [Cauchy-Riemann equation](../../analysis.md#cauchy-riemann-equations) $u_x=v_y$ integrates to

$$
u=e^x(x\cos y-y\sin y)+F(y).
$$

Its $y$ derivative is $u_y=-e^x[(x+1)\sin y+y\cos y]+F'(y)$. On the other hand, $-v_x=-e^x[(x+1)\sin y+y\cos y]$. The second [Cauchy-Riemann equation](../../analysis.md#cauchy-riemann-equations) therefore requires $F'(y)=0$. Combining the real and imaginary parts,

$$
e^x[(x\cos y-y\sin y)+i(y\cos y+x\sin y)]=(x+iy)e^{x+iy}.
$$

Thus the most general answer on a connected domain is

$$
\boxed{f(z)=ze^z+C,\qquad C\in\mathbb R.}
$$

A real constant preserves the given imaginary part. Conversely, the difference of any two such [analytic functions](../../holomorphic-function.md) has zero imaginary part, and its Cauchy-Riemann derivatives force it to be constant. This proves completeness, rather than only exhibiting one possible [harmonic conjugate](../../partial-differential-equation.md#harmonic-conjugate).

<h3 id="7/c">c</h3>

↑ **Parent:** [7](#7)

<h4 id="7/c/i">i</h4>

↑ **Parent:** [C](#7/c)

<h5 id="7/c/i/solution">Solution</h5>

↑ **Parent:** [I](#7/c/i)

For coefficients $a_n=1/\ln n$, the [Cauchy-Hadamard theorem](../../sequence-and-series.md#cauchy-hadamard-theorem) gives $R^{-1}=\limsup|a_n|^{1/n}$. Here

$$
|a_n|^{1/n}=\exp\left[-\frac{\ln\ln n}{n}\right]\longrightarrow1.
$$

Therefore

$$
\boxed{R=1.}
$$

Omitting the first two powers has no effect on the [radius of convergence](../../sequence-and-series.md#radius-of-convergence).

<h4 id="7/c/ii">ii</h4>

↑ **Parent:** [C](#7/c)

<h5 id="7/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7/c/ii)

Let $a_n=(1+p/n)^{n^2}$. For every fixed real $p$, the base is positive once $n$ is sufficiently large; any initial negative or zero bases affect only finitely many coefficients. For that tail,

$$
\ln|a_n|^{1/n}=n\ln\left(1+\frac pn\right)=p-\frac{p^2}{2n}+O(n^{-2})\longrightarrow p.
$$

The [Cauchy-Hadamard theorem](../../sequence-and-series.md#cauchy-hadamard-theorem) therefore yields

$$
\boxed{R=e^{-p}\qquad\text{for every real }p.}
$$

For example $p=0$ recovers the geometric-series radius one. The stronger expansion $a_n=e^{pn-p^2/2+O(1/n)}$ also shows that, on $|z|=e^{-p}$, the magnitudes of the individual terms tend to $e^{-p^2/2}>0$. Thus this series diverges at every point on its convergence circle; the radius itself does not require that extra boundary analysis.

## 8

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8/a">a</h3>

↑ **Parent:** [8](#8)

<h4 id="8/a/solution">Solution</h4>

↑ **Parent:** [A](#8/a)

The origin is an [ordinary point](../../complex-analysis.md#ordinary-point-criterion-for-a-second-order-equation) of the [Hermite differential equation](../../analysis.md#hermite-differential-equation), so put $y=\sum_{n=0}^{\infty}a_nx^n$. Substitution and matching powers gives

$$
\sum_{n=0}^{\infty}\left[(n+2)(n+1)a_{n+2}+(\lambda-2n)a_n\right]x^n=0.
$$

Thus the [linear recurrence relation](../../algebra.md#linear-recurrence-relation) is

$$
\boxed{a_{n+2}=\frac{2n-\lambda}{(n+2)(n+1)}a_n,\qquad n\geq0.}
$$

Even and odd coefficients evolve independently from arbitrary $a_0,a_1$. The general [power series](../../sequence-and-series.md#power-series) solution is

$$
\boxed{y(x)=a_0\sum_{j=0}^{\infty}\frac{\prod_{r=0}^{j-1}(4r-\lambda)}{(2j)!}x^{2j}
+a_1\sum_{j=0}^{\infty}\frac{\prod_{r=0}^{j-1}(4r+2-\lambda)}{(2j+1)!}x^{2j+1},}
$$

with an empty product equal to one. Its first terms are

$$
y=a_0\left[1-\frac\lambda2x^2+\frac{\lambda(\lambda-4)}{24}x^4+\cdots\right]
+a_1\left[x+\frac{2-\lambda}{6}x^3+\frac{(2-\lambda)(6-\lambda)}{120}x^5+\cdots\right].
$$

Both series converge at every finite $x$, since the ratio of successive terms in each parity subsequence tends to zero. For a nonzero [polynomial](../../polynomial.md) of degree $N$, the highest coefficient in the [differential equation](../../differential-equation.md) requires $\lambda=2N$. Conversely, at such a value the appropriate parity series terminates, while its opposite-parity initial coefficient can be set to zero. Hence

$$
\boxed{\lambda=2N,\qquad N=0,1,2,\ldots,\qquad y\propto H_N(x).}
$$

Here $H_N$ is a physicists' [Hermite polynomial](../../orthogonal-polynomial.md#hermite-polynomial). Two explicit choices are

$$
\boxed{\lambda=4:\ y=4x^2-2,\qquad \lambda=6:\ y=8x^3-12x.}
$$

Direct differentiation verifies both. These are [polynomial](../../polynomial.md) solutions up to an arbitrary overall factor. Without a [polynomial](../../polynomial.md) requirement or additional [boundary conditions](../../differential-equation.md#boundary-condition), the equation also has nonpolynomial solutions for other real $\lambda$; discreteness here comes from termination.

<h3 id="8/b">b</h3>

↑ **Parent:** [8](#8)

<h4 id="8/b/solution">Solution</h4>

↑ **Parent:** [B](#8/b)

Insert the [Frobenius solution](../../complex-analysis.md#frobenius-solution) and its differentiated series into the equation. Collecting the terms before shifting an index gives

$$
\sum_{n=0}^{\infty}(n+\sigma)(n+\sigma+\gamma-1)a_nx^{n+\sigma-1}
-\sum_{n=0}^{\infty}(n+\sigma+\alpha)(n+\sigma+\beta)a_nx^{n+\sigma}=0.
$$

The coefficient of the lowest power $x^{\sigma-1}$ is $a_0\sigma(\sigma+\gamma-1)$. Because $a_0\ne0$, the [indicial equation](../../linear-ordinary-differential-equation.md#indicial-equation) gives

$$
\boxed{\sigma=0\quad\text{or}\quad\sigma=1-\gamma.}
$$

For the coefficient of $x^{n+\sigma-1}$ with $n\geq1$, shift the index in the second sum. The [hypergeometric Frobenius recurrence](../../complex-analysis.md#hypergeometric-frobenius-recurrence) is

$$
\boxed{(n+\sigma)(n+\sigma+\gamma-1)a_n
=(n+\sigma+\alpha-1)(n+\sigma+\beta-1)a_{n-1}.}
$$

Whenever the left coefficient is nonzero, division yields

$$
\boxed{a_n=\frac{(n+\sigma+\alpha-1)(n+\sigma+\beta-1)}{(n+\sigma)(n+\sigma+\gamma-1)}a_{n-1}.}
$$

For noninteger $\gamma$, the two independent local solutions can therefore be identified as

$$
y_1={}_2F_1(\alpha,\beta;\gamma;x),\qquad
y_2=x^{1-\gamma}{}_2F_1(\alpha-\gamma+1,\beta-\gamma+1;2-\gamma;x),
$$

with a consistent local branch for the fractional power. The [hypergeometric function](../../complex-analysis.md#hypergeometric-function) coefficients follow by iterating the recurrence using [rising factorials](../../combinatorics.md#rising-factorial).

There is a parameter qualification to the PDF's statement for all real constants: a zero denominator cannot be divided through. At an [undetermined coefficient at Frobenius resonance](../../complex-analysis.md#undetermined-coefficient-at-frobenius-resonance), use the undivided coefficient equation to test compatibility. For example, $\gamma=0,\sigma=0,n=1$ requires $0=\alpha\beta a_0$, so a pure exponent-zero series with $a_0\ne0$ is impossible if $\alpha\beta\ne0$. When $\gamma=1$ the two [indicial roots](../../linear-ordinary-differential-equation.md#indicial-root) coincide, and a second independent solution generally needs a logarithmic term. The [indicial roots](../../linear-ordinary-differential-equation.md#indicial-root) and undivided relation remain the valid coefficient conclusions in these exceptional cases.

## 9

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9/a">a</h3>

↑ **Parent:** [9](#9)

<h4 id="9/a/solution">Solution</h4>

↑ **Parent:** [A](#9/a)

Define $h=f-y'f_{y'}$. For a density without explicit $x$ dependence, the chain rule gives

$$
\frac{dh}{dx}=f_yy'+f_{y'}y''-y''f_{y'}-y'\frac d{dx}f_{y'}
=y'\left(f_y-\frac d{dx}f_{y'}\right).
$$

Thus the [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation) implies the [Beltrami identity](../../analysis.md#beltrami-identity)

$$
\boxed{h=f-y'\frac{\partial f}{\partial y'}=\text{constant},\qquad\frac{dh}{dx}=0.}
$$

Where $y'\ne0$ this first integral is equivalent to the original equation. At a turning point it extends by continuity. On an entire constant segment, however, its derivative alone can vanish without imposing the full [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation), so such candidate paths must still be checked in the original equation.

<h3 id="9/b">b</h3>

↑ **Parent:** [9](#9)

<h4 id="9/b/i">i</h4>

↑ **Parent:** [B](#9/b)

<h5 id="9/b/i/solution">Solution</h5>

↑ **Parent:** [I](#9/b/i)

The monotonic horizontal coordinate allows the path to be written as a graph. Its [arc length](../../riemannian-geometry.md#arc-length) element is $ds=\sqrt{1+y'^2}\,dx$, so the variational density is $f(y,y')=g(y)\sqrt{1+y'^2}$. It has no explicit horizontal-coordinate dependence. The [Beltrami identity](../../analysis.md#beltrami-identity) becomes

$$
f-y'f_{y'}=g\sqrt{1+y'^2}-\frac{g y'^2}{\sqrt{1+y'^2}}
=\frac{g}{\sqrt{1+y'^2}}.
$$

Consequently every smooth minimizing path satisfies

$$
\boxed{\frac d{dx}\left(\frac{g(y)}{\sqrt{1+y'^2}}\right)=0.}
$$

This is a first integral of the weighted arc-length problem; fixed endpoint values remove the endpoint variation terms.

<h4 id="9/b/ii">ii</h4>

↑ **Parent:** [B](#9/b)

<h5 id="9/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#9/b/ii)

Interpret the density $1/y$ on the physical region $y>0$. It is singular at zero and would not describe a nonnegative density for $y<0$. The first integral gives $y\sqrt{1+y'^2}=R$ for a positive constant $R$. To handle the horizontal tangent without dividing by $y'$, use the full [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation):

$$
yy''+y'^2+1=0,\qquad (yy')'=-1.
$$

Two integrations give $y^2=-(x-x_0)^2+R^2$. The equal endpoint heights force $x_0=0$, and either endpoint then gives $R^2=2$. Thus

$$
\boxed{y(x)=\sqrt{2-x^2},\qquad -1\leq x\leq1.}
$$

The path is the upper circular arc. A constant horizontal path solves the differentiated first integral trivially but fails $yy''+y'^2+1=0$, so is not another extremum.

One can prove global minimality, rather than only stationarity. Define $\Phi(x,y)=\operatorname{arsinh}(x/y)$ on the upper half-plane. Then

$$
\nabla\Phi=\frac{(1,-x/y)}{\sqrt{x^2+y^2}},\qquad |\nabla\Phi|=\frac1y.
$$

The [Cauchy-Schwarz inequality](../../probability-and-statistics.md#cauchy-schwarz-inequality) gives, along any admissible path from $A$ to $B$,

$$
D=\int\frac{ds}{y}\geq\int\nabla\Phi\cdot d\mathbf r
=\Phi(1,1)-\Phi(-1,1)=2\operatorname{arsinh}1.
$$

Our circle has tangent $(1,-x/y)$ for increasing $x$, so equality holds pointwise. This [calibration for semicircular hyperbolic geodesics](../../hyperbolic-geometry.md#calibration-for-semicircular-hyperbolic-geodesics) proves

$$
\boxed{D_{\min}=2\operatorname{arsinh}1=2\ln(1+\sqrt2).}
$$

The geometry is that of a [hyperbolic geodesic](../../hyperbolic-geometry.md#geodesic-in-the-poincare-half-plane-model) in the [Poincaré half-plane model](../../hyperbolic-geometry.md#poincare-half-plane-model). The proof even allows competing upper-half-plane paths beyond the class of monotonic graphs.

<h4 id="9/b/iii">iii</h4>

↑ **Parent:** [B](#9/b)

<h5 id="9/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#9/b/iii)

The path rises from $(-1,1)$ to its maximum height $\sqrt2$ at $x=0$, then falls symmetrically to $(1,1)$. Its radius is $\sqrt2$, and its endpoint polar angles are $3\pi/4$ and $\pi/4$, giving angular span $\pi/2$. Hence its ordinary [arc length](../../riemannian-geometry.md#arc-length) is

$$
\boxed{L=\sqrt2\,\frac\pi2=\frac\pi{\sqrt2}\simeq2.22144.}
$$

Equivalently, $\sqrt{1+y'^2}=\sqrt2/\sqrt{2-x^2}$ and integrating over $[-1,1]$ gives the same value. This Euclidean length differs from the weighted destruction integral $D_{\min}\simeq1.76275$: the slightly longer route saves undergrowth by travelling at greater height.

<a id="9/b/iii/image-the-least-destruction-path-bends-towards-lower-density"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-1-q9-minimum-destruction-path.png)

**[Figure 3](#9/b/iii/image-the-least-destruction-path-bends-towards-lower-density). The least-destruction path bends towards lower density**. Original exact semicircular minimizer and its horizontal competitor. The shaded background indicates the density $1/y$ in the upper half-plane. The minimizer has Euclidean length $\pi/\sqrt2$ but weighted cost $2\ln(1+\sqrt2)$, smaller than the straight path's cost two.

## 10

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10/solution">Solution</h3>

↑ **Parent:** [10](#10)

**Self-adjoint form.** Grouping the two derivative terms gives $[(1+\epsilon x)u']'-\epsilon u=-\lambda u$. Thus a regular [Sturm-Liouville operator](../../sturm-liouville-theory.md#sturm-liouville-operator) is

$$
\boxed{\mathcal L=-\frac d{dx}\left[(1+\epsilon x)\frac d{dx}\right]+\epsilon,
\qquad p=1+\epsilon x,\quad q=\epsilon,\quad w=1.}
$$

The [boundary conditions](../../differential-equation.md#boundary-condition) are mixed [Neumann boundary conditions](../../differential-equation.md#neumann-boundary-condition) at zero and [Dirichlet boundary conditions](../../differential-equation.md#dirichlet-boundary-condition) at $\pi$. For $\epsilon\geq0$, $p>0$, $q\geq0$ and $w>0$, as required. The boundary term $[p(fg'-f'g)]_0^\pi$ vanishes for two functions satisfying these conditions, confirming self-adjointness on that domain.

**Constrained variation.** Introduce a [Lagrange multiplier](../../mathematical-optimization.md#lagrange-multiplier) $\Lambda$ for the normalization and vary

$$
I[v]-\Lambda\left(\int_0^\pi wv^2\,dx-1\right).
$$

Its first variation is

$$
2[pv'\delta v]_0^\pi+2\int_0^\pi[-(pv')'+qv-\Lambda wv]\delta v\,dx.
$$

The endpoint term vanishes because $v'(0)=0$ and $\delta v(\pi)=0$. The [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation) is therefore

$$
-(pv')'+qv=\Lambda wv,
$$

which is exactly the original [eigenvalue](../../linear-operator-theory.md#eigenvalue) problem for the boxed choices of $p,q,w$. Multiply by $v$ and integrate by parts. The same endpoint conditions give

$$
I[v]=\int_0^\pi(pv'^2+qv^2)\,dx=\Lambda\int_0^\pi wv^2\,dx=\Lambda.
$$

Thus **the stationary functional values are the [eigenvalues](../../linear-operator-theory.md#eigenvalue)**, with $\Lambda=\lambda$. More generally, before normalization the relevant [Rayleigh quotient](../../linear-operator-theory.md#rayleigh-quotient) is

$$
\mathcal R_\epsilon[v]=\frac{\int_0^\pi[(1+\epsilon x)v'^2+\epsilon v^2]dx}{\int_0^\pi v^2dx}.
$$

**Unperturbed ground mode.** At $\epsilon=0$, the equation is $-u''=\lambda u$. The quadratic form is nonnegative, and zero [eigenvalue](../../linear-operator-theory.md#eigenvalue) would force a constant function incompatible with the endpoint at $\pi$. For positive $\lambda$, $u=A\cos(\sqrt\lambda x)+B\sin(\sqrt\lambda x)$. The derivative condition forces $B=0$, while the other endpoint gives $\cos(\pi\sqrt\lambda)=0$. Hence

$$
\lambda_n=(n+1/2)^2,\qquad n=0,1,2,\ldots.
$$

The lowest [eigenvalue](../../linear-operator-theory.md#eigenvalue) and normalized [eigenfunction](../../linear-operator-theory.md#eigenfunction) are

$$
\boxed{\lambda_0=\frac14,\qquad U_0(x)=\sqrt{\frac2\pi}\cos\frac x2,\qquad
\int_0^\pi U_0^2dx=1.}
$$

**Trial-function bound.** The [Rayleigh-Ritz method](../../finite-element-method.md#rayleigh-ritz-method) says that the minimum [eigenvalue](../../linear-operator-theory.md#eigenvalue) is no larger than the quotient of any admissible trial function. The same $U_0$ still satisfies both [boundary conditions](../../differential-equation.md#boundary-condition) and retains unit norm. Its derivative is $U_0'=-\sqrt{2/\pi}\sin(x/2)/2$, giving

$$
\mathcal R_\epsilon[U_0]=\frac14+\epsilon\left[1+\frac1{2\pi}\int_0^\pi x\sin^2\frac x2\,dx\right].
$$

Using $\sin^2(x/2)=(1-\cos x)/2$,

$$
\int_0^\pi x\sin^2\frac x2\,dx=\frac{\pi^2}{4}+1.
$$

Therefore the [affine-parameter Sturm-Liouville eigenvalue bound](../../finite-element-method.md#affine-parameter-sturm-liouville-eigenvalue-bound) is

$$
\boxed{\lambda_{\min}(\epsilon)\leq\frac14+\epsilon\left(1+\frac\pi8+\frac1{2\pi}\right)
\simeq\frac14+1.551854\epsilon.}
$$

This is an upper bound for every $\epsilon\geq0$, not merely a small-parameter approximation. As a lower-bound check, $p\geq1$ and the unperturbed variational minimum imply $\mathcal R_\epsilon[v]\geq1/4+\epsilon$ for every admissible normalized $v$. Thus

$$
\boxed{\frac14+\epsilon\leq\lambda_{\min}(\epsilon)\leq\frac14+\left(1+\frac\pi8+\frac1{2\pi}\right)\epsilon.}
$$

## ↑ Ancestors (10)

1. [2017](../2017.md)
2. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
3. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
4. [Year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
