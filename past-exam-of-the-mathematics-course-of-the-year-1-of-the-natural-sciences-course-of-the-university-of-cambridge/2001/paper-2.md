# Paper 2

↑ **Parent:** [2001](../2001.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2001/PaperNST_IA_2.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2001/PaperNST_IA_2.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [Solution](#4/solution)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
- [5](#5)
  - [a](#5/a)
    - [i](#5/a/i)
      - [Solution](#5/a/i/solution)
    - [ii](#5/a/ii)
      - [Solution](#5/a/ii/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
- [7](#7)
  - [a](#7/a)
    - [i](#7/a/i)
      - [Solution](#7/a/i/solution)
    - [ii](#7/a/ii)
      - [Solution](#7/a/ii/solution)
    - [iii](#7/a/iii)
      - [Solution](#7/a/iii/solution)
  - [b](#7/b)
    - [Solution](#7/b/solution)
  - [c](#7/c)
    - [Solution](#7/c/solution)
- [8](#8)
  - [a](#8/a)
    - [Solution](#8/a/solution)
  - [b](#8/b)
    - [Solution](#8/b/solution)
- [9](#9)
  - [a](#9/a)
    - [i](#9/a/i)
      - [Solution](#9/a/i/solution)
    - [ii](#9/a/ii)
      - [Solution](#9/a/ii/solution)
  - [b](#9/b)
    - [Solution](#9/b/solution)
- [10](#10)
  - [Solution](#10/solution)
- [11](#11)
  - [a](#11/a)
    - [Solution](#11/a/solution)
  - [b](#11/b)
    - [i](#11/b/i)
      - [Solution](#11/b/i/solution)
    - [ii](#11/b/ii)
      - [Solution](#11/b/ii/solution)
    - [iii](#11/b/iii)
      - [Solution](#11/b/iii/solution)
    - [iv](#11/b/iv)
      - [Solution](#11/b/iv/solution)
    - [v](#11/b/v)
      - [Solution](#11/b/v/solution)
- [12](#12)
  - [a](#12/a)
    - [i](#12/a/i)
      - [Solution](#12/a/i/solution)
    - [ii](#12/a/ii)
      - [Solution](#12/a/ii/solution)
    - [iii](#12/a/iii)
      - [Solution](#12/a/iii/solution)
  - [b](#12/b)
    - [i](#12/b/i)
      - [Solution](#12/b/i/solution)
    - [ii](#12/b/ii)
      - [Solution](#12/b/ii/solution)
  - [c](#12/c)
    - [Solution](#12/c/solution)

## 1

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Separate the variables in this [first-order ordinary differential equation](../../differential-equation.md#first-order-ordinary-differential-equation):

$$
\frac{y}{y^2+2}\,dy=\frac{x}{x^2-3}\,dx.
$$

Integration gives $\tfrac12\ln(y^2+2)=\tfrac12\ln|x^2-3|+C$, so $y^2+2=K|x^2-3|$. On the interval containing the prescribed point $x=3$, we have $x^2-3>0$. The [initial condition](../../differential-equation.md#initial-condition) $y(3)=4$ therefore gives $18=6K$, hence $K=3$. Choosing the positive [square root](../../algebra.md#square-root) to match that [initial condition](../../differential-equation.md#initial-condition) yields

$$
\boxed{y(x)=\sqrt{3x^2-11}.}
$$

The maximal interval containing $3$ on which this solves the explicit [ordinary differential equation](../../differential-equation.md#ordinary-differential-equation) is $\boxed{x>\sqrt{11/3}}$. At the left endpoint $y=0$, the original denominator vanishes and the [derivative](../../calculus.md#derivative) becomes unbounded. Directly, $y'=3x/y$ and $x(2+y^2)/[y(x^2-3)]=3x/y$, verifying the equation throughout this interval.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Recognize the left-hand side as a [product rule](../../calculus.md#product-rule) [derivative](../../calculus.md#derivative), and use $\tfrac12\sin2x=\sin x\cos x$:

$$
\frac{d}{dx}(y\sin x)=\sin x\cos x,\qquad y\sin x=\frac12\sin^2x+C.
$$

At $x=\pi/6$, both $y\sin x$ and $\tfrac12\sin^2x$ equal $1/8$, so $C=0$. Therefore

$$
\boxed{y(x)=\frac12\sin x.}
$$

Dividing by $\sin x$ first obtains this solution on $(0,\pi)$, the interval containing the [initial condition](../../differential-equation.md#initial-condition). The explicit expression is smooth on the entire real line and satisfies the original, undivided [differential equation](../../differential-equation.md) even where $\sin x=0$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For this [homogeneous first-order differential equation](../../differential-equation.md#homogeneous-first-order-differential-equation), set $v=y/x$, with $x\ne0$. The [product rule](../../calculus.md#product-rule) gives $y'=v+xv'$, and substitution simplifies the equation to

$$
(1+2ve^v)xv'=2(1-v^2e^v).
$$

The useful further substitution is $w=e^{-v}-v^2$. Its [chain rule](../../calculus.md#chain-rule) [derivative](../../calculus.md#derivative) satisfies

$$
x\frac{dw}{dx}=-(e^{-v}+2v)xv'=-2(e^{-v}-v^2)=-2w.
$$

Thus $(x^2w)'=0$. Replacing $v$ and $w$ gives the [implicit solution](../../differential-equation.md#implicit-solution)

$$
\boxed{x^2e^{-y/x}-y^2=C,\qquad x\ne0.}
$$

No division by $w$ was needed, so the level $C=0$ is included. A direct verification also identifies the [integrating factor for a differential one-form](../../linear-ordinary-differential-equation.md#integrating-factor-for-a-differential-one-form):

$$
d\bigl(x^2e^{-y/x}-y^2\bigr)=e^{-y/x}(2x+y)\,dx-(xe^{-y/x}+2y)\,dy.
$$

Setting this [exact differential](../../differential-form.md#exact-differential) to zero recovers precisely the original equation after multiplication by the nonzero factor $e^{y/x}$. The coefficient $1+2ve^v$ never vanishes for real $v$, since $ve^v\geq-1/e$ implies $1+2ve^v\geq1-2/e>0$. Hence these [level sets](../../topology.md#level-set) give local [function graphs](../../function.md#graph-of-a-function) $y(x)$ everywhere with $x\ne0$.

## 2

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [generalized Leibniz rule](../../calculus.md#generalized-leibniz-rule) follows by [mathematical induction](../../foundations-of-mathematics.md#mathematical-induction). The case $n=0$ is the identity $uv=uv$. Suppose the formula holds for $n$ and differentiate every term using the [product rule](../../calculus.md#product-rule):

$$
(uv)^{(n+1)}=\sum_{r=0}^n\binom nr\left[u^{(r+1)}v^{(n-r)}+u^{(r)}v^{(n-r+1)}\right].
$$

For an interior index $r$, the coefficient of $u^{(r)}v^{(n+1-r)}$ becomes $\binom n{r-1}+\binom nr=\binom{n+1}r$ by [Pascal's identity](../../binomial-coefficient.md#pascal-s-rule). The two endpoint coefficients are one. This proves

$$
\boxed{(uv)^{(n)}=\sum_{r=0}^n\binom nr u^{(r)}v^{(n-r)},\qquad\binom nr=\frac{n!}{r!(n-r)!}.}
$$

Only finitely many [derivatives](../../calculus.md#derivative) are involved; it suffices that both [functions](../../function.md) are $n$ times differentiable.

For $u=x(x+1)$ and $v=e^{2x}$, the [derivatives](../../calculus.md#derivative) of $u$ beyond order two vanish. The three surviving terms of the [generalized Leibniz rule](../../calculus.md#generalized-leibniz-rule) give

$$
\begin{aligned}
\frac{d^n}{dx^n}\bigl[x(x+1)e^{2x}\bigr]
&=e^{2x}\left[2^n(x^2+x)+n2^{n-1}(2x+1)+n(n-1)2^{n-2}\right]\\
&=\boxed{2^ne^{2x}\left[x^2+(n+1)x+\frac{n(n+1)}4\right].}
\end{aligned}
$$

The simplified expression works for every integer $n\geq0$, including the two cases where one or more of the three terms are absent.

For $u=x^2$ and $v=\sin x$, use $d^m(\sin x)/dx^m=\sin(x+m\pi/2)$. Again only three terms survive. With $T=x+n\pi/2$, they are

$$
\frac{d^n}{dx^n}(x^2\sin x)=x^2\sin T+2nx\sin(T-\pi/2)+n(n-1)\sin(T-\pi).
$$

Since $\sin(T-\pi/2)=-\cos T$ and $\sin(T-\pi)=-\sin T$, this becomes

$$
\boxed{\frac{d^n}{dx^n}(x^2\sin x)=\bigl[x^2-n(n-1)\bigr]\sin\left(x+\frac{n\pi}2\right)-2nx\cos\left(x+\frac{n\pi}2\right).}
$$

The factors $n$ and $n(n-1)$ remove the nonexistent terms when $n=0$ or $1$.

## 3

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The conversion from [cylindrical coordinates](../../multivariable-calculus.md#cylindrical-coordinate-system) to [Cartesian coordinates](../../linear-algebra.md#cartesian-coordinate-system) is

$$
\boxed{x=\rho\cos\phi,\qquad y=\rho\sin\phi,\qquad z=z.}
$$

Here $\rho\geq0$ is the distance from the $z$ axis and $\phi$ is measured around that axis. A full turn $\phi\mapsto\phi+2\pi$ describes the same point.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

On the [circular cylinder](../../differential-geometry.md#circular-cylinder), $\rho=R$ is constant, so the given [line element](../../riemannian-metric.md#line-element) reduces to $ds^2=R^2d\phi^2+dz^2$. Unroll the [circular cylinder](../../differential-geometry.md#circular-cylinder) with $u=R\phi$. The [line element](../../riemannian-metric.md#line-element) is then $ds^2=du^2+dz^2$, so the usual [Euclidean geometry](../../euclidean-geometry.md) formula measures [arc length](../../riemannian-geometry.md#arc-length) in the $(u,z)$ [plane](../../geometry-and-topology.md#plane).

The endpoint has infinitely many lifts $(R(\phi_1+2\pi k),z_1)$, with $k\in\mathbb Z$. For each lift, the [straight line](../../euclidean-geometry.md#straight-line) segment is shortest; its [length](../../physics.md#length) is $\sqrt{R^2(\phi_1+2\pi k)^2+z_1^2}$. Comparing the lifts gives the unrestricted [shortest path on a circular cylinder](../../differential-geometry.md#shortest-path-on-a-circular-cylinder):

$$
\boxed{L_{\min}=\min_{k\in\mathbb Z}\sqrt{R^2(\phi_1+2\pi k)^2+z_1^2}.}
$$

If $\delta$ is a minimizing angular increment, a shortest [geodesic](../../riemannian-geometry.md#geodesic) is parametrized by $(\rho,\phi,z)=(R,\delta t,z_1t)$, $0\leq t\leq1$. This is a [helix](../../topology.md#helix) when both increments are nonzero, and a circular arc or vertical generator in the limiting cases. A nonminimal lift also gives a [geodesic](../../riemannian-geometry.md#geodesic), but it is only shortest within its fixed winding class.

For $0\leq\phi_1\leq2\pi$, put $m=\min(\phi_1,2\pi-\phi_1)$. Then $\boxed{L_{\min}=\sqrt{R^2m^2+z_1^2}}$. At $\phi_1=\pi$, both winding directions give distinct shortest paths of equal [length](../../physics.md#length).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For $R=1$ and $z_1=0$, the [shortest path on a circular cylinder](../../differential-geometry.md#shortest-path-on-a-circular-cylinder) has [length](../../physics.md#length)

$$
\boxed{L_0(\phi_1)=\begin{cases}\phi_1,&0\leq\phi_1\leq\pi,\\2\pi-\phi_1,&\pi\leq\phi_1\leq2\pi.\end{cases}}
$$

Its graph is triangular, with endpoint values zero and maximum $\pi$ at $\phi_1=\pi$. In particular, increasing the angle to a full turn brings the endpoint back to the starting point.

For $R=1$ and $z_1=1$, the corresponding [length](../../physics.md#length) is

$$
\boxed{L_1(\phi_1)=\sqrt{1+\min(\phi_1,2\pi-\phi_1)^2}.}
$$

This graph has endpoint values one, a maximum $\sqrt{1+\pi^2}$ at $\pi$, and symmetry about $\pi$. Each half is smooth, with horizontal slope at the outer endpoint; at $\pi$ the two halves meet at a corner, because the minimizing winding direction changes.

<a id="3/c/image-unrolling-a-cylinder-and-choosing-the-shorter-angular-route"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-2-q3-cylinder-shortest-paths.png)

**[Figure 1](#3/c/image-unrolling-a-cylinder-and-choosing-the-shorter-angular-route). Unrolling a cylinder and choosing the shorter angular route**. Original diagram. Left: two lifts of an endpoint at angular position $3\pi/2$ and height one; the negative angular increment $-\pi/2$ gives the shorter segment. Right: both requested shortest-length graphs for unit radius, with height differences zero and one.

## 4

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

At an ordinary point, an order-$n$ [linear ordinary differential equation](../../linear-ordinary-differential-equation.md) has $n$ arbitrary constants in its general solution. Determining them uniquely requires $n$ independent, consistent scalar conditions. Prescribing $y,y',\ldots,y^{(n-1)}$ at one ordinary point gives uniqueness under the standard continuous-coefficient assumptions. Conditions at different endpoints need an additional nonsingularity check: for example, $y''+y=0$, $y(0)=y(\pi)=0$ leaves every multiple of $\sin x$ possible. Thus counting [boundary conditions](../../differential-equation.md#boundary-condition) alone does not guarantee uniqueness for a [boundary value problem](../../boundary-value-problem.md).

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [characteristic equation](../../linear-ordinary-differential-equation.md#characteristic-equation-of-a-constant-coefficient-differential-equation) is $m^2+3m+2=(m+1)(m+2)=0$, giving the [complementary function](../../linear-ordinary-differential-equation.md#homogeneous-solution) $C_1e^{-x}+C_2e^{-2x}$. For the forcing term $x$, a linear [particular solution](../../linear-ordinary-differential-equation.md#particular-solution) $ax+b$ gives $2ax+3a+2b=x$, hence $a=1/2$, $b=-3/4$.

The forcing $-e^{-x}$ gives [resonance in a differential equation](../../linear-ordinary-differential-equation.md#resonance-in-a-differential-equation), since $e^{-x}$ already appears in the [complementary function](../../linear-ordinary-differential-equation.md#homogeneous-solution). Try $Kxe^{-x}$. Direct differentiation gives

$$
\left(\frac{d^2}{dx^2}+3\frac d{dx}+2\right)(Kxe^{-x})=Ke^{-x},
$$

so $K=-1$. Combining the two [particular solutions](../../linear-ordinary-differential-equation.md#particular-solution) gives

$$
\boxed{y=(C_1-x)e^{-x}+C_2e^{-2x}+\frac x2-\frac34.}
$$

The factor $x$ in the [resonant exponential particular solution](../../linear-ordinary-differential-equation.md#resonant-exponential-particular-solution) is required because $-1$ is already a root of the [characteristic equation](../../linear-ordinary-differential-equation.md#characteristic-equation-of-a-constant-coefficient-differential-equation).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Now the [characteristic equation](../../linear-ordinary-differential-equation.md#characteristic-equation-of-a-constant-coefficient-differential-equation) is $(m+1)^2=0$, with a [repeated root](../../polynomial.md#multiple-root), so the [complementary function](../../linear-ordinary-differential-equation.md#homogeneous-solution) is $(C_1+C_2x)e^{-x}$. For the polynomial forcing, substitute $ax^2+bx+c$ to obtain

$$
ax^2+(4a+b)x+(2a+2b+c)=x^2.
$$

Thus $a=1$, $b=-4$, $c=6$. For the forcing $2e^{-x}$, both $e^{-x}$ and $xe^{-x}$ already occur in the [complementary function](../../linear-ordinary-differential-equation.md#homogeneous-solution); the [resonant exponential particular solution](../../linear-ordinary-differential-equation.md#resonant-exponential-particular-solution) therefore starts with $Kx^2e^{-x}$. The identity

$$
\left(\frac{d^2}{dx^2}+2\frac d{dx}+1\right)(e^{-x}v)=e^{-x}v''
$$

gives $K=1$. The resulting general solution is

$$
\boxed{y=(C_1+C_2x+x^2)e^{-x}+x^2-4x+6.}
$$

## 5

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/i">i</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5/a/i)

Parametrize the [straight line](../../euclidean-geometry.md#straight-line) by $r(t)=(t,t,t)$, $0\leq t\leq1$, with $r'(t)=(1,1,1)$. Substituting into the [vector field](../../multivariable-calculus.md#vector-field) and taking the [dot product](../../inner-product.md#dot-product) gives

$$
v(r(t))\cdot r'(t)=(t+1)e^t+5t^4.
$$

Hence the direct [line integral](../../multivariable-calculus.md#line-integral) is

$$
\boxed{\int_Cv\cdot dr=\int_0^1\bigl[(t+1)e^t+5t^4\bigr]\,dt=\left[te^t+t^5\right]_0^1=e+1.}
$$

<h4 id="5/a/ii">ii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/a/ii)

For the curved path $r(t)=(t,t^2,t^3)$, $r'(t)=(1,2t,3t^2)$. The [vector field](../../multivariable-calculus.md#vector-field) along this [parametric curve](../../topology.md#parametric-curve) is

$$
v(r(t))=(t^2e^t,\ e^t+2t^{11},\ 3t^{10}).
$$

Its [dot product](../../inner-product.md#dot-product) with the tangent is $(t^2+2t)e^t+13t^{12}$. Therefore the direct [line integral](../../multivariable-calculus.md#line-integral) is

$$
\boxed{\int_Cv\cdot dr=\int_0^1\bigl[(t^2+2t)e^t+13t^{12}\bigr]\,dt=\left[t^2e^t+t^{13}\right]_0^1=e+1.}
$$

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Compute the [curl](../../multivariable-calculus.md#curl) in [Cartesian coordinates](../../linear-algebra.md#cartesian-coordinate-system):

$$
\nabla\times v=\left(\partial_y(3y^2z^2)-\partial_z(e^x+2yz^3),\ \partial_z(e^xy)-\partial_x(3y^2z^2),\ \partial_x(e^x+2yz^3)-\partial_y(e^xy)\right).
$$

The three components are $6yz^2-6yz^2$, $0-0$, and $e^x-e^x$. Consequently

$$
\boxed{\nabla\times v=(0,0,0).}
$$

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Integrate $f_x=ye^x$ with respect to $x$, obtaining $f=ye^x+g(y,z)$. Matching $f_y=e^x+2yz^3$ gives $g_y=2yz^3$, so $g=y^2z^3+h(z)$. Finally, $f_z=3y^2z^2+h'(z)$ must equal the third component, so $h'=0$. Thus a [scalar potential](../../classical-field-theory.md#scalar-potential) is

$$
\boxed{f(x,y,z)=ye^x+y^2z^3+C,\qquad v=\nabla f.}
$$

The [fundamental theorem for line integrals](../../multivariable-calculus.md#fundamental-theorem-for-line-integrals) now gives $\int_Cv\cdot dr=f(1,1,1)-f(0,0,0)=e+1$ for either path, confirming both direct computations. Since the [curl of a gradient](../../multivariable-calculus.md#curl-of-a-gradient) is zero for this smooth [function](../../function.md), it also confirms the result in part (b). The potential is defined throughout $\mathbb R^3$, so no domain obstruction to [path independence](../../multivariable-calculus.md#path-independence) occurs.

## 6

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Use a [Lagrange multiplier](../../mathematical-optimization.md#lagrange-multiplier) to maximize $V=\pi r^2h$ subject to $2\pi r(r+h)=A$, with $r,h>0$. The equations $\nabla V=\lambda\nabla A$ are

$$
2\pi rh=\lambda(4\pi r+2\pi h),\qquad\pi r^2=2\lambda\pi r.
$$

The second equation gives $\lambda=r/2$. Substituting into the first gives $2rh=r(2r+h)$, hence $h=2r$. The [constraint](../../classical-mechanics.md#constraint-mechanics) then gives $A=6\pi r^2$, so

$$
\boxed{r=\sqrt{\frac A{6\pi}},\qquad h=2\sqrt{\frac A{6\pi}},\qquad V_{\max}=2\pi\left(\frac A{6\pi}\right)^{3/2}=\frac13\sqrt{\frac{A^3}{6\pi}}.}
$$

This is the same aspect ratio as the [minimum-area closed cylinder at fixed volume](../../mathematical-optimization.md#minimum-area-closed-cylinder-at-fixed-volume). To confirm maximality directly, eliminate $h$: $V(r)=Ar/2-\pi r^3$ on $0<r<\sqrt{A/(2\pi)}$. Its only stationary point is the value above, its second [derivative](../../calculus.md#derivative) there is negative, and the [volume](../../geometry-and-topology.md#volume) tends to zero at either end of the interval.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Maximize the total [surface area](../../differential-geometry.md#surface-area) $A=2\pi r(r+h)$ with the [constraint](../../classical-mechanics.md#constraint-mechanics) $g=r^2+h^2/4=1$. The [Lagrange multiplier](../../mathematical-optimization.md#lagrange-multiplier) equations are

$$
4\pi r+2\pi h=2\lambda r,\qquad2\pi r=\lambda h/2.
$$

From the second, $\lambda=4\pi r/h$. Substitute into the first and multiply by $h/(2\pi)$ to obtain $2rh+h^2=4r^2$. Thus the aspect ratio $q=h/r$ satisfies $q^2+2q-4=0$. Since $q>0$,

$$
\boxed{\frac hr=\sqrt5-1.}
$$

This is the [maximum-area cylinder inscribed in a sphere](../../mathematical-optimization.md#maximum-area-cylinder-inscribed-in-a-sphere). The dimensions and area, although not needed to specify the ratio, are

$$
r^2=\frac{5+\sqrt5}{10},\qquad h^2=\frac{2(5-\sqrt5)}5,\qquad A_{\max}=\pi(1+\sqrt5).
$$

There is only one positive stationary ratio. At the degenerate boundaries $r=0$ and $h=0$, the limiting areas are zero and $2\pi$, both below this value, confirming the maximum.

## 7

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/i">i</h4>

↑ **Parent:** [A](#7/a)

<h5 id="7/a/i/solution">Solution</h5>

↑ **Parent:** [I](#7/a/i)

The two-by-two [determinant](../../multilinear-algebra.md#determinant) is the difference of the diagonal products:

$$
\boxed{\begin{vmatrix}8&1\\5&3\end{vmatrix}=8\cdot3-1\cdot5=19.}
$$

<h4 id="7/a/ii">ii</h4>

↑ **Parent:** [A](#7/a)

<h5 id="7/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7/a/ii)

Expand the [determinant](../../multilinear-algebra.md#determinant) along the first row:

$$
\boxed{\begin{vmatrix}4&1&-2\\3&0&4\\10&1&-4\end{vmatrix}=4(-4)-1(-12-40)-2(3)=30.}
$$

The minus sign on the middle [cofactor](../../linear-algebra.md#cofactor) is essential.

<h4 id="7/a/iii">iii</h4>

↑ **Parent:** [A](#7/a)

<h5 id="7/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#7/a/iii)

The third row is twice the first, so the rows are [linearly dependent](../../vector-space.md#linear-dependence). Hence

$$
\boxed{\begin{vmatrix}4&1&-2\\3&0&4\\8&2&-4\end{vmatrix}=0.}
$$

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/solution">Solution</h4>

↑ **Parent:** [B](#7/b)

The [homogeneous linear system](../../linear-algebra.md#homogeneous-linear-system) has coefficient [matrix](../../vector-space.md#matrix)

$$
M=\begin{pmatrix}1&0&-3\\1&\lambda&-\lambda\\1&2&\lambda\end{pmatrix}.
$$

Nonzero solutions exist exactly when its [determinant](../../multilinear-algebra.md#determinant) vanishes. Expanding along the first row gives

$$
\det M=\lambda(\lambda+2)-3(2-\lambda)=\lambda^2+5\lambda-6=(\lambda-1)(\lambda+6).
$$

Thus $\lambda=1$ or $-6$. The first equation always gives $x=3z$. For $\lambda=1$, the second then gives $y=-2z$; the third imposes the same relation. For $\lambda=-6$, the second gives $y=3z/2$, again consistent with the third. Therefore the nonzero solutions are

$$
\boxed{\begin{cases}\lambda=1:&(x,y,z)=t(3,-2,1),\\\lambda=-6:&(x,y,z)=t(6,3,2),\end{cases}\qquad t\in\mathbb R\setminus\{0\}.}
$$

For every other $\lambda$, the [matrix](../../vector-space.md#matrix) is invertible and only the zero solution exists.

<h3 id="7/c">c</h3>

↑ **Parent:** [7](#7)

<h4 id="7/c/solution">Solution</h4>

↑ **Parent:** [C](#7/c)

Here the vertical bars denote [determinants](../../multilinear-algebra.md#determinant). Since $B=B^{-1}$, taking [determinants](../../multilinear-algebra.md#determinant) gives $(\det B)^2=1$. The condition $\det B>0$ selects $\det B=1$. By the multiplicative property of the [determinant](../../multilinear-algebra.md#determinant),

$$
\boxed{\det A=\frac{\det(AB)}{\det B}=\frac{-2}{1}=-2.}
$$

The hypotheses determine this [determinant](../../multilinear-algebra.md#determinant), while allowing many possible [matrices](../../vector-space.md#matrix) $A$ and $B$.

## 8

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8/a">a</h3>

↑ **Parent:** [8](#8)

<h4 id="8/a/solution">Solution</h4>

↑ **Parent:** [A](#8/a)

The [region of integration](../../integral.md#domain-of-integration) is $0\leq y\leq1$, $y\leq x\leq2-y$. It is the closed [triangle](../../euclidean-geometry.md#triangle) with vertices $(0,0)$, $(2,0)$, and $(1,1)$, bounded by $y=0$, $x=y$, and $x=2-y$. Each horizontal slice runs from the rising left edge to the falling right edge.

<a id="8/a/image-triangular-integration-region-and-a-horizontal-integration-slice"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-2-q8-triangular-region.png)

**[Figure 2](#8/a/image-triangular-integration-region-and-a-horizontal-integration-slice). Triangular integration region and a horizontal integration slice**. Original diagram of the region $0\leq y\leq1$, $y\leq x\leq2-y$, with its three vertices, boundary equations, and an example slice at fixed $y$.

Integrate with respect to $x$ first:

$$
\begin{aligned}
I&=\int_0^1\left[\frac23x^3+yx\right]_{x=y}^{x=2-y}\,dy\\
&=\int_0^1\left[\frac{16}3-6y+2y^2-\frac43y^3\right]dy\\
&=\frac{16}3-3+\frac23-\frac13=\boxed{\frac83}.
\end{aligned}
$$

The [triangle](../../euclidean-geometry.md#triangle) has area one, but the nonconstant integrand makes the [double integral](../../integral.md#double-integral) a weighted area.

<h3 id="8/b">b</h3>

↑ **Parent:** [8](#8)

<h4 id="8/b/solution">Solution</h4>

↑ **Parent:** [B](#8/b)

Use the [spherical polar coordinates](../../multivariable-calculus.md#spherical-coordinate-system) [volume element](../../integral.md#volume-element) $dV=r^2\sin\theta\,dr\,d\theta\,d\phi$. Since $1+\cos\theta\geq0$ throughout $0\leq\theta\leq\pi$, the solid has radial range $0\leq r\leq1+\cos\theta$ and full azimuthal range $0\leq\phi<2\pi$. Its [volume](../../geometry-and-topology.md#volume) is

$$
V=\int_0^{2\pi}\int_0^\pi\int_0^{1+\cos\theta}r^2\sin\theta\,dr\,d\theta\,d\phi=\frac{2\pi}3\int_0^\pi(1+\cos\theta)^3\sin\theta\,d\theta.
$$

Put $u=1+\cos\theta$, so $du=-\sin\theta\,d\theta$ and the endpoints become $2$ and $0$. Consequently

$$
\boxed{V=\frac{2\pi}3\int_0^2u^3\,du=\frac{8\pi}3.}
$$

The polar equation describes the entire three-dimensional surface, so the [spherical polar coordinates](../../multivariable-calculus.md#spherical-coordinate-system) [volume element](../../integral.md#volume-element), rather than a two-dimensional polar area element, is required.

## 9

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9/a">a</h3>

↑ **Parent:** [9](#9)

<h4 id="9/a/i">i</h4>

↑ **Parent:** [A](#9/a)

<h5 id="9/a/i/solution">Solution</h5>

↑ **Parent:** [I](#9/a/i)

Solve the two algebraic [constraints](../../classical-mechanics.md#constraint-mechanics) for the squared coordinates:

$$
x^2=\frac{z^2+u^2}{3},\qquad y^2=\frac{z^2-2u^2}{3}.
$$

On any nonsingular real branch, [implicit differentiation](../../multivariable-calculus.md#implicit-differentiation) at fixed $u$ gives $(\partial x/\partial z)_u=z/(3x)$ and $(\partial y/\partial z)_u=z/(3y)$. Differentiating $z^2=2x^2+y^2$ with the other original coordinate fixed gives $(\partial z/\partial x)_y=2x/z$ and $(\partial z/\partial y)_x=y/z$. Therefore

$$
\boxed{\left(\frac{\partial x}{\partial z}\right)_u\left(\frac{\partial z}{\partial x}\right)_y+\left(\frac{\partial y}{\partial z}\right)_u\left(\frac{\partial z}{\partial y}\right)_x=\frac z{3x}\frac{2x}z+\frac z{3y}\frac yz=\frac23+\frac13=1.}
$$

This is the [multivariable chain rule](../../calculus.md#multivariable-chain-rule) applied to $z(x(z,u),y(z,u))=z$. These formulas assume the relevant denominators are nonzero and the chosen variables are valid local coordinates.

<h4 id="9/a/ii">ii</h4>

↑ **Parent:** [A](#9/a)

<h5 id="9/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#9/a/ii)

At fixed $z$, differentiating $2x^2+y^2=z^2$ gives $(\partial x/\partial y)_z=-y/(2x)$. Also, $x^2=(z^2+u^2)/3$ gives $(\partial x/\partial u)_z=u/(3x)$. At fixed $y$, eliminate $x^2$ to write $u^2=(z^2-3y^2)/2$, giving $(\partial u/\partial z)_y=z/(2u)$. Finally, the previous part gave $(\partial y/\partial z)_u=z/(3y)$. Thus

$$
\boxed{\left(\frac{\partial x}{\partial y}\right)_z\left(\frac{\partial y}{\partial z}\right)_u+\left(\frac{\partial x}{\partial u}\right)_z\left(\frac{\partial u}{\partial z}\right)_y=-\frac y{2x}\frac z{3y}+\frac u{3x}\frac z{2u}=0.}
$$

The held-fixed subscripts matter: substituting a reciprocal [partial derivative](../../multivariable-calculus.md#partial-derivative) while silently changing what is held fixed would not preserve these cancellations.

<h3 id="9/b">b</h3>

↑ **Parent:** [9](#9)

<h4 id="9/b/solution">Solution</h4>

↑ **Parent:** [B](#9/b)

Differentiate both algebraic [constraints](../../classical-mechanics.md#constraint-mechanics) at fixed $y$ or fixed $x$:

$$
z_x=\frac{2x}z,\quad z_y=\frac yz,\qquad u_x=\frac xu,\quad u_y=-\frac yu.
$$

The [multivariable chain rule](../../calculus.md#multivariable-chain-rule) for $\phi(x,y)=\psi(z,u)$ therefore gives

$$
\left(\frac{\partial\phi}{\partial x}\right)_y=\frac{2x}z\left(\frac{\partial\psi}{\partial z}\right)_u+\frac xu\left(\frac{\partial\psi}{\partial u}\right)_z,\qquad\left(\frac{\partial\phi}{\partial y}\right)_x=\frac yz\left(\frac{\partial\psi}{\partial z}\right)_u-\frac yu\left(\frac{\partial\psi}{\partial u}\right)_z.
$$

Divide the first identity by $x$ and the second by $y$, and add. The $\psi_u$ terms cancel, leaving

$$
\boxed{\frac1x\left(\frac{\partial\phi}{\partial x}\right)_y+\frac1y\left(\frac{\partial\phi}{\partial y}\right)_x=\frac3z\left(\frac{\partial\psi}{\partial z}\right)_u.}
$$

The [Jacobian determinant](../../multivariable-calculus.md#jacobian-determinant) of $(x,y)\mapsto(z,u)$ is $-3xy/(zu)$, so the calculation is valid on real branches with $xyzu\ne0$. This explicitly supplies the local independence assumption underlying the change of coordinates.

## 10

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10/solution">Solution</h3>

↑ **Parent:** [10](#10)

If $P\,dx+Q\,dy=dF$ for a twice continuously differentiable potential $F$, then $P=F_x$ and $Q=F_y$. Equality of [mixed partial derivatives](../../multivariable-calculus.md#mixed-partial-derivative) gives the necessary condition for an [exact differential](../../differential-form.md#exact-differential):

$$
\boxed{P_y=Q_x.}
$$

This condition alone does not ensure global exactness on a domain with holes.

For the [Helmholtz free energy](../../thermodynamic-potential.md#helmholtz-free-energy) $A=U-TS$, use the stated identity for [internal energy](../../internal-energy.md) and the [product rule](../../calculus.md#product-rule):

$$
dA=dU-T\,dS-S\,dT=-S\,dT-p\,dV.
$$

Thus $A_T|_V=-S$ and $A_V|_T=-p$. Equality of [mixed partial derivatives](../../multivariable-calculus.md#mixed-partial-derivative) yields the [Maxwell relation](../../thermodynamics.md#maxwell-relations)

$$
\boxed{\left(\frac{\partial S}{\partial V}\right)_T=\left(\frac{\partial p}{\partial T}\right)_V.}
$$

The [temperature](../../temperature.md) and [volume](../../thermodynamics.md#volume-thermodynamics) are the independent variables here, with composition and amount of gas fixed.

Next express $S=S(T,V)$ and substitute its [total differential](../../multivariable-calculus.md#total-differential) into $dU=T\,dS-p\,dV$:

$$
dU=T\left(\frac{\partial S}{\partial T}\right)_VdT+\left[T\left(\frac{\partial S}{\partial V}\right)_T-p\right]dV.
$$

Matching the coefficient of $dV$ gives

$$
\boxed{\left(\frac{\partial U}{\partial V}\right)_T=T\left(\frac{\partial S}{\partial V}\right)_T-p=T\left(\frac{\partial p}{\partial T}\right)_V-p.}
$$

This is the [thermodynamic internal pressure](../../internal-energy.md#thermodynamic-internal-pressure) identity: an [equation of state](../../pressure.md#equation-of-state) determines how [internal energy](../../internal-energy.md) changes under an isothermal change of [volume](../../thermodynamics.md#volume-thermodynamics).

For the [Dieterici equation](../../thermodynamics.md#dieterici-equation), set $c=an/(VR)$ while differentiating at fixed $V$. Then

$$
p=\frac{nR}{V-nb}Te^{-c/T},\qquad\left(\frac{\partial p}{\partial T}\right)_V=\frac{nR}{V-nb}e^{-c/T}\left(1+\frac cT\right).
$$

Substitute into the [thermodynamic internal pressure](../../internal-energy.md#thermodynamic-internal-pressure) identity. The term proportional to $T$ cancels $p$, leaving

$$
\boxed{\left(\frac{\partial U}{\partial V}\right)_T=\frac{an^2}{V(V-nb)}\exp\left(-\frac{an}{VRT}\right).}
$$

The physical gas domain has $T>0$ and $V>nb$.

For the [ideal gas](../../ideal-gas.md) instead, $p=nRT/V$ gives $T(\partial p/\partial T)_V-p=0$. Therefore $U$ is independent of [volume](../../thermodynamics.md#volume-thermodynamics) at fixed amount of gas. Integrating the remaining condition $(\partial U/\partial T)_V=C_V$, with constant [heat capacity at constant volume](../../heat.md#heat-capacity-at-constant-volume), gives

$$
\boxed{U(T,V)=C_VT+U_0,}
$$

where $U_0$ is independent of both $T$ and $V$ and fixes the reference for [internal energy](../../internal-energy.md).

## 11

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="11/a">a</h3>

↑ **Parent:** [11](#11)

<h4 id="11/a/solution">Solution</h4>

↑ **Parent:** [A](#11/a)

With replacement, successive draws are [independent](../../random-variable.md#independent-random-variables), with red [probability](../../probability-theory.md#probability) $2/7$ and green [probability](../../probability-theory.md#probability) $5/7$. The first red on draw $n$ requires $n-1$ greens followed by one red. Hence

$$
\boxed{\mathbb P(N=n)=\left(\frac57\right)^{n-1}\frac27,\qquad n=1,2,\ldots.}
$$

This is a [geometric distribution](../../discrete-probability-distribution.md#geometric-distribution). Its total [probability](../../probability-theory.md#probability) is one because the [geometric series](../../sequence-and-series.md#geometric-series) sums to $(2/7)/(1-5/7)=1$.

<h3 id="11/b">b</h3>

↑ **Parent:** [11](#11)

<h4 id="11/b/i">i</h4>

↑ **Parent:** [B](#11/b)

<h5 id="11/b/i/solution">Solution</h5>

↑ **Parent:** [I](#11/b/i)

There are two red counters among seven equally likely first draws, so

$$
\boxed{\mathbb P(E_1)=\frac27.}
$$

<h4 id="11/b/ii">ii</h4>

↑ **Parent:** [B](#11/b)

<h5 id="11/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#11/b/ii)

Use the [law of total probability](../../probability-space.md#law-of-total-probability) according to the first draw. Without replacement, the second-draw red [probability](../../probability-theory.md#probability) is $1/6$ after a red and $2/6$ after a green. Thus

$$
\boxed{\mathbb P(E_2)=\frac27\frac16+\frac57\frac26=\frac27.}
$$

Equivalently, each counter has the same [probability](../../probability-theory.md#probability) of occupying the second position as the first. Equal marginal [probabilities](../../probability-theory.md#probability) do not make the two draw events [independent](../../random-variable.md#independent-random-variables).

<h4 id="11/b/iii">iii</h4>

↑ **Parent:** [B](#11/b)

<h5 id="11/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#11/b/iii)

After a red first draw, one red remains among six counters. The multiplication rule for [conditional probability](../../probability-theory.md#conditional-probability) gives

$$
\boxed{\mathbb P(E_1\cap E_2)=\mathbb P(E_1)\mathbb P(E_2\mid E_1)=\frac27\frac16=\frac1{21}.}
$$

<h4 id="11/b/iv">iv</h4>

↑ **Parent:** [B](#11/b)

<h5 id="11/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#11/b/iv)

By [inclusion-exclusion](../../combinatorics.md#inclusion-exclusion-principle), subtract the intersection once to correct the double counting:

$$
\boxed{\mathbb P(E_1\cup E_2)=\mathbb P(E_1)+\mathbb P(E_2)-\mathbb P(E_1\cap E_2)=\frac27+\frac27-\frac1{21}=\frac{11}{21}.}
$$

As a check, the complementary event is two greens, of [probability](../../probability-theory.md#probability) $(5/7)(4/6)=10/21$.

<h4 id="11/b/v">v</h4>

↑ **Parent:** [B](#11/b)

<h5 id="11/b/v/solution">Solution</h5>

↑ **Parent:** [V](#11/b/v)

The definition of [conditional probability](../../probability-theory.md#conditional-probability) gives

$$
\boxed{\mathbb P(E_1\mid E_2)=\frac{\mathbb P(E_1\cap E_2)}{\mathbb P(E_2)}=\frac{1/21}{2/7}=\frac16.}
$$

Conditioning on a red in the second position leaves one red among the six counters that could occupy the first position, giving the same result directly.

## 12

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="12/a">a</h3>

↑ **Parent:** [12](#12)

<h4 id="12/a/i">i</h4>

↑ **Parent:** [A](#12/a)

<h5 id="12/a/i/solution">Solution</h5>

↑ **Parent:** [I](#12/a/i)

Using the standard [sine](../../geometry-and-topology.md#sine) [limit](../../calculus.md#limit-of-a-function) $\sin t/t\to1$, with angles in radians,

$$
\boxed{\lim_{x\to0}\frac{\sin2x}{x}=2\lim_{x\to0}\frac{\sin2x}{2x}=2.}
$$

Thus the two-sided [limit](../../calculus.md#limit-of-a-function) exists and is finite.

<h4 id="12/a/ii">ii</h4>

↑ **Parent:** [A](#12/a)

<h5 id="12/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#12/a/ii)

Although $\cos(1/x)$ oscillates without a [limit](../../calculus.md#limit-of-a-function), its magnitude is at most one. Therefore $|x\cos(1/x)|\leq|x|\to0$. The [squeeze theorem](../../calculus.md#squeeze-theorem) gives

$$
\boxed{\lim_{x\to0}x\cos(1/x)=0.}
$$

The shrinking factor $x$ suppresses the oscillation from either side of zero.

<h4 id="12/a/iii">iii</h4>

↑ **Parent:** [A](#12/a)

<h5 id="12/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#12/a/iii)

The [derivative](../../calculus.md#derivative) of the [exponential function](../../calculus.md#exponential-function) at zero gives $e^{-x}=1-x+O(x^2)$. Hence $1-e^{-x}=x+O(x^2)$, and

$$
\boxed{\lim_{x\to0}\frac{x}{1-e^{-x}}=1.}
$$

The denominator is nonzero for every real $x\ne0$, so this is a two-sided finite [limit](../../calculus.md#limit-of-a-function).

<h3 id="12/b">b</h3>

↑ **Parent:** [12](#12)

<h4 id="12/b/i">i</h4>

↑ **Parent:** [B](#12/b)

<h5 id="12/b/i/solution">Solution</h5>

↑ **Parent:** [I](#12/b/i)

A [series](../../sequence-and-series.md#series-mathematics) $\sum_{n=1}^{\infty}u_n$ is a [convergent series](../../sequence-and-series.md#convergent-series) if its [partial sums](../../sequence-and-series.md#partial-sum) $S_N=\sum_{n=1}^Nu_n$ have a finite [limit](../../calculus.md#limit-of-a-function) $S$ as $N\to\infty$. The number $S$ is the sum of the [series](../../sequence-and-series.md#series-mathematics). Explicitly, for every $\varepsilon>0$ there is an integer $N_0$ such that $|S_N-S|<\varepsilon$ whenever $N\geq N_0$. The condition $u_n\to0$ alone is insufficient: the [harmonic series](../../sequence-and-series.md#harmonic-series) has terms tending to zero but diverges.

<h4 id="12/b/ii">ii</h4>

↑ **Parent:** [B](#12/b)

<h5 id="12/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#12/b/ii)

The [series](../../sequence-and-series.md#series-mathematics) $\sum u_n$ has [absolute convergence](../../sequence-and-series.md#absolute-convergence) if $\sum|u_n|$ is a [convergent series](../../sequence-and-series.md#convergent-series), meaning its nonnegative [partial sums](../../sequence-and-series.md#partial-sum) have a finite [limit](../../calculus.md#limit-of-a-function). [Absolute convergence](../../sequence-and-series.md#absolute-convergence) implies convergence of the original real or complex [series](../../sequence-and-series.md#series-mathematics). The converse fails: the [alternating harmonic series](../../sequence-and-series.md#alternating-harmonic-series) converges, while its absolute-value [series](../../sequence-and-series.md#series-mathematics) is the divergent [harmonic series](../../sequence-and-series.md#harmonic-series).

<h3 id="12/c">c</h3>

↑ **Parent:** [12](#12)

<h4 id="12/c/solution">Solution</h4>

↑ **Parent:** [C](#12/c)

The summands $u_n=n^4/2^n$ are positive. Apply the [ratio test](../../sequence-and-series.md#ratio-test):

$$
\frac{u_{n+1}}{u_n}=\frac{(n+1)^4}{2n^4}=\frac12\left(1+\frac1n\right)^4\longrightarrow\frac12<1.
$$

Therefore

$$
\boxed{\sum_{n=1}^{\infty}\frac{n^4}{2^n}\text{ converges absolutely}.}
$$

For a direct comparison interpretation, the ratio is eventually at most any fixed number between $1/2$ and $1$, such as $3/4$. The tail is then bounded by a convergent [geometric series](../../sequence-and-series.md#geometric-series). Thus the exponential denominator wins over the fourth-power numerator strongly enough to make the whole [series](../../sequence-and-series.md#series-mathematics) summable.

## ↑ Ancestors (10)

1. [2001](../2001.md)
2. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
3. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge)
4. [Year 1 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-1-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
