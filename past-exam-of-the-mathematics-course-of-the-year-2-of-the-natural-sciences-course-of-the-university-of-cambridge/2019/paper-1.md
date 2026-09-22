# Paper 1

↑ **Parent:** [2019](../2019.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2019/papernst_ib_1_2019.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2019/papernst_ib_1_2019.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
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
    - [i](#3/d/i)
      - [Solution](#3/d/i/solution)
    - [ii](#3/d/ii)
      - [Solution](#3/d/ii/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)
  - [d](#6/d)
    - [Solution](#6/d/solution)
- [7](#7)
  - [a](#7/a)
    - [Solution](#7/a/solution)
  - [b](#7/b)
    - [Solution](#7/b/solution)
  - [c](#7/c)
    - [Solution](#7/c/solution)
  - [d](#7/d)
    - [i](#7/d/i)
      - [Solution](#7/d/i/solution)
    - [ii](#7/d/ii)
      - [Solution](#7/d/ii/solution)
  - [e](#7/e)
    - [Solution](#7/e/solution)
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
    - [i](#9/b/i)
      - [Solution](#9/b/i/solution)
    - [ii](#9/b/ii)
      - [Solution](#9/b/ii/solution)
  - [c](#9/c)
    - [Solution](#9/c/solution)
- [10](#10)
  - [a](#10/a)
    - [Solution](#10/a/solution)
  - [b](#10/b)
    - [Solution](#10/b/solution)
  - [c](#10/c)
    - [Solution](#10/c/solution)
  - [d](#10/d)
    - [Solution](#10/d/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use the [Levi-Civita symbol](../../multivariable-calculus.md#levi-civita-symbol) and the [contraction of two Levi-Civita symbols](../../multivariable-calculus.md#contraction-of-two-levi-civita-symbols) in [Cartesian coordinates](../../linear-algebra.md#cartesian-coordinate-system). With repeated indices summed,

$$
\begin{aligned}
[\nabla\times(\mathbf A\times\mathbf B)]_i
&=\epsilon_{ijk}\epsilon_{klm}\partial_j(A_lB_m)\\
&=(\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl})\partial_j(A_lB_m)\\
&=\partial_j(A_iB_j)-\partial_j(A_jB_i)\\
&=B_j\partial_jA_i+A_i\partial_jB_j-B_i\partial_jA_j-A_j\partial_jB_i.
\end{aligned}
$$

The last line is the [product rule](../../calculus.md#product-rule). Reading its four terms in vector notation proves the [curl of a cross product](../../multivariable-calculus.md#curl-of-a-cross-product) identity:

$$
\boxed{\nabla\times(\mathbf A\times\mathbf B)=(\mathbf B\cdot\nabla)\mathbf A-\mathbf B(\nabla\cdot\mathbf A)-(\mathbf A\cdot\nabla)\mathbf B+\mathbf A(\nabla\cdot\mathbf B).}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For an oriented piecewise smooth surface $S$ with boundary curve $C=\partial S$, and a continuously differentiable vector field $\mathbf F$ near $S$, [Stokes theorem](../../multivariable-calculus.md#stokes-theorem) states

$$
\boxed{\int_S(\nabla\times\mathbf F)\cdot\mathbf n\,dS=\oint_C\mathbf F\cdot d\mathbf r.}
$$

Here $\mathbf n$ is the chosen [unit normal](../../differential-geometry.md#unit-normal), $dS$ is positive surface area, and $d\mathbf r$ is the directed tangent [line element](../../riemannian-metric.md#line-element). The positive traversal of $C$ is fixed by the right-hand rule relative to $\mathbf n$. Thus the [flux](../../mathematical-physics.md#flux) of the [curl](../../multivariable-calculus.md#curl) through the surface equals the circulation along its oriented boundary.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Differentiate the position vector, keeping the other coordinates fixed in each [derivative](../../calculus.md#derivative):

$$
\boxed{\mathbf h_u=(a\sinh u\cos v,a\cosh u\sin v,0),\quad\mathbf h_v=(-a\cosh u\sin v,a\sinh u\cos v,0),\quad\mathbf h_z=(0,0,1).}
$$

The first two have zero [dot product](../../inner-product.md#dot-product), since their two planar contributions cancel, and both are orthogonal to $\mathbf h_z$. Hence these are [orthogonal coordinates](../../multivariable-calculus.md#orthogonal-coordinates) away from coordinate degeneracies. Their scale factors, which are the lengths of these coordinate basis vectors, are

$$
\boxed{h_u=h_v=a\sqrt{\sinh^2u+\sin^2v},\qquad h_z=1.}
$$

For example $|\mathbf h_u|^2=a^2[\sinh^2u\cos^2v+\cosh^2u\sin^2v]=a^2(\sinh^2u+\sin^2v)$. The unit basis vectors are $\mathbf h_i/h_i$ when $h_i\ne0$; the given coordinate basis vectors themselves are not normalized. The [Jacobian determinant](../../multivariable-calculus.md#jacobian-determinant) is $a^2(\sinh^2u+\sin^2v)>0$ except on the focal lines. These are [elliptic cylindrical coordinates](../../multivariable-calculus.md#elliptic-cylindrical-coordinates).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For $u>0$, eliminating $v$ gives

$$
\boxed{\frac{x^2}{a^2\cosh^2u}+\frac{y^2}{a^2\sinh^2u}=1.}
$$

Thus constant $u$ surfaces are confocal [elliptic cylinders](../../euclidean-geometry.md#elliptic-cylinder) parallel to the $z$ axis. The limiting $u=0$ surface is the vertical strip $y=0$, $|x|\leq a$.

For generic $v$, eliminating $u$ gives

$$
\boxed{\frac{x^2}{a^2\cos^2v}-\frac{y^2}{a^2\sin^2v}=1.}
$$

These are [hyperbolic cylinders](../../euclidean-geometry.md#hyperbolic-cylinder) with the same focal lines. A specified angular value selects the half-branch with $\operatorname{sgn}x=\operatorname{sgn}(\cos v)$ and $\operatorname{sgn}y=\operatorname{sgn}(\sin v)$, because $u\geq0$. At $v=0,\pi$ the surfaces are the vertical half-planes $y=0$, $x\geq a$ or $x\leq-a$; at $v=\pi/2,3\pi/2$ they are $x=0$, $y\geq0$ or $y\leq0$.

Finally, constant $z$ gives horizontal planes. The three surface families express the [orthogonality](../../inner-product.md#orthogonal-vectors) of [elliptic cylindrical coordinates](../../multivariable-calculus.md#elliptic-cylindrical-coordinates).

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

The ellipse bounding the surface is $u=1$. With the upward normal, its positively oriented boundary is traversed by increasing $v$ from zero to $2\pi$:

$$
\mathbf r(v)=(a\cosh1\cos v,a\sinh1\sin v,c),\qquad d\mathbf r=(-a\cosh1\sin v,a\sinh1\cos v,0)dv.
$$

The given components are Cartesian components, so their ordinary [dot product](../../inner-product.md#dot-product) with this tangent is

$$
\mathbf F\cdot d\mathbf r=-2a\sinh1\cosh1(\sin^2v+\cos^2v)dv.
$$

Therefore [Stokes theorem](../../multivariable-calculus.md#stokes-theorem) gives

$$
\boxed{\int_S(\nabla\times\mathbf F)\cdot d\mathbf S=-4\pi a\sinh1\cosh1=-2\pi a\sinh2.}
$$

A direct check uses $F_x=2y/a$ and $F_y=-2x/a$, hence $(\nabla\times\mathbf F)_z=-4/a$, and multiplies by the ellipse area $\pi a^2\sinh1\cosh1$. The third component cannot affect either calculation because the surface and its boundary lie at fixed $z$. Equivalently one may apply Stokes to the smooth planar field $(2y/a,-2x/a,0)$, avoiding any need to differentiate the elliptic-coordinate expression for the third component at its foci.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Write a nonzero separated solution as $T=X(x)Y(y)S(t)$. Division of the [heat equation](../../diffusion-equation.md#heat-equation) by this product gives

$$
\frac{S'}{\lambda S}=\frac{X''}{X}+\frac{Y''}{Y}.
$$

The two spatial factors solve independent constant-coefficient [eigenvalue](../../linear-operator-theory.md#eigenvalue) problems. Zero endpoint values in $x$ require

$$
X_n(x)=\sin(n\pi x/a),\qquad X_n''=-(n\pi/a)^2X_n,\quad n=1,2,\ldots.
$$

The insulating conditions require

$$
Y_m(y)=\cos(m\pi y/b),\qquad Y_m''=-(m\pi/b)^2Y_m,\quad m=0,1,2,\ldots.
$$

The zero cosine mode is the nonzero constant function and must be retained; there is no nonzero zero-index sine mode. The temporal equation is $S'=-\lambda\pi^2(n^2/a^2+m^2/b^2)S$. Superposing the complete sine-cosine basis yields

$$
\boxed{T(x,y,t)=\sum_{n=1}^\infty\sum_{m=0}^\infty A_{nm}\sin\frac{n\pi x}{a}\cos\frac{m\pi y}{b}\exp\left[-\lambda\pi^2\left(\frac{n^2}{a^2}+\frac{m^2}{b^2}\right)t\right].}
$$

The constants are fixed by expansion of the initial profile. [Orthogonality](../../inner-product.md#orthogonal-vectors) gives sine norm $a/2$; the cosine norm is $b$ at $m=0$ and $b/2$ otherwise. This is the [heat equation on a rectangle with two insulated sides](../../diffusion-equation.md#heat-equation-on-a-rectangle-with-two-insulated-sides).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

First decompose the initial $y$ dependence using $\sin^2(2\pi y/b)=[1-\cos(4\pi y/b)]/2$. Only the cosine indices $m=0$ and $m=4$ occur. Expand the remaining factor in a [Fourier sine series](../../fourier-series.md#fourier-sine-series):

$$
x(a-x)=\sum_{n=1}^\infty b_n\sin\frac{n\pi x}{a},\qquad b_n=\frac2a\int_0^ax(a-x)\sin\frac{n\pi x}{a}\,dx.
$$

For $k_n=n\pi/a$, two [integrations by parts](../../calculus.md#integration-by-parts) give

$$
\int_0^ax(a-x)\sin(k_nx)dx=\frac{2[1-(-1)^n]}{k_n^3},\qquad b_n=\frac{4a^2[1-(-1)^n]}{n^3\pi^3}.
$$

Thus even $n$ vanish, while $b_n=8a^2/(n^3\pi^3)$ for odd $n$. The nonzero double-series coefficients are $A_{n0}=b_n/2$ and $A_{n4}=-b_n/2$. Their separate heat-mode decay factors give

$$
\boxed{T(x,y,t)=\frac{4a^2}{\pi^3}\sum_{\substack{n\geq1\\n\text{ odd}}}\frac{\sin(n\pi x/a)}{n^3}e^{-\lambda\pi^2n^2t/a^2}\left[1-e^{-16\lambda\pi^2t/b^2}\cos\frac{4\pi y}{b}\right].}
$$

At $t=0$ the bracket is $2\sin^2(2\pi y/b)$, which recovers the initial profile with the displayed sine coefficients. Each term satisfies the mixed [Dirichlet boundary conditions](../../differential-equation.md#dirichlet-boundary-condition) and [Neumann boundary conditions](../../differential-equation.md#neumann-boundary-condition).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The slowest surviving mode has $n=1,m=0$. Hence

$$
\boxed{T(x,y,t)\sim\frac{4a^2}{\pi^3}\sin\frac{\pi x}{a}\,e^{-\lambda\pi^2t/a^2}\qquad(t\to\infty).}
$$

It is independent of $y$: insulation allows the constant transverse mode, while every nonconstant transverse mode decays faster. The next possible relative decay rates are $8\lambda\pi^2/a^2$ from $n=3,m=0$ and $16\lambda\pi^2/b^2$ from $n=1,m=4$.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For each source point $z$, construct the [Green function](../../green-s-function.md) from homogeneous solutions on either side:

$$
G(x,z)=\begin{cases}A(z)y_a(x),&a\leq x<z,\\B(z)y_b(x),&z<x\leq b.\end{cases}
$$

The endpoint conditions are then automatic. The equation $L_xG=\delta(x-z)$ requires continuity of $G$ and a unit jump in its first [derivative](../../calculus.md#derivative): a discontinuity in $G$ would introduce an unwanted delta [derivative](../../calculus.md#derivative), while integrating across the source fixes $G_x(z^+,z)-G_x(z^-,z)=1$. Thus

$$
A y_a(z)=B y_b(z),\qquad B y_b'(z)-A y_a'(z)=1.
$$

Solving this two-by-two system, with the [Wronskian](../../linear-ordinary-differential-equation.md#wronskian) $W=y_a y_b'-y_b y_a'\ne0$, gives

$$
\boxed{G(x,z)=\begin{cases}y_a(x)y_b(z)/W(z),&a\leq x\leq z,\\y_b(x)y_a(z)/W(z),&z\leq x\leq b.\end{cases}}
$$

This derivation also remains valid if one of the solution values at the matching point vanishes: only the [Wronskian](../../linear-ordinary-differential-equation.md#wronskian) must be nonzero. For a regular nonsingular two-point problem it supplies the inverse kernel; at a singular endpoint, uniqueness requires separate checking, as part (d) illustrates.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [Green-function representation](../../green-s-function.md#green-function-representation) is

$$
\boxed{y_p(x)=\int_a^bG(x,z)f(z)\,dz.}
$$

The delta identity gives $Ly_p=f$ and the endpoint conditions follow from those of $G$. If a nonzero homogeneous solution also satisfies both endpoint conditions, it may be added; uniqueness is not automatic in that case.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For the [Euler-Cauchy equation](../../linear-ordinary-differential-equation.md#euler-cauchy-equation), substitute $y=x^n$ on an interval not containing zero. The coefficient of $x^{n-2}$ is

$$
n(n-1)-3n+3=n^2-4n+3=(n-1)(n-3).
$$

The distinct roots give

$$
\boxed{y(x)=C_1x+C_2x^3.}
$$

These solutions are linearly independent since their [Wronskian](../../linear-ordinary-differential-equation.md#wronskian) is $2x^3\ne0$ away from zero. Both nevertheless approach zero as $x\to0$, which will make the endpoint conditions in the next part insufficient for uniqueness.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/i">i</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/i/solution">Solution</h5>

↑ **Parent:** [I](#3/d/i)

Choose $y_a=x$ and $y_b=x^3-x$, satisfying the left and right conditions respectively. Their [Wronskian](../../linear-ordinary-differential-equation.md#wronskian) is

$$
W(x)=x(3x^2-1)-(x^3-x)=2x^3.
$$

Part (a) therefore supplies the valid kernel

$$
\boxed{G_0(x,z)=\begin{cases}\dfrac{x(z^3-z)}{2z^3},&0\leq x\leq z,\\[4pt]\dfrac{x^3-x}{2z^2},&z\leq x\leq1,\end{cases}\qquad0<z<1.}
$$

It is continuous at the source, its first [derivative](../../calculus.md#derivative) has jump one, and it vanishes at both endpoints. However, it is not unique: $x^3-x$ is a nonzero homogeneous solution satisfying both stated endpoint conditions. Thus $G_0+(x^3-x)h(z)$ has the same defining properties for any suitable $h$.

This is a [nonunique Green kernel at a singular endpoint with two vanishing modes](../../green-s-function.md#nonunique-green-kernel-at-a-singular-endpoint-with-two-vanishing-modes). Choosing $y_a=x^3$ instead also gives a valid kernel, corresponding to the stronger selection $y(x)/x\to0$ at the left endpoint. The original problem states no such selection, so the family must be acknowledged.

<h4 id="3/d/ii">ii</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/d/ii)

The original PDF shows $x^2$ in the nonzero source branch. Inserting that source into $G_0$ gives, for $x<1/2$,

$$
y_p(x)=\frac x2\int_{1/2}^1(z^2-1)\,dz=-\frac{5x}{48}.
$$

For $x\geq1/2$, split the integral at $z=x$:

$$
\begin{aligned}
y_p(x)&=\frac{x^3-x}{2}\int_{1/2}^x1\,dz+\frac x2\int_x^1(z^2-1)\,dz\\
&=\frac{x^4}{3}-\frac{x^3}{4}-\frac{x}{12}.
\end{aligned}
$$

Because of the homogeneous freedom established in part (i), the full answer to the stated endpoint problem is

$$
\boxed{y(x)=\begin{cases}-5x/48,&0\leq x<1/2,\\x^4/3-x^3/4-x/12,&1/2\leq x\leq1,\end{cases}+C(x^3-x),\qquad C\in\mathbb R.}
$$

At the interface, both branches have value $-5/96$ and [derivative](../../calculus.md#derivative) $-5/48$, so no extra delta or delta [derivative](../../calculus.md#derivative) occurs there. Direct substitution gives zero source on the left and $x^2$ on the right; the endpoint values are zero for every $C$. If the extra condition $y/x\to0$ is imposed, it selects $C=-5/48$, but that is additional information absent from the printed question.

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For the stated [Fourier transform](../../fourier-transform.md) convention, [Fourier inversion](../../fourier-analysis.md#fourier-inversion-theorem) is

$$
\boxed{f(x)=\frac1{2\pi}\int_{-\infty}^{\infty}\widetilde f(k)e^{ikx}\,dk.}
$$

For example, the pointwise formula holds at continuity points under the usual integrability hypotheses; the same normalization applies to the $L^2$ or distributional inverse.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Assume initially that $f,g$ are integrable, so [Fubini's theorem](../../measure-theory.md#fubini-s-theorem) justifies interchanging the integrals. Transform the [convolution](../../fourier-analysis.md#convolution) and put $u=x-z$:

$$
\begin{aligned}
\widetilde h(k)&=\int_{\mathbb R}\!\int_{\mathbb R}f(z)g(x-z)e^{-ikx}\,dz\,dx\\
&=\int_{\mathbb R}f(z)e^{-ikz}\,dz\int_{\mathbb R}g(u)e^{-iku}\,du\\
&=\boxed{\widetilde f(k)\widetilde g(k)}.
\end{aligned}
$$

This is the [convolution theorem](../../fourier-analysis.md#convolution-theorem). No factor $2\pi$ appears in this direction because the forward transform in the question is unnormalized.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Differentiate the defining Fourier integral $n$ times with respect to $k$:

$$
\frac{d^n\widetilde f}{dk^n}=\int_{\mathbb R}(-ix)^nf(x)e^{-ikx}\,dx.
$$

For a nonnegative integer $n$, this gives

$$
\boxed{\mathcal F[x^nf(x)](k)=i^n\frac{d^n\widetilde f(k)}{dk^n}.}
$$

Integrability of $x^nf$ together with suitable lower moments justifies differentiation under the integral. The same multiplication-derivative identity holds more generally for [tempered distributions](../../fourier-analysis.md#tempered-distribution).

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Evenness means the negative half of the function is determined as well: this is the [triangular function](../../fourier-analysis.md#triangular-function) $q(x)=1-|x|$ on $|x|\leq1$, zero outside. Its transform is real and even:

$$
\widetilde q(k)=2\int_0^1(1-x)\cos(kx)\,dx.
$$

[Integration by parts](../../calculus.md#integration-by-parts), or integrating the two terms separately, gives

$$
\boxed{\widetilde q(k)=\frac{2(1-\cos k)}{k^2}=\left(\frac{\sin(k/2)}{k/2}\right)^2,\qquad\widetilde q(0)=1.}
$$

The apparent singularity at zero is removable, and its limiting value is the area under $q$. This is the [Fourier transform of a triangular function](../../fourier-analysis.md#fourier-transform-of-a-triangular-function).

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Let $r(z)$ be the indicator of $[-1,1]$. The finite integral is exactly the [convolution](../../fourier-analysis.md#convolution) $p=q*r$. Its additional transform factor is

$$
\widetilde r(k)=\int_{-1}^1e^{-ikz}\,dz=\frac{2\sin k}{k},\qquad\widetilde r(0)=2.
$$

Applying the [convolution theorem](../../fourier-analysis.md#convolution-theorem) and part (d),

$$
\boxed{\widetilde p(k)=\frac{4\sin k(1-\cos k)}{k^3},\qquad\widetilde p(0)=2.}
$$

Equivalently this is $2(\sin k/k)[\sin(k/2)/(k/2)]^2$. The value at zero also follows from $\int p=(\int q)(\int r)=1\times2$.

## 5

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The [adjoint operator](../../hilbert-space.md#adjoint-operator) $A^\dagger$, when it exists, is defined by

$$
\boxed{\langle Ax,y\rangle=\langle x,A^\dagger y\rangle}
$$

for all vectors in the relevant domains. This convention takes the [inner product](../../inner-product.md) to be conjugate-linear in its first argument. Nondegeneracy makes the adjoint unique.

For the standard complex [inner product](../../inner-product.md) $\langle x,y\rangle=\overline{x}^{\,T}y$, the equality becomes $\overline{x}^{\,T}\overline{A}^{\,T}y=\overline{x}^{\,T}A^\dagger y$ for every $x,y$, so

$$
\boxed{A^\dagger=\overline A^{\,T}.}
$$

Thus the matrix adjoint is the [Hermitian conjugate](../../hilbert-space.md#hermitian-conjugation), not merely the [transpose](../../vector-space.md#transpose) unless the entries are real. In a basis with positive Hermitian [Gram matrix](../../inner-product.md#gram-matrix) $G$, the same definition instead gives $A^\dagger_G=G^{-1}\overline A^{\,T}G$, making the dependence on the chosen [inner product](../../inner-product.md) explicit.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

An [invertible matrix](../../linear-algebra.md#invertible-matrix) is a square matrix for which there is a matrix $A^{-1}$ with $AA^{-1}=A^{-1}A=I$. Write its assumed [diagonalization](../../linear-operator-theory.md#diagonalization-of-a-matrix) as $A=P\Lambda P^{-1}$, where $P$ is invertible and $\Lambda=\operatorname{diag}(\lambda_1,\ldots,\lambda_n)$. Then

$$
\det A=\det\Lambda=\prod_{j=1}^n\lambda_j.
$$

If the [determinant](../../multilinear-algebra.md#determinant) is nonzero, every $\lambda_j$ is nonzero, so $\Lambda^{-1}=\operatorname{diag}(\lambda_j^{-1})$ exists and $A^{-1}=P\Lambda^{-1}P^{-1}$. If the [determinant](../../multilinear-algebra.md#determinant) is zero, at least one [eigenvalue](../../linear-operator-theory.md#eigenvalue) is zero; its nonzero [eigenvector](../../linear-operator-theory.md#eigenvector) is mapped to zero, which an invertible map cannot do. Hence

$$
\boxed{A\text{ is invertible}\quad\Longleftrightarrow\quad\det A\ne0.}
$$

The equivalence holds even without diagonalizability, but the eigenbasis proves the stated case directly.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

The entries of $M^TM$ are real, and the [transpose](../../vector-space.md#transpose) rule gives $(M^TM)^T=M^TM$. Thus it is a real [symmetric matrix](../../linear-algebra.md#symmetric-matrix), hence also a [Hermitian matrix](../../hilbert-space.md#hermitian-operator).

For any complex vector $v$,

$$
v^\dagger M^TMv=(Mv)^\dagger(Mv)=\|Mv\|^2\geq0.
$$

In particular, if $M^TMv=\lambda v$ with $v\ne0$,

$$
\boxed{\lambda=\frac{\|Mv\|^2}{\|v\|^2}\geq0.}
$$

Thus $M^TM$ is [positive semidefinite](../../quadratic-form.md#positive-semidefinite-matrix). Its zero [eigenspace](../../linear-operator-theory.md#eigenspace) is precisely the kernel of $M$, since $\|Mv\|^2=0$ is equivalent to $Mv=0$. This is the Gram-matrix structure behind the nonnegative [eigenvalues](../../linear-operator-theory.md#eigenvalue).

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

For the positive integer $k$ in the nilpotence condition, diagonalize $B=P\Lambda P^{-1}$. Then

$$
0=B^k=P\operatorname{diag}(\lambda_1^k,\ldots,\lambda_n^k)P^{-1}.
$$

Every diagonal entry must vanish, so each $\lambda_j=0$. Consequently $\Lambda=0$ and $\boxed{B=0}$. This proves that [a diagonalizable nilpotent matrix is zero](../../linear-operator-theory.md#a-diagonalizable-nilpotent-matrix-is-zero).

Without diagonalizability a counterexample is

$$
\boxed{C=\begin{pmatrix}0&1\\0&0\end{pmatrix}\ne0,\qquad C^2=0.}
$$

Its only [eigenvalue](../../linear-operator-theory.md#eigenvalue) is zero but its kernel has dimension one, so it cannot have a basis of [eigenvectors](../../linear-operator-theory.md#eigenvector). It is the simplest nontrivial nilpotent [Jordan block](../../linear-operator-theory.md#jordan-block).

## 6

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

By the [spectral theorem](../../hilbert-space.md#spectral-theorem), a [Hermitian matrix](../../hilbert-space.md#hermitian-operator) has real [eigenvalues](../../linear-operator-theory.md#eigenvalue) and an orthonormal eigenbasis. Choose column vectors $u_j$ with $Hu_j=\lambda_ju_j$ and $u_i^\dagger u_j=\delta_{ij}$, and form $U=(u_1\ \cdots\ u_n)$. Then $U^\dagger U=I$, so $U$ is unitary, and $HU=U\Lambda$ gives

$$
\boxed{U^\dagger HU=\Lambda=\operatorname{diag}(\lambda_1,\ldots,\lambda_n).}
$$

The entries of $\Lambda$ are the real [eigenvalues](../../linear-operator-theory.md#eigenvalue), repeated according to their multiplicities. Within a degenerate [eigenspace](../../linear-operator-theory.md#eigenspace), any [orthonormal basis](../../inner-product.md#orthonormal-basis) may be used. Equivalently $H=U\Lambda U^\dagger$.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

A real [symmetric matrix](../../linear-algebra.md#symmetric-matrix) has a real orthonormal eigenbasis. Put those [eigenvectors](../../linear-operator-theory.md#eigenvector) into an [orthogonal matrix](../../linear-algebra.md#orthogonal-matrix) $Q$, so $Q^TAQ=\operatorname{diag}(a_1,\ldots,a_n)$. With the change of coordinates $x=Qx'$, or $x'=Q^Tx$,

$$
\boxed{\sum_{ij}A_{ij}x_ix_j=x^TAx=x'^T(Q^TAQ)x'=\sum_i a_i(x_i')^2.}
$$

Thus the coefficients are the [eigenvalues](../../linear-operator-theory.md#eigenvalue) and the new coordinate directions are the [eigenvectors](../../linear-operator-theory.md#eigenvector). This [orthogonal diagonalization](../../linear-algebra.md#orthogonal-diagonalization-of-a-real-symmetric-matrix) preserves Euclidean lengths and angles while removing cross terms from the [quadratic form](../../quadratic-form.md).

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

The second coordinate direction is already an [eigenvector](../../linear-operator-theory.md#eigenvector) with [eigenvalue](../../linear-operator-theory.md#eigenvalue) three. The first and third coordinates form a symmetric block, whose sum and difference directions give

$$
\boxed{\begin{array}{c|c}
\text{eigenvalue}&\text{unit eigenvector}\\\hline
6&(1,0,1)^T/\sqrt2\\
3&(0,1,0)^T\\
2c-4&(1,0,-1)^T/\sqrt2
\end{array}.}
$$

For example, the sum of the block's diagonal and off-diagonal entries is $(1+c)+(5-c)=6$, while their difference is $(1+c)-(5-c)=2c-4$. Equivalently the characteristic polynomial is $(\lambda-6)(\lambda-3)(\lambda-2c+4)$.

The displayed basis works for every real $c$. At $c=7/2$, the [eigenvalue](../../linear-operator-theory.md#eigenvalue) three has [eigenspace](../../linear-operator-theory.md#eigenspace) spanned by the second and third listed vectors; at $c=5$, the [eigenvalue](../../linear-operator-theory.md#eigenvalue) six has [eigenspace](../../linear-operator-theory.md#eigenspace) spanned by the first and third. Every nonzero vector in a repeated [eigenspace](../../linear-operator-theory.md#eigenspace) is an [eigenvector](../../linear-operator-theory.md#eigenvector), and any [orthonormal basis](../../inner-product.md#orthonormal-basis) of it may replace the displayed choices.

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

Use the principal coordinates

$$
p=\frac{x_1+x_3}{\sqrt2},\qquad q=x_2,\qquad r=\frac{x_1-x_3}{\sqrt2}.
$$

Part (c) puts the equation in the canonical form

$$
\boxed{6p^2+3q^2+(2c-4)r^2=1.}
$$

If $c>2$, all three coefficients are positive: the surface is an [ellipsoid](../../euclidean-geometry.md#ellipsoid) with semiaxes $1/\sqrt6$, $1/\sqrt3$ and $1/\sqrt{2c-4}$ along the three [eigenvectors](../../linear-operator-theory.md#eigenvector) listed in part (c).

If $c=2$, the equation is independent of $r$: it is an [elliptic cylinder](../../euclidean-geometry.md#elliptic-cylinder) parallel to $(1,0,-1)$, with cross-sectional semiaxes $1/\sqrt6$ and $1/\sqrt3$.

If $c<2$, the form has two positive coefficients and one negative coefficient: it is a [one-sheet hyperboloid](../../differential-geometry.md#one-sheet-hyperboloid), with axis $(1,0,-1)$ and waist ellipse $6p^2+3q^2=1$ at $r=0$. Its axial scale is $1/\sqrt{4-2c}$.

These are the three cases of the [signature transition from an ellipsoid to an elliptic cylinder and a one-sheet hyperboloid](../../euclidean-geometry.md#signature-transition-from-an-ellipsoid-to-an-elliptic-cylinder-and-a-one-sheet-hyperboloid). At the repeated [eigenvalues](../../linear-operator-theory.md#eigenvalue) $c=7/2$ and $c=5$, [principal axes](../../rigid-body-dynamics.md#principal-axis) in the corresponding two-dimensional [eigenspace](../../linear-operator-theory.md#eigenspace) are not unique: the [ellipsoid](../../euclidean-geometry.md#ellipsoid) is respectively an [oblate spheroid](../../galaxy.md#oblate-spheroid) about the $p$ axis or a [prolate spheroid](../../euclidean-geometry.md#prolate-spheroid) about the $q$ axis.

## 7

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

For $f=u+iv$ analytic in $z=x+iy$, the [Cauchy-Riemann equations](../../analysis.md#cauchy-riemann-equations) are

$$
\boxed{u_x=v_y,\qquad u_y=-v_x.}
$$

They follow by computing the same complex [derivative](../../calculus.md#derivative) along the real and imaginary coordinate directions.

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/solution">Solution</h4>

↑ **Parent:** [B](#7/b)

The [Cauchy-Riemann equations](../../analysis.md#cauchy-riemann-equations) give

$$
\nabla u\cdot\nabla v=u_xv_x+u_yv_y=u_x(-u_y)+u_yu_x=0.
$$

At a regular point, each level curve has tangent perpendicular to its nonzero [gradient](../../multivariable-calculus.md#gradient). The two [gradients](../../multivariable-calculus.md#gradient), and hence the two tangents, are orthogonal. Therefore **regular level curves meet at right angles**.

The qualification is necessary: $|\nabla u|=|\nabla v|=|f'(z)|$, so at a critical point both [gradients](../../multivariable-calculus.md#gradient) vanish and this argument gives no tangent direction. For example, for $f(z)=z^2$, the zero level curves of the real and imaginary parts are diagonals and coordinate axes; they meet at $45^\circ$ at zero. This is the regular-point statement of [orthogonal level curves of harmonic conjugates](../../partial-differential-equation.md#orthogonal-level-curves-of-harmonic-conjugates).

<h3 id="7/c">c</h3>

↑ **Parent:** [7](#7)

<h4 id="7/c/solution">Solution</h4>

↑ **Parent:** [C](#7/c)

Recognize that $z^2=(x^2-y^2)+2ixy$ and $e^{-z}=e^{-x}(\cos y-i\sin y)$. Their product has exactly the specified real part. Its imaginary part is

$$
v_0=e^{-x}[2xy\cos y-(x^2-y^2)\sin y].
$$

One can also recover it directly from the [Cauchy-Riemann equations](../../analysis.md#cauchy-riemann-equations). Differentiating the specified real part gives

$$
u_x=e^{-x}[(2x-x^2+y^2)\cos y+2y(1-x)\sin y].
$$

Integration of $v_y=u_x$ gives $v=v_0+h(x)$; the other equation $v_x=-u_y$ then forces $h'(x)=0$. Thus the most general answer on a connected domain is

$$
\boxed{f(z)=z^2e^{-z}+iC,\qquad C\in\mathbb R.}
$$

Indeed the difference of any two [analytic functions](../../holomorphic-function.md) with the same real part has zero real part; its two [Cauchy-Riemann equations](../../analysis.md#cauchy-riemann-equations) force its imaginary part to be constant. This proves that no further analytic freedom is missing.

<h3 id="7/d">d</h3>

↑ **Parent:** [7](#7)

<h4 id="7/d/i">i</h4>

↑ **Parent:** [D](#7/d)

<h5 id="7/d/i/solution">Solution</h5>

↑ **Parent:** [I](#7/d/i)

The denominator factors as $z^2+iz+6=(z-2i)(z+3i)$, with no cancellation against the numerator. Thus there are

$$
\boxed{\text{simple poles at }z=2i,-3i;\qquad\text{a simple zero at }z=4.}
$$

To inspect infinity, put $w=1/z$:

$$
f(1/w)=\frac{w-4w^2}{1+iw+6w^2}=w+O(w^2).
$$

Hence infinity is a [removable singularity at infinity](../../isolated-singularity.md#removable-singularity-at-infinity), with limiting value zero. After this natural extension to the [Riemann sphere](../../riemann-surfaces.md#riemann-sphere) it is also a **simple zero**. There are no other zeros or singularities.

<h4 id="7/d/ii">ii</h4>

↑ **Parent:** [D](#7/d)

<h5 id="7/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7/d/ii)

The [complex exponential](../../calculus.md#complex-exponential-function) never vanishes. The zeros of $\sinh z$ occur at $z=n\pi i$, $n\in\mathbb Z$, and they are simple because $\cosh(n\pi i)=(-1)^n\ne0$. The numerator is $e^{2n\pi i}=1$ there, so no cancellation occurs. Therefore

$$
\boxed{\text{simple poles at }z=n\pi i\ (n\in\mathbb Z);\qquad\text{no finite zeros}.}
$$

For example their residues are $1/\cosh(n\pi i)=(-1)^n$.

Infinity requires care: the [poles](../../isolated-singularity.md#pole) themselves tend to infinity. Equivalently $f(1/w)$ has [poles](../../isolated-singularity.md#pole) at $w=1/(n\pi i)$ accumulating at zero. Thus $\boxed{\infty\text{ is a non-isolated singularity}}$, and it is not a zero. In the usual classification of isolated singularities, it cannot be called a [removable singularity](../../isolated-singularity.md#removable-singularity), [pole](../../isolated-singularity.md#pole) or isolated essential singularity. The [non-isolated singularity](../../isolated-singularity.md#non-isolated-singularity) distinction is necessary even though the function is meromorphic at every finite point.

<h3 id="7/e">e</h3>

↑ **Parent:** [7](#7)

<h4 id="7/e/solution">Solution</h4>

↑ **Parent:** [E](#7/e)

Put $\zeta=z-3$ and apply the [geometric series](../../sequence-and-series.md#geometric-series):

$$
\frac1{z-2i}=\frac1{3-2i}\frac1{1+\zeta/(3-2i)}=\sum_{n=0}^\infty\frac{(-1)^n}{(3-2i)^{n+1}}(z-3)^n.
$$

Thus

$$
\boxed{a_n=\frac{(-1)^n}{(3-2i)^{n+1}},\qquad |z-3|<\sqrt{13},\qquad R=\sqrt{13}.}
$$

The radius is the distance from the expansion centre $3$ to the nearest singularity $2i$, not the distance of that [pole](../../isolated-singularity.md#pole) from the origin. On the boundary circle the series terms all have magnitude $1/\sqrt{13}$, so they do not approach zero: this particular series diverges at every boundary point.

## 8

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8/a">a</h3>

↑ **Parent:** [8](#8)

<h4 id="8/a/solution">Solution</h4>

↑ **Parent:** [A](#8/a)

For the normalized equation, $x_0$ is an [ordinary point](../../complex-analysis.md#ordinary-point-criterion-for-a-second-order-equation) when both $p$ and $q$ are analytic near $x_0$. A singular point is a [regular singular point](../../complex-analysis.md#regular-singular-point) when $(x-x_0)p(x)$ and $(x-x_0)^2q(x)$ extend analytically to $x_0$; equivalently $p$ has at most a [simple pole](../../isolated-singularity.md#simple-pole) and $q$ at most a double [pole](../../isolated-singularity.md#pole) there.

Thus ordinary points admit ordinary power-series solutions, while the [Frobenius method](../../complex-analysis.md#frobenius-method) applies at a regular singular point. The definitions refer to the coefficients after dividing by the leading coefficient of $y''$.

<h3 id="8/b">b</h3>

↑ **Parent:** [8](#8)

<h4 id="8/b/solution">Solution</h4>

↑ **Parent:** [B](#8/b)

After normalization, $p=-6x^2/(1-x^3)$ and $q=-6x/(1-x^3)$. Both are analytic at zero, so $\boxed{x=0\text{ is ordinary}}$. At one,

$$
(x-1)p=\frac{6x^2}{1+x+x^2},\qquad (x-1)^2q=\frac{6x(x-1)}{1+x+x^2}
$$

are analytic, whereas $p,q$ themselves have [poles](../../isolated-singularity.md#pole). Hence $\boxed{x=1\text{ is a regular singular point}}$.

Insert $y=\sum_{n\geq0}a_nx^n$. The coefficient of $x^0$ gives $a_2=0$; for $k\geq1$ the coefficient of $x^k$ gives

$$
(k+2)(k+1)a_{k+2}=(k+2)(k+1)a_{k-1}.
$$

Thus $a_n=a_{n-3}$ for $n\geq3$. The initial data give $a_0=1$, $a_1=0$, so

$$
\boxed{y(x)=1+x^3+x^6+\cdots=\frac1{1-x^3},\qquad |x|<1.}
$$

The radius is one because the three cube roots of unity are [poles](../../isolated-singularity.md#pole) of this solution. A direct structural check observes that the differential equation is exactly $[(1-x^3)y]''=0$. Thus $(1-x^3)y=A+Bx$, and the initial data select $A=1,B=0$. This is the [product-derivative reduction of a second-order differential equation](../../linear-ordinary-differential-equation.md#product-derivative-reduction-of-a-second-order-differential-equation).

<h3 id="8/c">c</h3>

↑ **Parent:** [8](#8)

<h4 id="8/c/solution">Solution</h4>

↑ **Parent:** [C](#8/c)

Use a [Frobenius solution](../../complex-analysis.md#frobenius-solution) $y=x^\sigma\sum_{n\geq0}a_nx^n$, with $a_0\ne0$. The lowest power $x^{\sigma-1}$ has coefficient $2\sigma(2\sigma-1)a_0$, giving the [indicial equation](../../linear-ordinary-differential-equation.md#indicial-equation)

$$
\boxed{2\sigma(2\sigma-1)=0,\qquad\sigma=0,\frac12.}
$$

For $n\geq1$, matching the coefficient of $x^{n+\sigma-1}$ gives

$$
2(n+\sigma)(2n+2\sigma-1)a_n-(2n+2\sigma-1)a_{n-1}=0.
$$

For both candidate exponents the cancelled factor is nonzero in this range, so the recurrence is

$$
\boxed{a_n=\frac{a_{n-1}}{2(n+\sigma)}.}
$$

With $a_0=1$, the exponent-zero solution is

$$
\boxed{y_1(x)=\sum_{n=0}^\infty\frac{x^n}{2^nn!}=e^{x/2}.}
$$

For $\sigma=1/2$, the coefficients are $a_n=1/(2n+1)!!=2^nn!/(2n+1)!$, giving

$$
\boxed{y_2(x)=\sqrt{x}\sum_{n=0}^\infty\frac{x^n}{(2n+1)!!}=\sqrt{x}\left(1+\frac x3+\frac{x^2}{15}+\frac{x^3}{105}+\cdots\right).}
$$

The [ratio test](../../sequence-and-series.md#ratio-test) gives infinite [radius of convergence](../../sequence-and-series.md#radius-of-convergence) for both series factors, since the successive ratios in magnitude are $|x|/(2n+2)$ and $|x|/(2n+3)$. The second full solution still needs a square-root branch in the complex plane; on $x>0$ it is a real solution. The distinct leading behaviors $1$ and $\sqrt{x}$ prove [linear independence](../../vector-space.md#linear-independence).

For an independent closed-form check on the structure, put $z=x/2$. The equation becomes $zY''+(1/2-z)Y'-(1/2)Y=0$, a [Kummer differential equation](../../linear-ordinary-differential-equation.md#kummer-differential-equation) with equal parameters. Its [exponential reduction of a confluent hypergeometric equation with equal parameters](../../linear-ordinary-differential-equation.md#exponential-reduction-of-a-confluent-hypergeometric-equation-with-equal-parameters) explains the elementary first solution and the branched companion.

## 9

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9/a">a</h3>

↑ **Parent:** [9](#9)

<h4 id="9/a/solution">Solution</h4>

↑ **Parent:** [A](#9/a)

[Fermat principle](../../mathematical-physics.md#fermat-principle) states that the [optical path length](../../physical-optics.md#optical-path-length) $\mathcal S=\int n\,ds$, or equivalently travel time $\mathcal S/c_0$, is stationary under small variations of the ray with fixed endpoints. Stationarity need not mean a global minimum.

For a plane ray written as $y(x)$, use $\mathcal S[y]=\int F(x,y,y')dx$, with $F=n(x,y)\sqrt{1+y'^2}$. Its stationary paths obey the [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation)

$$
\boxed{\frac{\partial F}{\partial y}-\frac d{dx}\left(\frac{\partial F}{\partial y'}\right)=0.}
$$

It follows by taking the [first variation](../../calculus-of-variations.md#first-variation), integrating the term in $\delta y'$ by parts, and using zero endpoint variations.

<h3 id="9/b">b</h3>

↑ **Parent:** [9](#9)

<h4 id="9/b/i">i</h4>

↑ **Parent:** [B](#9/b)

<h5 id="9/b/i/solution">Solution</h5>

↑ **Parent:** [I](#9/b/i)

Choose the mirror as the line $y=0$, the source as $(x_A,h_A)$ and the observer as $(x_B,h_B)$, with positive heights. Within the plane of incidence, let the reflection point be $(s,0)$. In a uniform medium the optical length is a constant index times

$$
\ell(s)=\sqrt{(s-x_A)^2+h_A^2}+\sqrt{(x_B-s)^2+h_B^2}.
$$

Stationarity with respect to the point on the mirror gives

$$
0=\ell'(s)=\frac{s-x_A}{\sqrt{(s-x_A)^2+h_A^2}}-\frac{x_B-s}{\sqrt{(x_B-s)^2+h_B^2}}.
$$

These two ratios are the sines of the angles to the normal, with the stationary point between the two projected endpoints. Therefore

$$
\boxed{\sin\theta_{\rm in}=\sin\theta_{\rm out},\qquad\theta_{\rm in}=\theta_{\rm out}.}
$$

The angles lie in $[0,\pi/2)$, where sine is injective. Varying a second tangential coordinate in three dimensions also enforces that the source, normal and reflected ray lie in one plane. This derives the [law of reflection](../../geometrical-optics.md#law-of-reflection) from [Fermat principle](../../mathematical-physics.md#fermat-principle).

<h4 id="9/b/ii">ii</h4>

↑ **Parent:** [B](#9/b)

<h5 id="9/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#9/b/ii)

Place the interface at $y=0$, with source $(x_A,h_1)$ and observer $(x_B,-h_2)$ in the two uniform media. Let $(s,0)$ be the crossing point. The optical length is

$$
\mathcal S(s)=\mu_1\sqrt{(s-x_A)^2+h_1^2}+\mu_2\sqrt{(x_B-s)^2+h_2^2}.
$$

Differentiating with respect to $s$ and setting the result to zero gives

$$
\mu_1\frac{s-x_A}{\sqrt{(s-x_A)^2+h_1^2}}=\mu_2\frac{x_B-s}{\sqrt{(x_B-s)^2+h_2^2}}.
$$

Recognizing the ratios as the sines of the angles measured from the interface normal proves [Snell's law](../../partial-differential-equation.md#snell-s-law):

$$
\boxed{\mu_1\sin\theta_1=\mu_2\sin\theta_2.}
$$

The stationarity condition is the continuity of the tangential optical momentum across the planar interface.

<h3 id="9/c">c</h3>

↑ **Parent:** [9](#9)

<h4 id="9/c/solution">Solution</h4>

↑ **Parent:** [C](#9/c)

The original PDF places both endpoints at height $5/4$; the vertically stacked fraction can be misread in extracted text. The coefficient in the index is $4$, multiplying $\sqrt y$.

For the optical-length integrand $F=4\sqrt y\sqrt{1+y'^2}$, the [Beltrami identity](../../analysis.md#beltrami-identity) applies because there is no explicit $x$ dependence. It gives

$$
F-y'F_{y'}=\frac{4\sqrt y}{\sqrt{1+y'^2}}=4\sqrt h,
$$

where $h>0$ is constant. Therefore $y'^2=y/h-1$. The full [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation) is $2yy''=1+y'^2$, and combining these gives $y''=1/(2h)$. This also excludes a constant curve, which would satisfy the squared first integral but not the full variational equation. Integration yields

$$
y(x)=h+\frac{(x-x_0)^2}{4h}.
$$

Equal endpoint heights at $x=-1,1$ require $x_0=0$. The height condition then becomes $h+1/(4h)=5/4$, or $4h^2-5h+1=0$. Its two positive roots are $h=1$ and $h=1/4$. Hence the two possible stationary rays are

$$
\boxed{y(x)=1+\frac{x^2}{4}\qquad\text{or}\qquad y(x)=\frac14+x^2,\qquad-1\leq x\leq1.}
$$

Both stay in $y>0$, have the required endpoints and satisfy the variational equation. These are the [two optical rays in a square-root refractive-index profile](../../mathematical-physics.md#two-optical-rays-in-a-square-root-refractive-index-profile). Fermat stationarity supplies two rays; it does not assert that both globally minimize travel time.

<a id="9/c/image-the-two-stationary-optical-rays-from-fermat-principle-in-a-medium-with-refractive-index-4-sqrt-y"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-1-square-root-index-rays.png)

**[Figure 1](#9/c/image-the-two-stationary-optical-rays-from-fermat-principle-in-a-medium-with-refractive-index-4-sqrt-y). The two stationary optical rays from Fermat principle in a medium with refractive index $4\sqrt y$**.

## 10

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10/a">a</h3>

↑ **Parent:** [10](#10)

<h4 id="10/a/solution">Solution</h4>

↑ **Parent:** [A](#10/a)

Take real admissible functions with finite $F,G$, positive $G$, and a self-adjoint domain for the [Sturm-Liouville operator](../../sturm-liouville-theory.md#sturm-liouville-operator). Compactly supported variations $\eta$ avoid any boundary contribution at infinity. Formal self-adjointness gives

$$
\delta F=\int_{\mathbb R}[\eta Ly+yL\eta]dx=2\int_{\mathbb R}\eta Ly\,dx,\qquad\delta G=2\int_{\mathbb R}wy\eta\,dx.
$$

For $\Lambda=F/G$, the quotient rule therefore gives

$$
\delta\Lambda=\frac2G\int_{\mathbb R}\eta(Ly-\Lambda wy)dx.
$$

Vanishing for arbitrary variations requires

$$
\boxed{Ly=\lambda wy,\qquad\lambda=\Lambda[y].}
$$

Conversely an [eigenfunction](../../linear-operator-theory.md#eigenfunction) in the self-adjoint domain makes this variation zero. Multiplying its equation by $y$ and integrating also shows directly that its stationary quotient is $\boxed{\Lambda[y_n]=\lambda_n}$.

Thus the stationary values are the admissible [eigenvalues](../../linear-operator-theory.md#eigenvalue). Under the usual positive-weight, semibounded hypotheses the lowest is the global minimum, while higher [eigenfunctions](../../linear-operator-theory.md#eigenfunction) generally give saddle points. The assumption $y\to0$ alone is not a complete domain specification for arbitrary $\rho,\sigma$: the required integrals and boundary form must exist. The rapidly decaying oscillator trials in part (b) meet these conditions.

<h3 id="10/b">b</h3>

↑ **Parent:** [10](#10)

<h4 id="10/b/solution">Solution</h4>

↑ **Parent:** [B](#10/b)

Normalize the Gaussian trial first. The [Gaussian integral](../../integral.md#gaussian-integral) gives

$$
1=C^2\sqrt{\frac\pi\alpha},\qquad\boxed{C=\pm\left(\frac\alpha\pi\right)^{1/4}.}
$$

Its second and fourth moments are $\langle x^2\rangle=1/(2\alpha)$ and $\langle x^4\rangle=3/(4\alpha^2)$. Since $\psi'=-\alpha x\psi$, the kinetic term is $\int(\psi')^2=\alpha^2\langle x^2\rangle=\alpha/2$. At the specified coupling, the [energy](../../energy.md) is therefore

$$
E(\alpha)=\frac\alpha2+\frac1{2\alpha}+\frac3{2\alpha^2}.
$$

The stationary condition is

$$
E'(\alpha)=\frac{\alpha^3-\alpha-6}{2\alpha^3}=0,\qquad\alpha^3-\alpha-6=(\alpha-2)(\alpha^2+2\alpha+3).
$$

The quadratic factor is positive for real $\alpha$, so the unique positive stationary width is $\alpha=2$. Also $E''=\alpha^{-3}+9\alpha^{-4}>0$ and $E$ diverges at both ends of $\alpha>0$, proving a global minimum within this trial family. Its value is

$$
\boxed{E_{\rm trial,min}=\frac{13}{8},\qquad\psi_*(x)=\pm(2/\pi)^{1/4}e^{-x^2}.}
$$

The associated [Sturm-Liouville problem](../../sturm-liouville-theory.md#sturm-liouville-problem) is

$$
\boxed{-\psi''+(x^2+2x^4)\psi=E\psi,\qquad\psi\in L^2(\mathbb R),\quad\psi\to0\text{ at }\pm\infty.}
$$

Here $\rho=1$, $\sigma=x^2+2x^4$ and $w=1$. The [Rayleigh-Ritz variational principle](../../linear-operator-theory.md#rayleigh-ritz-variational-principle) makes the exact lowest [eigenvalue](../../linear-operator-theory.md#eigenvalue) the minimum over all normalized admissible states. Restricting to Gaussians can only raise this minimum, hence $\boxed{E_0\leq13/8}$. The inequality is strict because $H\psi_*/\psi_*=2-3x^2+2x^4$ is not constant: the trial is not an exact [eigenfunction](../../linear-operator-theory.md#eigenfunction). This is the [Gaussian trial for a quadratic-plus-quartic oscillator](../../quantum-theory.md#gaussian-trial-for-a-quadratic-plus-quartic-oscillator).

<h3 id="10/c">c</h3>

↑ **Parent:** [10](#10)

<h4 id="10/c/solution">Solution</h4>

↑ **Parent:** [C](#10/c)

Enlarge the trial space while retaining the optimized Gaussian. For example, use

$$
\psi(x)=e^{-\alpha x^2/2}(c_0+c_1x^2+c_2x^4+\cdots+c_Nx^{2N}),\qquad N\geq2,
$$

normalize it and minimize the [Rayleigh quotient](../../linear-operator-theory.md#rayleigh-quotient) over its coefficients, optionally optimizing $\alpha$ too. This even trial space respects the even ground-state parity of the confining symmetric potential and adds independent shape freedom beyond a Gaussian width.

The original Gaussian remains included by setting the later coefficients to zero, so the optimized upper bound cannot increase. Finite-basis optimization is the [Rayleigh-Ritz method](../../finite-element-method.md#rayleigh-ritz-method), with matrix entries given by the Hamiltonian and overlap integrals. Increasing the basis size systematically improves the available approximation.

<h3 id="10/d">d</h3>

↑ **Parent:** [10](#10)

<h4 id="10/d/solution">Solution</h4>

↑ **Parent:** [D](#10/d)

For any real coupling, the same normalized Gaussian family has [energy](../../energy.md)

$$
E_\epsilon(\alpha)=\frac\alpha2+\frac1{2\alpha}+\frac{3\epsilon}{4\alpha^2}.
$$

If $\epsilon<0$, then as $\alpha\downarrow0$ the negative $\alpha^{-2}$ term dominates the positive $\alpha^{-1}$ and $\alpha$ terms. Each trial still has finite [energy](../../energy.md), is normalized and decays at infinity, but its [energy](../../energy.md) tends to $-\infty$. Therefore

$$
\boxed{\inf_{\|\psi\|_2=1}E[\psi]=-\infty;\qquad\text{there is no minimum energy.}}
$$

This variational sequence makes the instability of the negative quartic potential explicit, without mistaking any local well near the origin for a global ground-state bound.

## ↑ Ancestors (10)

1. [2019](../2019.md)
2. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
3. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
4. [Year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
