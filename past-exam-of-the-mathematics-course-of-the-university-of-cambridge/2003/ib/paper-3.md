# Paper 3

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2003/PaperIB_3.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2003/PaperIB_3.pdf)

**Table of contents**

- [1F](#1f)
  - [Solution](#1f/solution)
- [2D](#2d)
  - [Solution](#2d/solution)
- [3E](#3e)
  - [a](#3e/a)
    - [Solution](#3e/a/solution)
  - [b](#3e/b)
    - [Solution](#3e/b/solution)
- [4F](#4f)
  - [Solution](#4f/solution)
- [5H](#5h)
  - [Solution](#5h/solution)
- [6B](#6b)
  - [a](#6b/a)
    - [Solution](#6b/a/solution)
  - [b](#6b/b)
    - [Solution](#6b/b/solution)
- [7G](#7g)
  - [Solution](#7g/solution)
- [8C](#8c)
  - [Solution](#8c/solution)
- [9G](#9g)
  - [Solution](#9g/solution)
- [10A](#10a)
  - [Solution](#10a/solution)
- [11F](#11f)
  - [Solution](#11f/solution)
- [12D](#12d)
  - [a](#12d/a)
    - [Solution](#12d/a/solution)
  - [b](#12d/b)
    - [Solution](#12d/b/solution)
- [13E](#13e)
  - [a](#13e/a)
    - [Solution](#13e/a/solution)
  - [b](#13e/b)
    - [Solution](#13e/b/solution)
  - [c](#13e/c)
    - [Solution](#13e/c/solution)
  - [d](#13e/d)
    - [Solution](#13e/d/solution)
  - [e](#13e/e)
    - [Solution](#13e/e/solution)
- [14F](#14f)
  - [Solution](#14f/solution)
- [15H](#15h)
  - [Solution](#15h/solution)
- [16B](#16b)
  - [a](#16b/a)
    - [Solution](#16b/a/solution)
  - [b](#16b/b)
    - [Solution](#16b/b/solution)
- [17G](#17g)
  - [Solution](#17g/solution)
- [18C](#18c)
  - [Solution](#18c/solution)
- [19G](#19g)
  - [a](#19g/a)
    - [Solution](#19g/a/solution)
  - [b](#19g/b)
    - [Solution](#19g/b/solution)
  - [c](#19g/c)
    - [Solution](#19g/c/solution)
  - [d](#19g/d)
    - [Solution](#19g/d/solution)
- [20A](#20a)
  - [Solution](#20a/solution)

## 1F

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="1f/solution">Solution</h3>

↑ **Parent:** [1F](#1f)

The [integral](../../../calculus.md#integral) is finite because a [continuous function](../../../calculus.md#continuous-function) on a [compact](../../../topology.md#compact-space) [closed interval](../../../real-analysis.md#closed-real-interval) is bounded. Nonnegativity is immediate, and [absolute homogeneity of a norm](../../../functional-analysis.md#absolute-homogeneity-of-a-norm) follows from $|cf(x)|=|c|\,|f(x)|$. The pointwise [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives

$$
\|f+g\|\leq\int_{-1}^1(|f(x)|+|g(x)|)\,dx=\|f\|+\|g\|.
$$

For positive definiteness, if $f(x_0)\ne0$, [continuity](../../../calculus.md#continuous-function) gives a relative interval of positive length on which $|f(x)|\geq |f(x_0)|/2$. Its [integral](../../../calculus.md#integral) is positive, including when $x_0$ is an endpoint. Thus $\|f\|=0$ implies $f=0$, and this is a [norm](../../../functional-analysis.md#norm) on the given [vector space](../../../vector-space.md).

For the given [sequence](../../../real-analysis.md#sequence),

$$
\|f_n\|=2\int_0^1x^n\,dx=\frac2{n+1},\qquad \|f_n-f_m\|\leq\frac2{n+1}+\frac2{m+1}.
$$

The last bound tends to zero as both indices tend to infinity, proving the [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) property. Moreover, **the sequence converges to the zero function in this norm**:

$$
\boxed{\|f_n-0\|=\frac2{n+1}\longrightarrow0.}
$$

There is no conflict with the nonzero endpoint values: convergence in this [norm](../../../functional-analysis.md#norm) does not imply [pointwise convergence](../../../real-analysis.md#pointwise-convergence).

## 2D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="2d/solution">Solution</h3>

↑ **Parent:** [2D](#2d)

Write the cone as $z=r\cot\alpha$, with $r$ the distance from its axis and $0<\alpha<\pi/2$. Its [Euclidean metric](../../../differential-geometry.md#euclidean-metric) gives

$$
ds^2=dr^2+r^2d\theta^2+dz^2=\csc^2\alpha\,dr^2+r^2d\theta^2.
$$

Consequently a differentiable path expressed as $r=r(\theta)$ has [arc length](../../../riemannian-geometry.md#arc-length)

$$
\boxed{S=\int\sqrt{r^2+\csc^2\alpha\,(r')^2}\,d\theta.}
$$

For $L(r,r')=\sqrt{r^2+\csc^2\alpha(r')^2}$, the [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) has the [Beltrami identity](../../../analysis.md#beltrami-identity) because $L$ has no explicit $\theta$ dependence:

$$
L-r'\frac{\partial L}{\partial r'}=\frac{r^2}{L}=C.
$$

For a nonradial minimizing path, $C>0$. Rearranging and integrating gives

$$
(r')^2=\sin^2\alpha\,r^2\left(\frac{r^2}{C^2}-1\right),\qquad \boxed{r\cos\bigl((\theta-\theta_0)\sin\alpha\bigr)=C.}
$$

The endpoint conditions determine $C$ and $\theta_0$ on the selected angular branch.

To verify that this stationary path really minimizes [arc length](../../../riemannian-geometry.md#arc-length), use the [local isometry from a circular cone to the plane](../../../differential-geometry.md#local-isometry-from-a-circular-cone-to-the-plane). Set $s=r/\sin\alpha$ and $\phi=\theta\sin\alpha$; then $ds^2+s^2d\phi^2$ is the plane [metric](../../../topological-analysis.md#metric). The displayed path is a straight line $s\cos(\phi-\phi_0)=C/\sin\alpha$, so its segment realizes the plane distance. Choose endpoint angular lifts with $|\Delta\theta|\leq\pi$; then $|\Delta\phi|<\pi$, and the joining segment avoids the apex. Its length is

$$
\frac1{\sin\alpha}\sqrt{r_1^2+r_2^2-2r_1r_2\cos(\sin\alpha\,\Delta\theta)}.
$$

Other lifts with developed angular difference less than $\pi$ give at least this distance; an angular change of at least $\pi$ has infimum at least $s_1+s_2$, attained only if passage through the apex is allowed. This proves the global choice above. Endpoints on a common generator have the radial segment as shortest path, which is the limiting case omitted by the $r(\theta)$ parametrization. If an endpoint is the apex, its shortest path is a generator. Thus **shortest paths are straight segments after developing the cone**.

## 3E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="3e/a">a</h3>

↑ **Parent:** [3E](#3e)

<h4 id="3e/a/solution">Solution</h4>

↑ **Parent:** [A](#3e/a)

Fix any $z_0\in\mathbb C$. The [Cauchy estimate](../../../analysis.md#cauchy-estimate) on the circle $|z-z_0|=R$ applies for every $R>0$ because $f$ is an [entire function](../../../complex-analysis.md#entire-function). It gives

$$
|f'(z_0)|\leq\frac{\max_{|z-z_0|=R}|f(z)|}{R}\leq\frac{1+\sqrt{|z_0|+R}}R\longrightarrow0.
$$

Therefore $f'(z_0)=0$. Since $z_0$ was arbitrary and $\mathbb C$ is [connected](../../../geometry-and-topology.md#connected-space), **$f$ is constant**. This is the sublinear case of the [polynomial growth theorem for entire functions](../../../complex-analysis.md#polynomial-growth-theorem-for-entire-functions).

<h3 id="3e/b">b</h3>

↑ **Parent:** [3E](#3e)

<h4 id="3e/b/solution">Solution</h4>

↑ **Parent:** [B](#3e/b)

The composition $g(z)=e^{-f(z)}$ is an [entire function](../../../complex-analysis.md#entire-function), and

$$
|g(z)|=e^{-\operatorname{Re}f(z)}\leq1.
$$

By [Liouville's theorem](../../../complex-analysis.md#liouville-theorem), $g$ is constant. Since the [exponential function](../../../calculus.md#exponential-function) never vanishes,

$$
0=g'(z)=-f'(z)e^{-f(z)}\quad\Longrightarrow\quad f'(z)=0.
$$

Thus **$f$ is constant**. Notice that constancy of an exponential alone need not be inverted by choosing a global logarithm; differentiating supplies the conclusion directly.

## 4F

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="4f/solution">Solution</h3>

↑ **Parent:** [4F](#4f)

Let $T$ be the [isometry](../../../riemannian-geometry.md#isometry). Since $T(0)=0$, it preserves [norms](../../../functional-analysis.md#norm), and the [polarization identity](../../../linear-algebra.md#polarization-identity) applied to distances gives $\langle T(x),T(y)\rangle=\langle x,y\rangle$. For an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) $e_1,e_2,e_3$, the vectors $T(e_i)$ are again an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis), and

$$
\langle T(x),T(e_i)\rangle=\langle x,e_i\rangle.
$$

Expanding in that [basis](../../../vector-space.md#basis) proves $T(x)=\sum_i\langle x,e_i\rangle T(e_i)$. Hence $T$ is a [linear map](../../../vector-space.md#linear-map) represented by an [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix) $Q$.

A [reflection in a hyperplane](../../../linear-algebra.md#reflection-in-a-hyperplane) with nonzero normal $v$ is $H_v(x)=x-2\langle x,v\rangle v/\langle v,v\rangle$. If $Qe_1\ne e_1$, choose $v=Qe_1-e_1$. Because $\|Qe_1\|=\|e_1\|$, substitution shows $H_vQe_1=e_1$. If they agree, no [reflection](../../../linear-algebra.md#reflection-mathematics) is needed. The resulting [orthogonal transformation](../../../linear-algebra.md#orthogonal-transformation) fixes $e_1$ and preserves its [orthogonal complement](../../../hilbert-space.md#orthogonal-complement). Apply the same construction there to fix $e_2$; the second normal is perpendicular to $e_1$, so the first vector remains fixed. Finally the restriction to the remaining line is either the identity or negation; in the latter case a third [reflection](../../../linear-algebra.md#reflection-mathematics), normal to $e_3$, fixes it. Reversing these steps writes $Q$ as a product of at most three [reflections](../../../linear-algebra.md#reflection-mathematics), each in a plane through the origin. This proves the three-dimensional case of the [Cartan–Dieudonné theorem](../../../linear-algebra.md#cartan-dieudonne-theorem).

**Three reflections are sometimes necessary.** The map $-I$ is the product of the three coordinate-plane [reflections](../../../linear-algebra.md#reflection-mathematics). Its [determinant](../../../linear-algebra.md#determinant) is $-1$, excluding zero or two [reflections](../../../linear-algebra.md#reflection-mathematics). A single plane [reflection](../../../linear-algebra.md#reflection-mathematics) fixes a two-dimensional [vector subspace](../../../vector-space.md#vector-subspace), whereas $-I$ fixes only zero, excluding one. Thus the bound is sharp.

## 5H

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="5h/solution">Solution</h3>

↑ **Parent:** [5H](#5h)

Player A maximizes the [payoff](../../../game-theory.md#payoff), while B minimizes it. The fourth row is strictly worse for A than the first in every column, so remove $A_4$ by [dominated strategy elimination](../../../game-theory.md#dominated-strategy-elimination). On the remaining rows, column $B_3$ is strictly better for B than $B_2$, so remove $B_2$. Now $A_3$ is strictly worse than $A_2$ in the two remaining columns. The reduced [zero-sum game](../../../game-theory.md#zero-sum-game) has [payoff matrix](../../../game-theory.md#payoff-matrix)

$$
\begin{pmatrix}4&-5\\-2&3\end{pmatrix},
$$

with rows $A_1,A_2$ and columns $B_1,B_3$.

If A uses [mixed strategy](../../../game-theory.md#mixed-strategy) $(p,1-p)$, the expected [payoffs](../../../game-theory.md#payoff) against these columns are $-2+6p$ and $3-8p$. The first increases and the second decreases, so their minimum is maximized where they are equal: $14p=5$. Thus

$$
\boxed{A:\ (5/14,9/14,0,0),\qquad v=1/7.}
$$

For an optimality certificate, B uses [mixed strategy](../../../game-theory.md#mixed-strategy) $(q,0,1-q)$, making A's first two row [payoffs](../../../game-theory.md#payoff) $-5+9q$ and $3-5q$. Equality gives $q=4/7$. Against this B strategy the four row [payoffs](../../../game-theory.md#payoff) are $(1/7,1/7,-6/7,-6/7)$, while against the displayed A strategy the three column [payoffs](../../../game-theory.md#payoff) are $(1/7,13/7,1/7)$. Therefore A guarantees $1/7$ and B holds A to $1/7$, verifying the [value of a zero-sum game](../../../game-theory.md#value-of-a-zero-sum-game) and the original, unreduced [mixed strategy](../../../game-theory.md#mixed-strategy).

## 6B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="6b/a">a</h3>

↑ **Parent:** [6B](#6b)

<h4 id="6b/a/solution">Solution</h4>

↑ **Parent:** [A](#6b/a)

The [Lagrange basis polynomials](../../../numerical-analysis.md#lagrange-cardinal-polynomial) satisfy $\ell_i(x_j)=\delta_{ij}$: for $j\ne i$, the product has a zero factor, whereas for $j=i$ every factor is one. The [polynomial](../../../polynomial.md)

$$
q(x)=p(x)-\sum_{i=0}^np(x_i)\ell_i(x)
$$

has [degree of a polynomial](../../../polynomial.md#degree-of-a-polynomial) at most $n$ and has $n+1$ distinct [roots of a polynomial](../../../polynomial.md#root-of-a-polynomial). The [root bound for a polynomial](../../../polynomial.md#lagrange-root-bound-over-a-field) implies $q=0$. Hence **the interpolation identity holds for every polynomial of degree at most $n$**.

<h3 id="6b/b">b</h3>

↑ **Parent:** [6B](#6b)

<h4 id="6b/b/solution">Solution</h4>

↑ **Parent:** [B](#6b/b)

At a simple [root of a polynomial](../../../polynomial.md#root-of-a-polynomial) $x_i$ of $\omega$, differentiating the product gives $\omega'(x_i)=\prod_{k\ne i}(x_i-x_k)\ne0$. Consequently the [Lagrange basis polynomials](../../../numerical-analysis.md#lagrange-cardinal-polynomial) can be written

$$
\ell_i(x)=\frac{\omega(x)}{(x-x_i)\omega'(x_i)}.
$$

Divide the [polynomial interpolation](../../../numerical-analysis.md#polynomial-interpolation) identity from part (a) by $\omega(x)$, at points outside the nodes. This gives the [partial fraction decomposition](../../../isolated-singularity.md#partial-fraction-decomposition)

$$
\boxed{\frac{p(x)}{\omega(x)}=\sum_{i=0}^n\frac{p(x_i)}{\omega'(x_i)}\frac1{x-x_i}.}
$$

Every denominator of $\omega$ is simple, and the [rational function](../../../isolated-singularity.md#rational-function) is proper because $\deg p<\deg\omega$, so no polynomial part is missing.

## 7G

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="7g/solution">Solution</h3>

↑ **Parent:** [7G](#7g)

For $x\in\ker(\alpha-\lambda I)$, commutation gives

$$
(\alpha-\lambda I)\beta x=\beta(\alpha-\lambda I)x=0.
$$

Thus each [eigenspace](../../../linear-operator-theory.md#eigenspace) of $\alpha$ is an [invariant subspace](../../../representation-theory.md#invariant-subspace) for $\beta$.

If $\alpha=\beta^2$, the two [endomorphisms](../../../algebra.md#endomorphism) commute. The $n$ distinct real [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of $\alpha$ have one-dimensional real [eigenspaces](../../../linear-operator-theory.md#eigenspace), since their direct sum is the $n$-dimensional [vector space](../../../vector-space.md). Take a nonzero real [eigenvector](../../../linear-operator-theory.md#eigenvector) $x_i$. Its [eigenspace](../../../linear-operator-theory.md#eigenspace) is invariant under $\beta$, so $\beta x_i=c_ix_i$ for a real scalar $c_i$. Squaring gives

$$
\lambda_i x_i=\alpha x_i=\beta^2x_i=c_i^2x_i,\qquad \boxed{\lambda_i=c_i^2\geq0.}
$$

The simple-spectrum hypothesis is essential: the real $90$-degree [rotation matrix](../../../linear-algebra.md#rotation-matrix) squares to $-I$ in dimension two, whose negative [eigenvalue](../../../linear-operator-theory.md#eigenvalue) has a two-dimensional [eigenspace](../../../linear-operator-theory.md#eigenspace).

## 8C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="8c/solution">Solution</h3>

↑ **Parent:** [8C](#8c)

With polar unit vectors $\mathbf e_r=(\cos\theta,\sin\theta,0)$ and $\mathbf e_\theta=(-\sin\theta,\cos\theta,0)$, the second term is $\Gamma\mathbf e_\theta/(2\pi r)$. It is tangent to circles, independent of $z$, and has zero [divergence](../../../calculus.md#divergence) and zero [vorticity](../../../fluid-mechanics.md#vorticity) away from the axis. Its singular axis carries a [line vortex](../../../fluid-mechanics.md#line-vortex); adding the constant [velocity field](../../../fluid-mechanics.md#velocity-field) gives a [uniform flow](../../../fluid-mechanics.md#uniform-flow) plus that [line vortex](../../../fluid-mechanics.md#line-vortex).

The counterclockwise [circulation](../../../fluid-mechanics.md#circulation-physics) around a positively oriented loop is $\oint\mathbf u\cdot d\mathbf r$. For a radius-$R$ circle, the [uniform flow](../../../fluid-mechanics.md#uniform-flow) contributes zero and the [line vortex](../../../fluid-mechanics.md#line-vortex) contributes

$$
\oint_{C_R}\frac\Gamma{2\pi R}\mathbf e_\theta\cdot R\mathbf e_\theta\,d\theta=\Gamma.
$$

Any loop winding once around the axis has the same [circulation](../../../fluid-mechanics.md#circulation-physics), by [Stokes theorem](../../../calculus.md#stokes-theorem) in the nonsingular intervening region.

On $C_R$, $\mathbf n=\mathbf e_r$, $\mathbf u\cdot\mathbf n=U\cos\theta$, and $dl=R\,d\theta$. Thus

$$
\oint_{C_R}(\mathbf u\cdot\mathbf n)\mathbf u\,dl=RU^2\mathbf e_x\int_0^{2\pi}\cos\theta\,d\theta+\frac{U\Gamma}{2\pi}\int_0^{2\pi}\cos\theta\,\mathbf e_\theta\,d\theta=\boxed{\frac12\boldsymbol\Gamma\mathbin\times\mathbf U}.
$$

In fact this equality holds for every $R>0$ for the stated field, since the remaining vector [integral](../../../calculus.md#integral) is $(0,\pi,0)$.

This is the advective part of the [momentum flux](../../../physics.md#momentum-flux). To obtain the force, include [pressure](../../../thermodynamics.md#pressure). For steady [irrotational flow](../../../fluid-mechanics.md#irrotational-flow), the [Bernoulli equation](../../../fluid-mechanics.md#bernoulli-equation) gives

$$
p=p_\infty-\frac\rho2(|\mathbf u|^2-U^2)=p_\infty+\frac{\rho U\Gamma\sin\theta}{2\pi R}-\frac{\rho\Gamma^2}{8\pi^2R^2}.
$$

The constant terms integrate to zero against $\mathbf n$; the remaining [pressure](../../../thermodynamics.md#pressure) contribution is $\oint p\mathbf n\,dl=\rho\boldsymbol\Gamma\times\mathbf U/2$. The total outward [momentum flux](../../../physics.md#momentum-flux) plus [pressure](../../../thermodynamics.md#pressure) term is therefore $\rho\boldsymbol\Gamma\times\mathbf U$, the force of the obstacle on the fluid. The opposite force, of fluid on the obstacle per unit span, is

$$
\boxed{\mathbf F=\rho\mathbf U\times\boldsymbol\Gamma.}
$$

This is the [Kutta–Joukowski theorem](../../../fluid-mechanics.md#kutta-joukowski-theorem), with positive $\Gamma$ defined counterclockwise: positive $U$ and $\Gamma$ give force in the negative $y$ direction. For an actual two-dimensional [aerofoil](../../../fluid-mechanics.md#airfoil), faster-decaying far-field terms do not change this limit. **The displayed advective integral supplies half the lift; pressure supplies the other half.**

## 9G

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="9g/solution">Solution</h3>

↑ **Parent:** [9G](#9g)

The [discriminant of a binary quadratic form](../../../number-theory.md#discriminant-of-a-binary-quadratic-form) is $d=b^2-4ac$; it is unchanged by a [unimodular matrix](../../../linear-algebra.md#unimodular-matrix) change of integral variables and satisfies $d\equiv0$ or $1\pmod4$. For such a $d$, the [discriminant criterion for prime representation by a binary quadratic form](../../../number-theory.md#discriminant-criterion-for-prime-representation-by-a-binary-quadratic-form) says that some integral [binary quadratic form](../../../number-theory.md#binary-quadratic-form) of [discriminant of a binary quadratic form](../../../number-theory.md#discriminant-of-a-binary-quadratic-form) $d$ represents an odd [prime](../../../number-theory.md#prime-number) $p$ exactly when $d$ is a square modulo $p$, including zero. Equivalently,

$$
\boxed{\text{there is an integer }B\text{ with }B^2\equiv d\pmod{4p}.}
$$

These versions agree: a square root modulo $p$ can be chosen even when $d\equiv0\pmod4$ and odd when $d\equiv1\pmod4$, by adding $p$ if needed, and then the [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem) applies.

For completeness, if $f(x,y)=p$, then $(x,y)$ is primitive, since any common divisor would have its square divide $p$. Complete $(x,y)$ to a basis of $\mathbb Z^2$ with [determinant](../../../linear-algebra.md#determinant) one using [Bézout's identity](../../../algebra.md#bezout-identity). The transformed [binary quadratic form](../../../number-theory.md#binary-quadratic-form) has leading coefficient $p$ and [discriminant of a binary quadratic form](../../../number-theory.md#discriminant-of-a-binary-quadratic-form) $B^2-4pC=d$. Conversely, a suitable $B$ makes $[p,B,(B^2-d)/(4p)]$ an integral [binary quadratic form](../../../number-theory.md#binary-quadratic-form) representing $p$ at $(1,0)$.

For $x^2+3y^2$, the [discriminant of a binary quadratic form](../../../number-theory.md#discriminant-of-a-binary-quadratic-form) is $-12$. The [prime](../../../number-theory.md#prime-number) $3$ is represented. If $p\ne3$ is represented, reducing modulo $3$ gives $p\equiv x^2\equiv1\pmod3$, which also excludes $p=2$. To prove sufficiency for $p\equiv1\pmod3$, [quadratic reciprocity](../../../number-theory.md#quadratic-reciprocity) gives

$$
\left(\frac{-3}{p}\right)=\left(\frac{-1}{p}\right)\left(\frac3p\right)=\left(\frac p3\right)=1.
$$

The criterion constructs a positive definite [binary quadratic form](../../../number-theory.md#binary-quadratic-form) $[p,B,C]$ of [discriminant of a binary quadratic form](../../../number-theory.md#discriminant-of-a-binary-quadratic-form) $-12$. It is primitive: a common divisor of its coefficients would divide $p$, and if that divisor were $p$, then $p^2$ would divide $12$, impossible for $p\ne2,3$.

We must still establish that this form is equivalent to $x^2+3y^2$, rather than merely some form of the same [discriminant of a binary quadratic form](../../../number-theory.md#discriminant-of-a-binary-quadratic-form). In a positive definite integral [binary quadratic form](../../../number-theory.md#binary-quadratic-form), replace $x$ by $x+ky$ to arrange $|b|\leq a$. If $c<a$, apply $(x,y)\mapsto(-y,x)$ and repeat. Each such exchange strictly decreases the positive integer leading coefficient, so this [reduction algorithm for a positive definite binary quadratic form](../../../number-theory.md#reduction-algorithm-for-a-positive-definite-binary-quadratic-form) terminates with $|b|\leq a\leq c$. Then $12=4ac-b^2\geq3a^2$, so $a\leq2$. With $a=1$, parity forces $b=0$, giving $c=3$. With $a=2$, the only integral choices are $b=\pm2,c=2$, and these are not primitive. Thus every primitive positive definite [binary quadratic form](../../../number-theory.md#binary-quadratic-form) of [discriminant of a binary quadratic form](../../../number-theory.md#discriminant-of-a-binary-quadratic-form) $-12$ is equivalent to $[1,0,3]$, and preserves its represented integers. Therefore

$$
\boxed{p=x^2+3y^2\text{ for integers }x,y\quad\Longleftrightarrow\quad p=3\text{ or }p\equiv1\pmod3.}
$$

## 10A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="10a/solution">Solution</h3>

↑ **Parent:** [10A](#10a)

A [photon](../../../quantum-mechanics.md#photon) of [wavelength](../../../wave-equation.md#wavelength) $\lambda$ has [energy](../../../classical-mechanics.md#energy) $E=h\nu=hc/\lambda$ and [momentum](../../../classical-mechanics.md#momentum) $\mathbf p=(h/\lambda)\hat{\mathbf n}$ along its propagation direction.

The specified [Compton scattering](../../../physics.md#compton-scattering) formula requires the electron to be initially at rest in the frame where the wavelengths and angle are measured. This initial-rest assumption is implicit in the printed request; it is not valid for arbitrary initial electron [momentum](../../../classical-mechanics.md#momentum). Use [four-momentum](../../../special-relativity.md#four-momentum) with [Minkowski metric](../../../special-relativity.md#minkowski-metric) signature $(+---)$: initially $P=(mc,\mathbf0)$, while $K=(E/c,(E/c)\hat{\mathbf n})$ and $K'=(E'/c,(E'/c)\hat{\mathbf n}')$ are null. Conservation gives $P'=P+K-K'$, and the outgoing electron satisfies the same [mass-shell condition](../../../string-theory.md#string-mass-shell-condition) $P'^2=P^2=m^2c^2$. Hence

$$
P\cdot(K-K')=K\cdot K',\qquad m(E-E')=\frac{EE'}{c^2}(1-\cos\theta).
$$

After dividing by $EE'$ and substituting the [photon](../../../quantum-mechanics.md#photon) [energy](../../../classical-mechanics.md#energy) relation,

$$
\frac1{E'}-\frac1E=\frac{1-\cos\theta}{mc^2},\qquad \boxed{\lambda'-\lambda=\frac h{mc}(1-\cos\theta).}
$$

The scale $h/(mc)$ is the electron [Compton wavelength](../../../physics.md#compton-wavelength). For a moving initial electron, the earlier invariant identity remains valid, but $P\cdot K$ includes its initial velocity and the wavelength shift is different.

## 11F

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="11f/solution">Solution</h3>

↑ **Parent:** [11F](#11f)

The [contraction mapping theorem](../../../analysis.md#contraction-mapping-theorem) states that a [contraction mapping](../../../analysis.md#contraction-mapping) $f$ of a nonempty [complete metric space](../../../topological-analysis.md#complete-metric-space) into itself has a unique [fixed point](../../../function.md#fixed-point). More explicitly, if $d(f(x),f(y))\leq qd(x,y)$ with $0\leq q<1$, iteration from any $x_0$ converges to that [fixed point](../../../function.md#fixed-point).

To prove this, put $x_{n+1}=f(x_n)$. Induction gives $d(x_{n+1},x_n)\leq q^nd(x_1,x_0)$, so for $m>n$ the [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives

$$
d(x_m,x_n)\leq\sum_{j=n}^{m-1}q^jd(x_1,x_0)\leq\frac{q^n}{1-q}d(x_1,x_0).
$$

Thus $(x_n)$ is a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence), and [completeness](../../../topological-analysis.md#completeness) supplies a limit $x_*$. A [contraction mapping](../../../analysis.md#contraction-mapping) is [continuous](../../../calculus.md#continuous-function), so $f(x_*)=\lim f(x_n)=\lim x_{n+1}=x_*$. Two [fixed points](../../../function.md#fixed-point) satisfy $d(x_*,y_*)\leq qd(x_*,y_*)$, forcing equality of the points. Passing to the limit in the bound also gives the useful error estimate $d(x_n,x_*)\leq q^nd(x_1,x_0)/(1-q)$.

For the function space, take $X$ nonempty; otherwise the supremum in the printed definition is undefined without a convention. Boundedness of $X$ makes the [uniform metric](../../../topological-analysis.md#uniform-metric) $\rho(f,g)$ finite. Nonnegativity and symmetry follow from $d$; $\rho(f,g)=0$ means $f(x)=g(x)$ at every $x$. Taking suprema in $d(f(x),h(x))\leq d(f(x),g(x))+d(g(x),h(x))$ proves the [triangle inequality](../../../topological-analysis.md#triangle-inequality). Hence $\rho$ is a [metric](../../../topological-analysis.md#metric).

Suppose $(f_n)$ is a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) for this [uniform metric](../../../topological-analysis.md#uniform-metric). At each $x$, $d(f_n(x),f_m(x))\leq\rho(f_n,f_m)$, so [completeness](../../../topological-analysis.md#completeness) of $X$ supplies a value $f(x)=\lim_n f_n(x)$. Given $\varepsilon>0$, choose $N$ with $\rho(f_n,f_m)<\varepsilon/2$ for all $n,m\geq N$. Fix $n\geq N$ and let $m\to\infty$ pointwise; then $d(f_n(x),f(x))\leq\varepsilon/2$ for every $x$. Thus $\rho(f_n,f)\leq\varepsilon/2<\varepsilon$. The [uniform limit theorem](../../../real-analysis.md#uniform-limit-theorem) makes this limit continuous, so $f\in F$. This proves the [completeness of the continuous-map space in the uniform metric](../../../topological-analysis.md#completeness-of-the-continuous-map-space-in-the-uniform-metric).

Finally fix $f\in C$ with contraction constant $q_f<1$, and write $x_f=\theta(f)$ and $x_g=\theta(g)$. Using the [fixed point](../../../function.md#fixed-point) equations,

$$
d(x_g,x_f)\leq d(g(x_g),f(x_g))+d(f(x_g),f(x_f))\leq\rho(f,g)+q_fd(x_g,x_f).
$$

Therefore the [fixed-point stability in the uniform metric](../../../analysis.md#fixed-point-stability-in-the-uniform-metric) estimate is

$$
\boxed{d(\theta(g),\theta(f))\leq\frac{\rho(f,g)}{1-q_f}.}
$$

Choosing $\rho(f,g)<(1-q_f)\varepsilon$ proves **continuity of $\theta$ at every $f$**. The estimate uses the constant of the fixed map $f$ only; it does not require a common contraction constant for all nearby $g$.

## 12D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="12d/a">a</h3>

↑ **Parent:** [12D](#12d)

<h4 id="12d/a/solution">Solution</h4>

↑ **Parent:** [A](#12d/a)

Assume the impulse point is in the interior, $0<a<l$. Expand the displacement in the fixed-end [Fourier sine series](../../../fourier-series.md#fourier-sine-series)

$$
y(x,t)=\sum_{n=1}^{\infty}T_n(t)\sin\frac{n\pi x}{l},\qquad \alpha_n=\frac{n\pi c}{l}.
$$

[Orthogonality](../../../linear-algebra.md#orthogonal-vectors) gives the initial velocity coefficient by applying the [Dirac delta](../../../distribution-theory.md#dirac-delta-function) to the sine function:

$$
T_n(0)=0,\qquad T_n'(0)=\frac2l\int_0^l\delta(x-a)\sin\frac{n\pi x}{l}\,dx=\frac2l\sin\frac{n\pi a}{l}.
$$

Substitution in the [wave equation](../../../wave-equation.md) yields $T_n''+2kT_n'+\alpha_n^2T_n=0$. For $k<\alpha_n$, its roots are $-k\pm i\omega_n$, where $\omega_n=\sqrt{\alpha_n^2-k^2}$. The two initial conditions determine

$$
T_n(t)=\frac2l\sin\frac{n\pi a}{l}\,e^{-kt}\frac{\sin(\omega_nt)}{\omega_n}.
$$

Hence the normalized [velocity-impulse Green function for a damped string](../../../wave-equation.md#velocity-impulse-green-function-for-a-damped-string) is

$$
\boxed{y(x,t)=\frac2l\sum_{n=1}^{\infty}\sin\frac{n\pi a}{l}\sin\frac{n\pi x}{l}\,e^{-kt}\frac{\sin\bigl(\sqrt{\alpha_n^2-k^2}\,t\bigr)}{\sqrt{\alpha_n^2-k^2}}.}
$$

For a mode with [critical damping](../../../wave-equation.md#critical-damping), use the limit $e^{-kt}t$ in place of the time factor. For $k>\alpha_n$, put $\eta_n=\sqrt{k^2-\alpha_n^2}$ and use $e^{-kt}\sinh(\eta_nt)/\eta_n$. These choices solve the same modal [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) and initial conditions, so the formula covers arbitrary $k>0$. The impulse initial velocity is a [distribution](../../../distribution-theory.md#distribution-mathematical-analysis), so initial differentiation of the [series](../../../real-analysis.md#series-mathematics) is interpreted distributionally.

**The printed formula requires correction:** the factor depending on $n$ must lie inside the sum, and sine-mode normalization requires $2/l$, rather than $2$. The printed slash after the final sine is also stray. Direct differentiation at $t=0$ verifies the corrected normalization: the initial sine coefficients are exactly those of $\delta(x-a)$.

<h3 id="12d/b">b</h3>

↑ **Parent:** [12D](#12d)

<h4 id="12d/b/solution">Solution</h4>

↑ **Parent:** [B](#12d/b)

A mode has dimensionless damping ratio $k/\alpha_n$, and characteristic roots

$$
s_\pm=-k\pm\sqrt{k^2-\alpha_n^2}.
$$

If $k/\alpha_n\ll1$, the [normal mode](../../../wave-equation.md#normal-mode) oscillates at $\omega_n=\alpha_n+O(k^2/\alpha_n)$ with exponentially decaying envelope $e^{-kt}$. As $k\to0$, the solution approaches the undamped [wave equation](../../../wave-equation.md) response.

If $k/\alpha_n\gg1$, the roots are real and negative, with

$$
s_+=-\frac{\alpha_n^2}{2k}+O(\alpha_n^4/k^3),\qquad s_-=-2k+\frac{\alpha_n^2}{2k}+O(\alpha_n^4/k^3).
$$

The mode has a fast transient and a slow nonoscillatory relaxation. After the fast transient, neglecting $y_{tt}$ gives the [diffusion equation](../../../diffusion-equation.md) $y_t\simeq c^2y_{xx}/(2k)$ for these long-wavelength modes. At $k=\alpha_n$, the repeated root produces $te^{-kt}$: this is [critical damping](../../../wave-equation.md#critical-damping).

Thus **the critical parameter is $k/\alpha_n=1$ for each mode**, and the fundamental threshold is

$$
\boxed{\frac{kl}{\pi c}=1.}
$$

When $k<\pi c/l$ every mode is oscillatory. For any fixed, finite $k$, sufficiently large $n$ still gives oscillatory modes, so large damping of the lowest modes does not mean that every mode of the full string is overdamped.

## 13E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="13e/a">a</h3>

↑ **Parent:** [13E](#13e)

<h4 id="13e/a/solution">Solution</h4>

↑ **Parent:** [A](#13e/a)

The complex [Taylor series](../../../calculus.md#taylor-series) theorem states that if $f$ is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) in $|z-z_0|<R$, then

$$
\boxed{f(z)=\sum_{n=0}^{\infty}\frac{f^{(n)}(z_0)}{n!}(z-z_0)^n\quad (|z-z_0|<R).}
$$

The [power series](../../../real-analysis.md#power-series) converges absolutely there and uniformly on each smaller closed disc; its coefficients are unique. For $|z-z_0|<r<R$, the [Cauchy integral formula](../../../analysis.md#cauchy-integral-formula) also gives $f^{(n)}(z_0)/n!=(2\pi i)^{-1}\int_{|\zeta-z_0|=r}f(\zeta)(\zeta-z_0)^{-n-1}\,d\zeta$. This is the analytic, rather than finite real-variable, form of [Taylor theorem](../../../calculus.md#taylor-theorem) relevant here.

<h3 id="13e/b">b</h3>

↑ **Parent:** [13E](#13e)

<h4 id="13e/b/solution">Solution</h4>

↑ **Parent:** [B](#13e/b)

Let $h=f-g$, whose [power series](../../../real-analysis.md#power-series) coefficients are $c_n=a_n-b_n$. Suppose some coefficient is nonzero, and let $N$ be the least such index. Inside the common convergence disc,

$$
h(z)=(z-z_0)^N\left(c_N+\sum_{j=1}^{\infty}c_{N+j}(z-z_0)^j\right).
$$

The parenthesized [analytic function](../../../complex-analysis.md#space-of-holomorphic-functions) tends to $c_N\ne0$ as $z\to z_0$, so it does not vanish in some neighborhood. Hence $h$ has no [zeros](../../../polynomial.md#zero-of-a-function) sufficiently near $z_0$ except possibly $z_0$ itself. This contradicts $h(z_k)=0$ with $z_k\ne z_0$ and $z_k\to z_0$. Thus **all coefficients agree**:

$$
\boxed{a_n=b_n\quad\text{for every }n\geq0.}
$$

This also proves the local isolation of [zeros](../../../polynomial.md#zero-of-a-function) of a nonzero [analytic function](../../../complex-analysis.md#space-of-holomorphic-functions).

<h3 id="13e/c">c</h3>

↑ **Parent:** [13E](#13e)

<h4 id="13e/c/solution">Solution</h4>

↑ **Parent:** [C](#13e/c)

Put $h=f-g$. Choose a disc about $z_0$ contained in the [domain](../../../topology.md#domain-mathematical-analysis) $D$. Part (a) gives a convergent [Taylor series](../../../calculus.md#taylor-series) there, and the accumulating [zeros](../../../polynomial.md#zero-of-a-function) together with part (b) force all its coefficients to vanish. Thus $h=0$ near $z_0$.

To propagate this to the entire [domain](../../../topology.md#domain-mathematical-analysis), define

$$
S=\{z\in D:h^{(n)}(z)=0\text{ for every }n\geq0\}.
$$

The set is nonempty by the preceding local argument. Each derivative is [continuous](../../../calculus.md#continuous-function), so $S$ is closed relative to $D$ as the intersection of their zero sets. If $z\in S$, its [Taylor series](../../../calculus.md#taylor-series) is zero on a disc about $z$, and all derivatives vanish throughout that disc; hence $S$ is open relative to $D$. [Connectedness](../../../geometry-and-topology.md#connected-space) forces $S=D$. Therefore **$f=g$ throughout $D$**, proving the [identity theorem for holomorphic functions](../../../complex-analysis.md#identity-theorem) rather than merely invoking it.

<h3 id="13e/d">d</h3>

↑ **Parent:** [13E](#13e)

<h4 id="13e/d/solution">Solution</h4>

↑ **Parent:** [D](#13e/d)

Take the [analytic function](../../../complex-analysis.md#space-of-holomorphic-functions)

$$
\boxed{f(z)=\sin(\pi/z)\quad\text{on }\mathbb C\setminus\{0\}.}
$$

It vanishes at $z=1/n$ for every positive integer $n$, but $f(2)=1$, so it is not identically zero. The [identity theorem](../../../complex-analysis.md#identity-theorem) does not apply at the accumulation point $0$, because that point lies outside the [domain](../../../topology.md#domain-mathematical-analysis).

<h3 id="13e/e">e</h3>

↑ **Parent:** [13E](#13e)

<h4 id="13e/e/solution">Solution</h4>

↑ **Parent:** [E](#13e/e)

Let $f$ have the stated [zeros](../../../polynomial.md#zero-of-a-function) but not be identically zero. The origin is an [isolated singularity](../../../isolated-singularity.md). If it were a [removable singularity](../../../isolated-singularity.md#removable-singularity), the extended [holomorphic function](../../../complex-analysis.md#holomorphic-function) would have [zeros](../../../polynomial.md#zero-of-a-function) accumulating at an interior point. The proof in part (c) would force the extension, and then $f$ on its [domain](../../../topology.md#domain-mathematical-analysis), to be identically zero.

If the origin were a [pole](../../../isolated-singularity.md#pole) of order $m$, then $g(z)=z^mf(z)$ would have a [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) extension with $g(0)\ne0$. [Continuity](../../../calculus.md#continuous-function) would make $g$ nonzero on a small disc, so $f$ would have no [zeros](../../../polynomial.md#zero-of-a-function) in its punctured disc, again a contradiction. The classification of [isolated singularities](../../../isolated-singularity.md) leaves only an **essential singularity at the origin**. This argument applies to every function in part (d), not just the particular sine example.

## 14F

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="14f/solution">Solution</h3>

↑ **Parent:** [14F](#14f)

Work first on the unit [sphere](../../../geometry-and-topology.md#sphere). A [spherical lune](../../../geometry-and-topology.md#spherical-lune) of angle $\alpha$ has area $2\alpha$: its fraction of sphere area is $\alpha/(2\pi)$. The three [great circles](../../../geometry-and-topology.md#great-circle) extending the sides of a nondegenerate [spherical triangle](../../../geometry-and-topology.md#spherical-triangle) divide the sphere into four antipodal pairs of triangular regions. Call the desired region $T$, of area $A$, and its three adjacent regions $T_1,T_2,T_3$, of areas $A_1,A_2,A_3$. These four regions contain one region from each antipodal pair, so $A+A_1+A_2+A_3=2\pi$. The lune at each vertex consists of $T$ and one of these adjacent regions. Therefore, if the three interior angles are $\alpha,\beta,\gamma$,

$$
2(\alpha+\beta+\gamma)=3A+A_1+A_2+A_3=2A+2\pi,
$$

which proves the [spherical excess formula](../../../differential-geometry.md#spherical-excess-formula), the spherical-triangle form of the [Gauss-Bonnet theorem](../../../differential-geometry.md#gauss-bonnet-theorem):

$$
\boxed{A=\alpha+\beta+\gamma-\pi.}
$$

For a sphere of radius $s$, multiply this area by $s^2$.

Triangulate a convex spherical $n$-gon by diagonals from a vertex. There are $n-2$ [spherical triangles](../../../geometry-and-topology.md#spherical-triangle), and their angles add to the polygon's interior angle sum. Thus its unit-sphere area is

$$
\boxed{A=\sum_{i=1}^n\alpha_i-(n-2)\pi.}
$$

For a nondegenerate convex regular polygon in an [open hemisphere](../../../geometry-and-topology.md#open-hemisphere), area is positive and each angle is less than $\pi$, giving $(n-2)\pi/n<\alpha<\pi$. Every angle in this interval occurs. Indeed place $n$ vertices at equal longitude spacings and colatitude $t\in(0,\pi/2)$ about a pole, and join consecutive vertices by shorter [great circle](../../../geometry-and-topology.md#great-circle) arcs. The polygon is convex and regular. Split a central isosceles [spherical triangle](../../../geometry-and-topology.md#spherical-triangle) along the perpendicular to its edge. The resulting right [spherical triangle](../../../geometry-and-topology.md#spherical-triangle) has angles $\pi/n$, $\alpha/2$, $\pi/2$, and hypotenuse $t$. The angular [spherical law of cosines](../../../geometry-and-topology.md#spherical-law-of-cosines) yields

$$
0=-\cos(\pi/n)\cos(\alpha/2)+\sin(\pi/n)\sin(\alpha/2)\cos t,
$$

so $\cot(\alpha/2)=\cos t\tan(\pi/n)$. As $t$ increases from $0$ to $\pi/2$, $\alpha$ increases continuously through exactly

$$
\boxed{\frac{n-2}{n}\pi<\alpha<\pi,\qquad n\geq3.}
$$

The endpoints are degenerate limits, not strict convex polygons.

For the [spherical triangle reflection group](../../../geometry-and-topology.md#spherical-triangle-reflection-group), positive area requires $1/p+1/q+1/r>1$. Each angle is less than $\pi$, so the integer denominators are at least two. Arrange $p\leq q\leq r$. If $p\geq3$ the sum is at most one, hence $p=2$. If $q\geq4$ the sum is again at most one; thus either $q=2$ and any $r\geq2$ works, or $q=3$ and $r=3,4,5$. These triangles exist, for example as the reflection chambers of a regular dihedral configuration, tetrahedron, cube, and dodecahedron, respectively.

To count group elements using the assumed [tessellation](../../../geometry-and-topology.md#tessellation), first label the original triangle's three vertices by their types and propagate these labels through side [reflections](../../../linear-algebra.md#reflection-mathematics). Around a type-$p$ vertex there are $2p$ sectors; the associated alternating reflections make a full turn and return the labels unchanged. The same holds at the other types. Every closed path in the dual tessellation is generated by these circuits around vertices, since the sphere is [simply connected](../../../algebraic-topology.md#simply-connected-space). Thus the labels are globally consistent, including when two angle denominators coincide. Every generated [isometry](../../../riemannian-geometry.md#isometry) preserves these labels. An element stabilizing a triangle therefore fixes its three vertices and is the identity. Consequently group elements correspond bijectively to triangles, and area gives

$$
|G|=\frac{4\pi}{\pi(1/p+1/q+1/r-1)}.
$$

The possibilities, including permutations of the entries, are

$$
\boxed{\begin{array}{c|c}(p,q,r)&|G|\\\hline(2,2,n),\ n\geq2&4n\\(2,3,3)&24\\(2,3,4)&48\\(2,3,5)&120\end{array}}.
$$

Here is an explicit [dodecahedron](../../../geometry-and-topology.md#dodecahedron) construction for the last case, avoiding an assumption about which vertices of the tessellation to join. Put $\varphi=(1+\sqrt5)/2$, and take the [convex hull](../../../mathematical-optimization.md#convex-hull) of the twenty points

$$
(\pm1,\pm1,\pm1),\quad (0,\pm\varphi^{-1},\pm\varphi),\quad(\pm\varphi^{-1},\pm\varphi,0),\quad(\pm\varphi,0,\pm\varphi^{-1}),
$$

with independent signs. They all have squared radius three. The supporting plane $\varphi y+z=\varphi^2$ contains the five vertices

$$
(1,1,1),\ (\varphi^{-1},\varphi,0),\ (-\varphi^{-1},\varphi,0),\ (-1,1,1),\ (0,\varphi^{-1},\varphi)
$$

in cyclic order. Consecutive distances are $2/\varphi$, and nonconsecutive distances are $2$, so this is a regular pentagon. Changing the two signs in its normal $(0,\varphi,1)$ and cyclically permuting coordinates gives twelve supporting planes, all with a congruent pentagon. Each listed vertex lies on three of these faces; the sixty face-edge incidences pair into thirty edges. The faces form a closed convex polyhedral surface with $20-30+12=2$, hence exhaust the boundary of the [convex hull](../../../mathematical-optimization.md#convex-hull). This constructs a regular [dodecahedron](../../../geometry-and-topology.md#dodecahedron).

Choose the spherical directions of a face center $F=(0,\varphi,1)$, the midpoint $M=(0,\varphi,0)$ of its edge between $(\pm\varphi^{-1},\varphi,0)$, and that edge's endpoint $V=(\varphi^{-1},\varphi,0)$. Normalize these to the unit sphere. The three side planes of triangle $FMV$ are $x=0$, $z=0$, and $\mathbf n\cdot\mathbf x=0$ with $\mathbf n=(-\varphi,\varphi^{-1},-1)$. Their [reflections](../../../linear-algebra.md#reflection-mathematics) are coordinate sign changes in the first two cases and

$$
H(\mathbf x)=\mathbf x-\frac12(\mathbf n\cdot\mathbf x)\mathbf n
$$

in the third, since $\|\mathbf n\|^2=4$. Substitution in the twenty listed vertices, using $\varphi^2=\varphi+1$, shows that all three [reflections](../../../linear-algebra.md#reflection-mathematics) permute the vertex set. The side-plane angles give interior angles $\pi/2$ at $M$, $\pi/3$ at $V$, and $\pi/5$ at $F$ because $|n_z|/\|\mathbf n\|=1/2$ and $|n_x|/\|\mathbf n\|=\varphi/2=\cos(\pi/5)$. Thus this triangle is congruent to $\Delta$, and its side-generated group is $G$, conjugated by the aligning [isometry](../../../riemannian-geometry.md#isometry).

<a id="14f/image-regular-dodecahedron-and-its-face-center-edge-midpoint-vertex-spherical-reflection-chamber"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-3-dodecahedron.png)

**[Figure 1](#14f/image-regular-dodecahedron-and-its-face-center-edge-midpoint-vertex-spherical-reflection-chamber). Regular dodecahedron and its face-center, edge-midpoint, vertex spherical reflection chamber**.

It already has $120$ elements. Conversely, a symmetry of the [dodecahedron](../../../geometry-and-topology.md#dodecahedron) is determined by the image of one face, one vertex on that face, and the orientation along its boundary: there are at most $12\cdot5\cdot2=120$ choices. An [isometry](../../../riemannian-geometry.md#isometry) fixing these choices fixes that face pointwise and must preserve the polyhedron's interior side, hence is the identity. Therefore **the complete symmetry group of the constructed dodecahedron is $G$**, including orientation-reversing symmetries.

## 15H

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="15h/solution">Solution</h3>

↑ **Parent:** [15H](#15h)

A balanced [transportation problem](../../../mathematical-optimization.md#transportation-problem) chooses nonnegative shipments $x_{ij}$ minimizing $\sum_{ij}c_{ij}x_{ij}$, subject to $\sum_jx_{ij}=s_i$ and $\sum_ix_{ij}=d_j$, where the total supply equals total demand. For multipliers $u_i,v_j$, its [Lagrangian](../../../calculus-of-variations.md#lagrangian) is

$$
\mathcal L=\sum_{ij}c_{ij}x_{ij}+\sum_i u_i\left(s_i-\sum_jx_{ij}\right)+\sum_jv_j\left(d_j-\sum_ix_{ij}\right)=\sum_i u_is_i+\sum_jv_jd_j+\sum_{ij}(c_{ij}-u_i-v_j)x_{ij}.
$$

Taking its infimum over $x_{ij}\geq0$ produces the [linear programming duality](../../../mathematical-optimization.md#linear-programming-duality) problem of maximizing $\sum_i u_is_i+\sum_jv_jd_j$ subject to $u_i+v_j\leq c_{ij}$. These are the [transportation dual potentials](../../../mathematical-optimization.md#transportation-dual-potentials).

The [transportation simplex algorithm](../../../mathematical-optimization.md#transportation-simplex-algorithm) starts with a feasible [transportation spanning tree](../../../mathematical-optimization.md#transportation-spanning-tree) of $m+n-1$ basic entries, obtainable by filling the north-west available cell with the smaller remaining supply or demand. Set $u_i+v_j=c_{ij}$ on basic cells; this determines all potentials up to adding a constant to all $u_i$ and subtracting it from all $v_j$. If all nonbasic reduced costs $r_{ij}=c_{ij}-u_i-v_j$ are nonnegative, feasibility and the dual bound prove optimality. Otherwise let a negative-cost cell enter. It closes a unique cycle in the basic tree. Alternate additions and subtractions around that cycle and choose the largest amount preserving nonnegativity, namely the minimum shipment on the subtraction cells. A cell that reaches zero leaves the basis. The cost changes by the entering reduced cost times the pivot amount. Zero basic cells and an anti-cycling rule can handle degeneracy; all pivots below are nondegenerate.

The north-west initial shipment matrix is

$$
X_0=\begin{pmatrix}14&22&0\\0&46&38\\0&0&40\end{pmatrix},\qquad C_0=1156.
$$

With $u_1=0$, its [transportation dual potentials](../../../mathematical-optimization.md#transportation-dual-potentials) are $u=(0,1,0)$ and $v=(5,9,5)$. The most negative reduced cost is $r_{32}=-7$. The cycle is $+(3,2),-(3,3),+(2,3),-(2,2)$; the pivot amount is $\min(40,46)=40$. Hence

$$
X_1=\begin{pmatrix}14&22&0\\0&6&78\\0&40&0\end{pmatrix},\qquad C_1=1156-7\cdot40=876.
$$

Now $u=(0,1,-7)$ and $v=(5,9,5)$. Enter $(1,3)$, of reduced cost $-4$, on cycle $+(1,3),-(1,2),+(2,2),-(2,3)$. The amount is $\min(22,78)=22$, giving

$$
X_2=\begin{pmatrix}14&0&22\\0&28&56\\0&40&0\end{pmatrix},\qquad C_2=876-4\cdot22=788.
$$

The new potentials are $u=(0,5,-3)$ and $v=(5,5,1)$. Enter $(2,1)$, of reduced cost $-7$, on cycle $+(2,1),-(1,1),+(1,3),-(2,3)$. The amount is $\min(14,56)=14$. Thus

$$
\boxed{X_* =\begin{pmatrix}0&0&36\\14&28&42\\0&40&0\end{pmatrix},\qquad C_*=788-7\cdot14=690.}
$$

To certify optimality in the original [transportation problem](../../../mathematical-optimization.md#transportation-problem), take $u=(0,5,-3)$ and $v=(-2,5,1)$. Their entire reduced-cost matrix is

$$
(c_{ij}-u_i-v_j)=\begin{pmatrix}7&4&0\\0&0&0\\12&0&7\end{pmatrix}\geq0.
$$

They satisfy [dual feasibility](../../../mathematical-optimization.md#dual-feasibility), and their value is $5\cdot84-3\cdot40-2\cdot14+5\cdot68+78=690$, equal to the shipment cost. **The minimum transportation cost is therefore $690$**, with no unproved optimality assertion from the iterations alone.

## 16B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="16b/a">a</h3>

↑ **Parent:** [16B](#16b)

<h4 id="16b/a/solution">Solution</h4>

↑ **Parent:** [A](#16b/a)

Repeated differentiation of the [Gaussian function](../../../calculus.md#gaussian-function) gives $D^ne^{-x^2}=P_n(x)e^{-x^2}$, where $P_0=1$ and $P_{n+1}=P_n'-2xP_n$. Induction shows $P_n$ has [degree of a polynomial](../../../polynomial.md#degree-of-a-polynomial) $n$ and leading coefficient $(-2)^n$: the differentiated term has lower degree, while multiplication by $-2x$ raises it by one. Thus the [Hermite polynomial](../../../numerical-analysis.md#hermite-polynomial) $H_n=(-1)^nP_n$ has **degree $n$ and leading coefficient $2^n$**.

For $m<n$, apply [integration by parts](../../../calculus.md#integration-by-parts) $n$ times to the Rodrigues expression:

$$
\int_{-\infty}^{\infty}H_nH_m e^{-x^2}\,dx=(-1)^n\int_{-\infty}^{\infty}H_m D^ne^{-x^2}\,dx=\int_{-\infty}^{\infty}H_m^{(n)}e^{-x^2}\,dx=0.
$$

All boundary terms vanish because each derivative of $e^{-x^2}$ is a [polynomial](../../../polynomial.md) times that exponential, and such products tend to zero at either infinity. The same result for $m>n$ follows by symmetry of the [inner product](../../../linear-algebra.md#inner-product). The diagonal value is positive; indeed $H_n^{(n)}=2^nn!$ gives

$$
\boxed{(H_n,H_m)=2^nn!\sqrt\pi\,\delta_{nm}.}
$$

This proves the requested [orthogonality](../../../linear-algebra.md#orthogonal-vectors) as well as its normalization.

<h3 id="16b/b">b</h3>

↑ **Parent:** [16B](#16b)

<h4 id="16b/b/solution">Solution</h4>

↑ **Parent:** [B](#16b/b)

Differentiating the Rodrigues representation directly gives the identity

$$
H_{n+1}=2xH_n-H_n'.
$$

We prove simultaneously by [induction](../../../foundations-of-mathematics.md#mathematical-induction) that $H_n'=2nH_{n-1}$ for $n\geq1$. It holds for $H_0=1$, $H_1=2x$. Suppose it holds at $n$. Differentiating the preceding identity and using the same identity at $n-1$ gives

$$
\begin{aligned}
H_{n+1}'&=2H_n+2xH_n'-H_n''\\
&=2H_n+4nxH_{n-1}-2nH_{n-1}'\\
&=2H_n+4nxH_{n-1}-2n(2xH_{n-1}-H_n)=2(n+1)H_n.
\end{aligned}
$$

The induction is complete. Substituting the derivative identity into the first formula proves the [Hermite polynomial](../../../numerical-analysis.md#hermite-polynomial) three-term [recurrence relation](../../../real-analysis.md#recurrence-relation)

$$
\boxed{H_{n+1}(x)=2xH_n(x)-2nH_{n-1}(x)\quad(n\geq1).}
$$

The initial step $H_1=2xH_0$ supplies the recurrence at $n=0$ without needing to define $H_{-1}$.

## 17G

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="17g/solution">Solution</h3>

↑ **Parent:** [17G](#17g)

Use the Leibniz definition of the [determinant](../../../linear-algebra.md#determinant):

$$
\det A=\sum_{\pi\in S_n}\operatorname{sgn}(\pi)\prod_{i=1}^na_{i,\pi(i)}.
$$

For the permuted-column [matrix](../../../vector-space.md#matrix), $a^\sigma_{ij}=a_{i,\sigma(j)}$. Reindex the sum by $\tau=\sigma\circ\pi$. The [sign of a permutation](../../../finite-group-theory.md#sign-of-a-permutation) is multiplicative, so $\operatorname{sgn}(\pi)=\operatorname{sgn}(\sigma)\operatorname{sgn}(\tau)$. It follows directly that

$$
\det(A^\sigma)=\operatorname{sgn}(\sigma)\det A.
$$

For the [matrix transpose](../../../vector-space.md#transpose), the products in its determinant are $\prod_i a_{\pi(i),i}$. Set $j=\pi(i)$ to obtain $\prod_j a_{j,\pi^{-1}(j)}$, and use $\operatorname{sgn}(\pi^{-1})=\operatorname{sgn}(\pi)$. This proves $\det(A^t)=\det A$. These facts also show that equal columns, or equal rows by transposition, force the [determinant](../../../linear-algebra.md#determinant) to be zero: exchanging the equal pair leaves the matrix unchanged but changes the determinant's sign.

Let $M_{ij}$ be the [matrix](../../../vector-space.md#matrix) obtained by deleting row $i$ and column $j$, with the empty determinant taken as one for $n=1$. Define the cofactor $C_{ij}=(-1)^{i+j}\det M_{ij}$ and the [adjugate matrix](../../../linear-algebra.md#adjugate-matrix) by $\operatorname{adj}(A)_{ij}=C_{ji}$. Grouping the Leibniz sum according to the column chosen in row $i$ gives the cofactor expansion $\det A=\sum_k a_{ik}C_{ik}$: deleting that row and its chosen column leaves a permutation of $n-1$ entries, with sign factor $(-1)^{i+k}$. Therefore

$$
(A\operatorname{adj}A)_{ij}=\sum_k a_{ik}C_{jk}.
$$

When $i=j$ this is $\det A$. When $i\ne j$ it is the cofactor expansion along row $j$ of the matrix formed by replacing that row with row $i$; its remaining minors are unchanged, and its two equal rows give determinant zero. The column version proves the other product in the same way. Thus the [adjugate identity](../../../linear-algebra.md#adjugate-identity) is

$$
\boxed{A\operatorname{adj}(A)=\operatorname{adj}(A)A=(\det A)I,\qquad A^{-1}=\frac{\operatorname{adj}(A)}{\det A}\quad(\det A\ne0).}
$$

For the real [matrices](../../../vector-space.md#matrix) $C,D$, let $p(t)=\det(C+tD)$. The determinant definition makes this a real [polynomial](../../../polynomial.md) of [degree of a polynomial](../../../polynomial.md#degree-of-a-polynomial) at most $n$. Since $C+iD$ is invertible, the allowed converse implies $p(i)\ne0$, so $p$ is not the zero polynomial. It has at most $n$ real [roots of a polynomial](../../../polynomial.md#root-of-a-polynomial). Choose a real $\lambda$ outside those roots; the adjugate argument proves that $C+\lambda D$ is invertible.

Finally write the given complex [similarity transformation](../../../linear-algebra.md#similarity-transformation) as $P=C+iD$. The relation $AP=PB$, with $A,B$ real, yields $AC=CB$ and $AD=DB$ by comparing real and imaginary parts. Choose the preceding $\lambda$ and put $Q=C+\lambda D$. Then $AQ=QB$, so

$$
\boxed{Q^{-1}AQ=B\quad\text{with }Q\text{ real and invertible}.}
$$

This proves [real similarity from complex similarity](../../../linear-algebra.md#real-similarity-from-complex-similarity) by constructing a real intertwiner, rather than requiring $C$ or $D$ separately to be invertible.

## 18C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="18c/solution">Solution</h3>

↑ **Parent:** [18C](#18c)

For an [inviscid flow](../../../fluid-mechanics.md#inviscid-flow) that is an [incompressible flow](../../../fluid-mechanics.md#incompressible-flow) and an [irrotational flow](../../../fluid-mechanics.md#irrotational-flow), write $\mathbf u=\nabla\phi$. The [Euler equations for an inviscid fluid](../../../fluid-mechanics.md#euler-equations-for-an-inviscid-fluid), without gravity, integrate spatially to the [Unsteady Bernoulli equation](../../../fluid-mechanics.md#unsteady-bernoulli-equation)

$$
\boxed{\frac{\partial\phi}{\partial t}+\frac12|\nabla\phi|^2+\frac p\rho=C(t).}
$$

A time-dependent addition to $\phi$ can absorb $C(t)$.

In the ideal uniform tube-plug model, let $u(t)$ be the axial speed toward the outlet. Incompressibility and fixed cross-section make the speed the same at both ends. With $\phi=u(t)x$, the kinetic terms cancel when the [Unsteady Bernoulli equation](../../../fluid-mechanics.md#unsteady-bernoulli-equation) is subtracted between entrance and exit, giving

$$
L\dot u=\frac{p_{\rm in}-p_{\rm out}}\rho=\frac{2\gamma}{\rho R}.
$$

Conservation of volume in the spherical balloon gives $4\pi R^2\dot R=-\pi a^2u$, or $u=-4R^2\dot R/a^2$. Differentiating and eliminating $u$ yields

$$
-\frac{4L}{a^2}(R^2\ddot R+2R\dot R^2)=\frac{2\gamma}{\rho R},\qquad \boxed{R^3\ddot R+2R^2\dot R^2=-K},\quad K=\frac{\gamma a^2}{2\rho L}.
$$

This is the [constant-tension balloon discharge](../../../fluid-mechanics.md#constant-tension-balloon-discharge) equation; entrance losses and a reservoir-to-tube kinetic-head correction are excluded by this ideal plug model.

Multiplication by $2R\dot R$ turns the equation into

$$
\frac d{dt}(R^4\dot R^2)=-K\frac d{dt}(R^2),\qquad R^4\dot R^2+KR^2=C.
$$

The printed time formula additionally assumes the water is initially at rest, $\dot R(0)=0$, although only $R_0$ is explicitly specified in the question. Under that assumption $C=KR_0^2$. On the shrinking branch,

$$
\dot R=-\frac{\sqrt K\sqrt{R_0^2-R^2}}{R^2},\qquad t=\frac1{\sqrt K}\int_R^{R_0}\frac{r^2}{\sqrt{R_0^2-r^2}}\,dr.
$$

Set $r=R_0\sin\vartheta$ and $\theta=\arcsin(R/R_0)$. The [integral](../../../calculus.md#integral) becomes $R_0^2K^{-1/2}\int_\theta^{\pi/2}\sin^2\vartheta\,d\vartheta$, hence

$$
\boxed{t=R_0^2\sqrt{\frac{2\rho L}{\gamma a^2}}\left(\frac\pi4-\frac\theta2+\frac{\sin2\theta}{4}\right).}
$$

Putting $R=0$, or $\theta=0$, gives the ideal **emptying time**

$$
\boxed{t_{\rm empty}=\frac{\pi R_0^2}{4}\sqrt{\frac{2\rho L}{\gamma a^2}}.}
$$

For an independently prescribed initial rate $v_0=\dot R(0)$, the [first integral](../../../differential-equation.md#first-integral) instead has $C=KR_0^2+R_0^4v_0^2$, so radius alone does not determine that emptying time. This explicitly identifies the extra initial datum needed for the displayed answer.

## 19G

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="19g/a">a</h3>

↑ **Parent:** [19G](#19g)

<h4 id="19g/a/solution">Solution</h4>

↑ **Parent:** [A](#19g/a)

For any [idempotent linear map](../../../vector-space.md#projection-linear-algebra) $\tau$, each vector decomposes as

$$
u=(u-\tau u)+\tau u,\qquad \tau(u-\tau u)=0,\qquad\tau u\in\operatorname{im}\tau.
$$

If $w\in\ker\tau\cap\operatorname{im}\tau$, write $w=\tau v$; then $0=\tau w=\tau^2v=\tau v=w$. Thus the [kernel of a linear map](../../../linear-algebra.md#kernel-of-a-linear-map) and [image of a linear map](../../../vector-space.md#image-of-a-linear-map) give a [direct sum](../../../vector-space.md#direct-sum).

For the self-adjoint map in the question, $k\in\ker\tau$ and $w=\tau v$ satisfy $\langle k,w\rangle=\langle k,\tau v\rangle=\langle\tau k,v\rangle=0$. Hence the direct sum is an [orthogonal decomposition](../../../hilbert-space.md#orthogonal-decomposition-by-a-closed-subspace):

$$
\boxed{U=\ker\tau\mathbin\oplus^{\perp}\operatorname{im}\tau.}
$$

<h3 id="19g/b">b</h3>

↑ **Parent:** [19G](#19g)

<h4 id="19g/b/solution">Solution</h4>

↑ **Parent:** [B](#19g/b)

For a [normal operator](../../../hilbert-space.md#normal-operator) $\phi$, the [adjoint operator](../../../hilbert-space.md#adjoint-operator) identity and $\phi^*\phi=\phi\phi^*$ give

$$
\|\phi u\|^2=\langle\phi^*\phi u,u\rangle=\langle\phi\phi^*u,u\rangle=\|\phi^*u\|^2.
$$

Positive definiteness implies $\ker\phi=\ker\phi^*$. Also $(\operatorname{im}\phi)^\perp=\ker\phi^*$, since orthogonality to every $\phi v$ means $\langle\phi^*u,v\rangle=0$ for every $v$. In finite dimension this gives $\operatorname{im}\phi=(\ker\phi)^{\perp}$.

The [idempotent linear map](../../../vector-space.md#projection-linear-algebra) decomposes $U=\ker\phi\oplus\operatorname{im}\phi$ as in part (a), now orthogonally, and acts as zero on its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) and identity on its [image](../../../set-theory.md#image-of-a-function). Writing $u=k+w$ and $v=k'+w'$ in these orthogonal summands,

$$
\langle\phi u,v\rangle=\langle w,w'\rangle=\langle u,\phi v\rangle.
$$

Thus $\phi$ is [self-adjoint](../../../linear-operator-theory.md#self-adjoint-operator), and together with idempotence this proves **$\phi$ is an orthogonal projection**.

<h3 id="19g/c">c</h3>

↑ **Parent:** [19G](#19g)

<h4 id="19g/c/solution">Solution</h4>

↑ **Parent:** [C](#19g/c)

The finite-dimensional [inner product space](../../../linear-algebra.md#inner-product-space) has the [orthogonal decomposition](../../../hilbert-space.md#orthogonal-decomposition-by-a-closed-subspace) $U=W\oplus W^\perp$. Define $\tau(w+z)=w$ for $w\in W$, $z\in W^\perp$. This is a [linear map](../../../vector-space.md#linear-map) with image $W$, satisfies $\tau^2=\tau$, and is self-adjoint by taking [inner products](../../../linear-algebra.md#inner-product) between decomposed vectors. Hence it is an [orthogonal projection](../../../hilbert-space.md#orthogonal-projection).

Any other [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) with image $W$ has kernel $W^\perp$ by part (a); it is identity on $W$ by idempotence and zero on its kernel. Its values are therefore forced to agree with $\tau$, proving uniqueness.

If $\tau_2\tau_1=0$, every $w_1\in W_1$ has $w_1=\tau_1w_1$, so $\tau_2w_1=0$ and $w_1\in W_2^\perp$. Conversely, if $W_1\subset W_2^\perp$, every image $\tau_1u$ is killed by $\tau_2$. Therefore

$$
\boxed{\tau_2\circ\tau_1=0\quad\Longleftrightarrow\quad W_1\perp W_2.}
$$

<h3 id="19g/d">d</h3>

↑ **Parent:** [19G](#19g)

<h4 id="19g/d/solution">Solution</h4>

↑ **Parent:** [D](#19g/d)

Take any positive definite [inner product](../../../linear-algebra.md#inner-product) $\langle\ ,\ \rangle_0$ on $U$ and define the [inner product adapted to an idempotent linear map](../../../vector-space.md#inner-product-adapted-to-an-idempotent-linear-map)

$$
\boxed{\langle u,v\rangle_{\phi}=\langle\phi u,\phi v\rangle_0+\langle(I-\phi)u,(I-\phi)v\rangle_0.}
$$

It is symmetric and bilinear. If its quadratic value at $u$ is zero, positive definiteness of the original [inner product](../../../linear-algebra.md#inner-product) forces both $\phi u=0$ and $(I-\phi)u=0$, hence $u=0$. Thus it is positive definite.

Using $\phi^2=\phi$ and $(I-\phi)\phi=0$ gives

$$
\langle\phi u,v\rangle_{\phi}=\langle\phi u,\phi v\rangle_0=\langle u,\phi v\rangle_{\phi}.
$$

The map is therefore [self-adjoint](../../../linear-operator-theory.md#self-adjoint-operator) for this new [inner product](../../../linear-algebra.md#inner-product) and remains idempotent, so **it is an orthogonal projection for the explicitly constructed inner product**. Geometrically the construction makes its complementary [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) and [image](../../../set-theory.md#image-of-a-function) orthogonal.

## 20A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="20a/solution">Solution</h3>

↑ **Parent:** [20A](#20a)

The time-independent [Schrödinger equation](../../../physics.md#schrodinger-equation) is $[-\hbar^2\nabla^2/(2m)+V]\psi=E\psi$, with attractive [Coulomb potential](../../../electromagnetism.md#coulomb-potential-energy) $V(r)=-\kappa/r$, where $\kappa=e^2/(4\pi\varepsilon_0)$. Separating $\psi=R(r)Y_\ell^m(\theta,\varphi)$ uses the [spherical harmonic](../../../analysis.md#spherical-harmonic) angular [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $-\ell(\ell+1)$ of the unit-sphere [Laplacian](../../../calculus.md#laplacian). The radial kinetic contribution is $-\hbar^2(R''+2R'/r)/(2m)$, the angular kinetic contribution is the centrifugal term $\hbar^2\ell(\ell+1)R/(2mr^2)$, and the remaining term is the attractive [potential energy](../../../classical-mechanics.md#potential-energy). The right side is the [energy eigenvalue](../../../quantum-mechanics.md#energy-eigenvalue) times the radial [wavefunction](../../../quantum-mechanics.md#wave-function). Here the stated $m$ neglects nuclear recoil; including it replaces the electron mass by the [reduced mass](../../../classical-mechanics.md#reduced-mass).

For $\ell=0$, substitution of the ground-state exponential gives

$$
-\frac{\hbar^2}{2m}(\alpha^2-2\alpha/r)-\frac\kappa r=E_1.
$$

Its $1/r$ coefficient must vanish and its constant coefficient determines the [energy](../../../classical-mechanics.md#energy), so

$$
\boxed{\alpha=\frac{m\kappa}{\hbar^2}=\frac1{a_0},\qquad E_1=-\frac{m\kappa^2}{2\hbar^2}.}
$$

Here $a_0=\hbar^2/(m\kappa)$ is the [Bohr radius](../../../physics.md#bohr-radius).

For $R_2=N_2(r+b)e^{-\beta r}$, direct differentiation yields

$$
R_2''+\frac2rR_2'=N_2e^{-\beta r}\left[\beta^2(r+b)-4\beta+\frac{2-2\beta b}{r}\right].
$$

Cancel the nonzero exponential in the radial [Schrödinger equation](../../../physics.md#schrodinger-equation) and compare coefficients of $r$, the constant term, and $1/r$. They give, respectively,

$$
E_2=-\frac{\hbar^2\beta^2}{2m},\qquad \frac{2\hbar^2\beta}{m}=\kappa,\qquad \frac{\hbar^2}{m}(\beta b-1)-\kappa b=0.
$$

Consequently

$$
\boxed{\beta=\frac1{2a_0},\qquad b=-2a_0,\qquad E_2=-\frac{m\kappa^2}{8\hbar^2}=\frac14E_1.}
$$

The positive decay constants ensure normalizability; the second radial [wavefunction](../../../quantum-mechanics.md#wave-function) has one positive-radius node at $2a_0$, as appropriate to the first radial excitation.

If the entire energy gap is carried by one [photon](../../../quantum-mechanics.md#photon), neglecting atomic recoil, [conservation of energy](../../../physics.md#conservation-of-energy) gives the requested frequency

$$
\boxed{\nu_{\rm gap}=\frac{E_2-E_1}{h}=\frac{3m\kappa^2}{8h\hbar^2}=\frac{3me^4}{8h\hbar^2(4\pi\varepsilon_0)^2}.}
$$

There is a physical qualification: these are the $2s$ and $1s$ states, so the usual single-photon electric-dipole transition is forbidden by the [electric-dipole selection rules for hydrogen](../../../physics.md#electric-dipole-selection-rules-for-hydrogen). Explicitly, both angular factors are $Y_0^0$, and $\int |Y_0^0|^2\hat{\mathbf r}\,d\Omega=0$, so every component of $\langle1s|\mathbf r|2s\rangle$ vanishes. The leading isolated-atom decay is instead two-photon emission, for which $\nu_1+\nu_2=\nu_{\rm gap}$ and individual frequencies are not fixed. This metastability and the two-photon channel are documented in [NIST's hydrogen spectral-data compilation](https://tsapps.nist.gov/publication/get_pdf.cfm?pub_id=842564). Thus the boxed answer is the energy-gap frequency under the printed single-photon assumption, rather than an assertion of an allowed electric-dipole line.

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
