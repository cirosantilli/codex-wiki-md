# Paper 1

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2018/paperib_1_2018.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2018/paperib_1_2018.pdf)

**Table of contents**

- [1E](#1e)
  - [Solution](#1e/solution)
- [2A](#2a)
  - [a](#2a/a)
    - [Solution](#2a/a/solution)
  - [b](#2a/b)
    - [Solution](#2a/b/solution)
  - [c](#2a/c)
    - [Solution](#2a/c/solution)
- [3G](#3g)
  - [a](#3g/a)
    - [Solution](#3g/a/solution)
  - [b](#3g/b)
    - [Solution](#3g/b/solution)
  - [c](#3g/c)
    - [Solution](#3g/c/solution)
- [4B](#4b)
  - [Solution](#4b/solution)
- [5D](#5d)
  - [Solution](#5d/solution)
- [6D](#6d)
  - [Solution](#6d/solution)
- [7H](#7h)
  - [Solution](#7h/solution)
- [8H](#8h)
  - [Solution](#8h/solution)
- [9E](#9e)
  - [Solution](#9e/solution)
- [10G](#10g)
  - [a](#10g/a)
    - [Solution](#10g/a/solution)
  - [b](#10g/b)
    - [Solution](#10g/b/solution)
  - [c](#10g/c)
    - [Solution](#10g/c/solution)
- [11F](#11f)
  - [a](#11f/a)
    - [Solution](#11f/a/solution)
  - [b](#11f/b)
    - [Solution](#11f/b/solution)
  - [c](#11f/c)
    - [Solution](#11f/c/solution)
- [12E](#12e)
  - [Solution](#12e/solution)
- [13A](#13a)
  - [a](#13a/a)
    - [Solution](#13a/a/solution)
  - [b](#13a/b)
    - [Solution](#13a/b/solution)
- [14C](#14c)
  - [Solution](#14c/solution)
- [15B](#15b)
  - [Solution](#15b/solution)
- [16C](#16c)
  - [Solution](#16c/solution)
- [17D](#17d)
  - [a](#17d/a)
    - [Solution](#17d/a/solution)
  - [b](#17d/b)
    - [Solution](#17d/b/solution)
  - [c](#17d/c)
    - [Solution](#17d/c/solution)
  - [d](#17d/d)
    - [Solution](#17d/d/solution)
- [18D](#18d)
  - [Solution](#18d/solution)
- [19H](#19h)
  - [a](#19h/a)
    - [Solution](#19h/a/solution)
  - [b](#19h/b)
    - [i](#19h/b/i)
      - [Solution](#19h/b/i/solution)
    - [ii](#19h/b/ii)
      - [Solution](#19h/b/ii/solution)
    - [iii](#19h/b/iii)
      - [Solution](#19h/b/iii/solution)
- [20H](#20h)
  - [Solution](#20h/solution)

## 1E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1e/solution">Solution</h3>

↑ **Parent:** [1E](#1e)

The [rank-nullity theorem](../../../linear-algebra.md#rank-nullity-theorem) says that for a linear map $T:V\to W$ with finite-dimensional domain, $\dim V=\dim\ker T+\dim\operatorname{im}T$. Apply it to $\beta|_{\operatorname{im}\alpha}$. Its image is $\operatorname{im}(\beta\alpha)$ and its kernel is $\operatorname{im}\alpha\cap\ker\beta$, so

$$
\boxed{\dim\operatorname{im}\alpha
=\dim\operatorname{im}(\beta\alpha)
+\dim(\operatorname{im}\alpha\cap\ker\beta).}
$$

Since $\operatorname{im}(\alpha\gamma)\subseteq\operatorname{im}\alpha$,

$$
\dim(\operatorname{im}(\alpha\gamma)\cap\ker\beta)
\leq\dim(\operatorname{im}\alpha\cap\ker\beta).
$$

Using the preceding identity for both restrictions and rearranging gives

$$
\boxed{\dim\operatorname{im}(\beta\alpha)+\dim\operatorname{im}(\alpha\gamma)
\leq\dim\operatorname{im}\alpha+\dim\operatorname{im}(\beta\alpha\gamma).}
$$

## 2A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2a/a">a</h3>

↑ **Parent:** [2A](#2a)

<h4 id="2a/a/solution">Solution</h4>

↑ **Parent:** [A](#2a/a)

Choose

$$
\operatorname{Log}z=\log|z|+i\arg z,\qquad -\frac\pi2<\arg z<\frac\pi2.
$$

It is holomorphic on the right half-plane with derivative $1/z\ne0$, and its inverse $z=e^w$ has positive real part precisely for $|\operatorname{Im}w|<\pi/2$. Thus this branch of the [complex logarithm](../../../analysis.md#complex-logarithm) is a conformal bijection onto $S$.

<h3 id="2a/b">b</h3>

↑ **Parent:** [2A](#2a)

<h4 id="2a/b/solution">Solution</h4>

↑ **Parent:** [B](#2a/b)

For $\operatorname{Re}z>0$,

$$
|z+1|^2-|z-1|^2=4\operatorname{Re}z>0,
$$

so $w=(z-1)/(z+1)$ lies in the unit disc. Its inverse is $z=(1+w)/(1-w)$, whose real part is $(1-|w|^2)/|1-w|^2>0$. Both derivatives are nonzero, proving this [Möbius transformation](../../../group-theory.md#mobius-transformation) is conformal.

<h3 id="2a/c">c</h3>

↑ **Parent:** [2A](#2a)

<h4 id="2a/c/solution">Solution</h4>

↑ **Parent:** [C](#2a/c)

Composing the maps gives

$$
\boxed{w\longmapsto\frac{e^w-1}{e^w+1}=\tanh\frac w2,}
$$

a conformal bijection from $S$ to the unit disc.

## 3G

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3g/a">a</h3>

↑ **Parent:** [3G](#3g)

<h4 id="3g/a/solution">Solution</h4>

↑ **Parent:** [A](#3g/a)

For a geodesic triangle on the unit sphere with angles $\alpha,\beta,\gamma$, the [Gauss-Bonnet theorem](../../../differential-geometry.md#gauss-bonnet-theorem) gives

$$
\boxed{\operatorname{area}=\alpha+\beta+\gamma-\pi.}
$$

<h3 id="3g/b">b</h3>

↑ **Parent:** [3G](#3g)

<h4 id="3g/b/solution">Solution</h4>

↑ **Parent:** [B](#3g/b)

For a geodesic triangulation with $V,E,F$ vertices, edges, and faces, summing the spherical excess gives $4\pi=2\pi V-\pi F$, because all angles around each vertex sum to $2\pi$. Also $3F=2E$. Therefore

$$
V-E+F=V-\frac32F+F=V-\frac12F=2.
$$

Thus **every geodesic triangulation of the sphere has Euler number $2$**.

<h3 id="3g/c">c</h3>

↑ **Parent:** [3G](#3g)

<h4 id="3g/c/solution">Solution</h4>

↑ **Parent:** [C](#3g/c)

If six triangles met at every vertex, counting vertex-face incidences would give $3F=6V$, hence $F=2V$. But part b gives $F=2V-4$, a contradiction. Therefore **no such triangulation exists**.

## 4B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4b/solution">Solution</h3>

↑ **Parent:** [4B](#4b)

For $f=x^2+y^2+z^2$ and $g=x^2+2y^2-z^2=1$, the [Lagrange multiplier](../../../mathematical-optimization.md#lagrange-multiplier) equations are

$$
(1-\lambda)x=0,\qquad(1-2\lambda)y=0,\qquad(1+\lambda)z=0.
$$

The four constrained stationary points are

$$
\boxed{(\pm1,0,0),\qquad(0,\pm1/\sqrt2,0).}
$$

On the constraint, $f=2x^2+3y^2-1$ with $x^2+2y^2\geq1$. The two $y$-axis points are global minima, while the $x$-axis points are saddles: motion along the waist decreases $f$, whereas motion away from it increases $f$. There is no maximum.

If instead $g=x^2+2y^2-z^2$ is optimized on $x^2+y^2+z^2=1$, the stationary points are all six coordinate-axis points. The $y$-axis points are maxima with value $2$, the $z$-axis points are minima with value $-1$, and the $x$-axis points are saddles with value $1$.

## 5D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5d/solution">Solution</h3>

↑ **Parent:** [5D](#5d)

The velocity is $\mathbf u=\nabla\phi=q\mathbf e_r/(2\pi r)$. Its [divergence in polar coordinates](../../../calculus.md#divergence-in-polar-coordinates) is zero for $r>0$, while a circle about the origin has flux

$$
\int_0^{2\pi}\frac{q}{2\pi r}r\,d\theta=\boxed q.
$$

By contour deformation the same holds for any enclosing contour. This is a two-dimensional [point source](../../../fluid-mechanics.md#point-source) of strength $q$.

For the second potential,

$$
\frac{\partial\phi}{\partial y}
=\frac q{2\pi}\left[
\frac{y-a}{x^2+(y-a)^2}+\frac{y+a}{x^2+(y+a)^2}\right],
$$

which vanishes at $y=0$. In the full plane this is a pair of equal sources of strength $q$ at $(0,\pm a)$. In $y>0$, it is one source at $(0,a)$ beside an impermeable slip wall, with the lower source serving as its [image](../../../mathematics.md#method-of-images).

## 6D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6d/solution">Solution</h3>

↑ **Parent:** [6D](#6d)

Substituting the exact solution and expanding about $t_n$ gives the [local truncation error](../../../numerical-analysis.md#local-truncation-error)

$$
y(t_{n+1})-y(t_n)-\frac h2\bigl(y'(t_n)+y'(t_{n+1})\bigr)
=-\frac{h^3}{12}y'''(t_n)+O(h^4).
$$

Thus the method is consistent of order two; as a stable one-step method it has **global convergence order $k=2$**.

The order cannot be higher. For $y'=t^2$, $y(0)=0$, the exact solution is $y=t^3/3$, and direct substitution makes the local truncation error exactly

$$
\boxed{-\frac16h^3.}
$$

## 7H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7h/solution">Solution</h3>

↑ **Parent:** [7H](#7h)

The distribution function is $F(x)=x^2/\theta^2$ on $[0,\theta]$, so its median is $\theta/\sqrt2$. The [likelihood function](../../../statistical-modelling.md#likelihood-function) is

$$
L(\theta)=2^n\left(\prod_iX_i\right)\theta^{-2n}\mathbf1_{\{\theta\geq X_{(n)}\}},
$$

which decreases over its admissible range. Hence $\widehat\theta=X_{(n)}=\max_iX_i$. By the [invariance property of maximum likelihood estimation](../../../statistical-modelling.md#invariance-property-of-maximum-likelihood-estimation),

$$
\boxed{\widehat m=\frac{X_{(n)}}{\sqrt2}.}
$$

## 8H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8h/solution">Solution</h3>

↑ **Parent:** [8H](#8h)

A [transportation problem](../../../mathematical-optimization.md#transportation-problem) minimizes $\sum_{ij}c_{ij}x_{ij}$ subject to nonnegative shipments, prescribed row supplies, and prescribed column demands.

One optimal shipment table is

$$
\boxed{
\begin{pmatrix}
0&4&6\\
0&0&8\\
3&5&0
\end{pmatrix},}
$$

which has the required row sums $(10,8,8)$ and column sums $(3,9,14)$ and costs $4(3)+6(1)+8(3)+3(3)+5(5)=\boxed{76}$.

For an optimality certificate, take row potentials $(1,3,3)$ and column potentials $(0,2,0)$. Their sums equal costs in occupied cells and do not exceed any cost:

$$
\begin{pmatrix}1&3&1\\3&5&3\\3&5&3\end{pmatrix}
\leq
\begin{pmatrix}4&3&1\\6&10&3\\3&5&7\end{pmatrix}.
$$

The dual value is $10+24+24+18=76$, so [linear programming duality](../../../mathematical-optimization.md#linear-programming-duality) proves optimality.

## 9E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9e/solution">Solution</h3>

↑ **Parent:** [9E](#9e)

A [Jordan block](../../../linear-operator-theory.md#jordan-block) $J_m(\lambda)$ has $\lambda$ on its diagonal, ones on its superdiagonal, and zeros elsewhere. A matrix is in [Jordan normal form](../../../linear-operator-theory.md#jordan-normal-form) when it is block diagonal with Jordan blocks.

On a block $J_m(\lambda)$, $\ker(\alpha-\lambda I)^r$ has dimension $\min(r,m)$. Its increase from $r-1$ to $r$ is one exactly when $m\geq r$. Summing over blocks proves that

$$
\boxed{\dim\ker(\alpha-\lambda I)^r-\dim\ker(\alpha-\lambda I)^{r-1}}
$$

counts the $\lambda$-blocks of size at least $r$.

If $\lambda\ne0$, the polynomial $z^2$ has nonzero derivative at $\lambda$, so

$$
\boxed{J_m(\lambda)^2\sim J_m(\lambda^2).}
$$

If $\lambda=0$, squaring the nilpotent shift separates the odd and even basis chains:

$$
\boxed{J_m(0)^2\sim J_{\lceil m/2\rceil}(0)\oplus J_{\lfloor m/2\rfloor}(0),}
$$

omitting a zero-size block.

The displayed invertible matrix preserves the subspaces spanned by $(e_1,e_4)$ and $(e_2,e_3)$. Its restrictions have characteristic polynomials $t^2-a_1a_4$ and $t^2-a_2a_3$. Since invertibility makes both products nonzero, each restriction has two distinct complex eigenvalues. Its Jordan form is therefore

$$
\boxed{\operatorname{diag}\left(\sqrt{a_1a_4},-\sqrt{a_1a_4},
\sqrt{a_2a_3},-\sqrt{a_2a_3}\right),}
$$

for either choices of the square roots.

## 10G

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10g/a">a</h3>

↑ **Parent:** [10G](#10g)

<h4 id="10g/a/solution">Solution</h4>

↑ **Parent:** [A](#10g/a)

Write $|G|=p^nm$ with $p\nmid m$. The [Sylow theorems](../../../finite-group-theory.md#sylow-theorems) state:

- $G$ has a subgroup of order $p^n$.
- Every $p$-subgroup lies in a Sylow $p$-subgroup, and all Sylow $p$-subgroups are conjugate.
- Their number $n_p$ satisfies $n_p\equiv1\pmod p$ and $n_p\mid m$.

<h3 id="10g/b">b</h3>

↑ **Parent:** [10G](#10g)

<h4 id="10g/b/solution">Solution</h4>

↑ **Parent:** [B](#10g/b)

Proceed by induction on $|G|$. If $p\mid|Z(G)|$, [Cauchy's theorem for finite groups](../../../finite-group-theory.md#cauchy-theorem-for-groups) gives a central subgroup $C$ of order $p$. By induction $G/C$ has a subgroup of order $p^{n-1}$; its inverse image in $G$ has order $p^n$.

If $p\nmid|Z(G)|$, the [class equation](../../../group-theory.md#class-equation) shows that some noncentral conjugacy class has size not divisible by $p$. For a representative $x$, its class size is $[G:C_G(x)]$, so $p^n\mid|C_G(x)|$. This centralizer is proper because $x$ is noncentral, and induction gives it, hence $G$, a subgroup of order $p^n$. This proves Sylow's first theorem.

<h3 id="10g/c">c</h3>

↑ **Parent:** [10G](#10g)

<h4 id="10g/c/solution">Solution</h4>

↑ **Parent:** [C](#10g/c)

For $|G|=12$, the third Sylow theorem gives $n_3\equiv1\pmod3$ and $n_3\mid4$, so $n_3=1$ or $4$. In the first case the Sylow $3$-subgroup is unique.

If $n_3=4$, conjugation acts transitively on the four Sylow $3$-subgroups. Each normalizer has order $|G|/4=3$ and is the subgroup it normalizes. The action kernel lies in every such subgroup, whose intersection is trivial, so $G$ embeds in $S_4$. Its image has order $12$ and hence index two. The unique index-two subgroup of $S_4$ is $A_4$, so

$$
\boxed{G\cong A_4.}
$$

## 11F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="11f/a">a</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/a/solution">Solution</h4>

↑ **Parent:** [A](#11f/a)

The map $f:U\to\mathbb R^n$ is [differentiable](../../../analysis.md#differentiable-function) at $a$ when there is a linear map $Df(a)$ such that

$$
f(a+h)=f(a)+Df(a)h+o(\|h\|).
$$

It is $C^1$ when it is differentiable everywhere and $a\mapsto Df(a)$ is continuous. The definition immediately gives $\|f(a+h)-f(a)\|\leq(\|Df(a)\|+o(1))\|h\|\to0$, so differentiability implies continuity.

The [inverse function theorem](../../../calculus.md#inverse-function-theorem) says that if $f$ is $C^1$ near $a$ and $Df(a)$ is invertible, then $f$ restricts to a diffeomorphism between neighbourhoods of $a$ and $f(a)$.

<h3 id="11f/b">b</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/b/solution">Solution</h4>

↑ **Parent:** [B](#11f/b)

For distinct $x,y\in U$, convexity keeps the segment $x+t(y-x)$ in $U$. Continuity of $Df$ makes

$$
q=\max_{0\leq t\leq1}\|Df(x+t(y-x))-I\|<1.
$$

The [fundamental theorem of calculus along a line segment](../../../calculus.md#fundamental-theorem-of-calculus-along-a-line-segment) gives

$$
\|f(y)-f(x)-(y-x)\|\leq q\|y-x\|,
$$

so $\|f(y)-f(x)\|\geq(1-q)\|y-x\|>0$. Thus **$f$ is injective**.

The bound $\|Df(a)-I\|<1$ makes $Df(a)$ invertible by the [Neumann series](../../../banach-algebra.md#neumann-series). The inverse function theorem therefore makes $f$ locally open at every point, so $f(U)$ is open.

Surjectivity need not hold: the identity map on a proper convex open set has proper image. Even for $U=\mathbb R^n$ it can fail. In one dimension, $f(x)=\arctan x$ satisfies $|f'(x)-1|=x^2/(1+x^2)<1$, but its image is $(-\pi/2,\pi/2)$.

<h3 id="11f/c">c</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/c/solution">Solution</h4>

↑ **Parent:** [C](#11f/c)

Here

$$
Df(x,y)-I=
\begin{pmatrix}2x-1&-2y\\2y&2x-1\end{pmatrix}.
$$

This matrix acts as multiplication by the complex number $(2x-1)+2iy$, so its operator norm is $\sqrt{(2x-1)^2+4y^2}$. The largest set is therefore

$$
\boxed{U=\left\{(x,y):\left(x-\frac12\right)^2+y^2<\frac14\right\}.}
$$

## 12E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12e/solution">Solution</h3>

↑ **Parent:** [12E](#12e)

A [compact space](../../../topology.md#compact-space) is one for which every open cover has a finite subcover. Let $\mathcal U$ cover $[0,1]$, and let

$$
A=\{x\in[0,1]:[0,x]\text{ has a finite subcover from }\mathcal U\}.
$$

The set is nonempty. If $s=\sup A<1$, choose $U\in\mathcal U$ containing $s$. An interval about $s$ lies in $U$; a point of $A$ just to the left of $s$ then extends the finite cover beyond $s$, contradicting the definition of the supremum. Hence $s=1$, and the same neighbourhood argument covers $1$, proving $[0,1]$ compact.

The continuous map $t\mapsto(\cos2\pi t,\sin2\pi t)$ maps $[0,1]$ onto $S^1$. A continuous image of a compact space is compact: pull an open cover back, choose a finite subcover, and push the corresponding sets forward. Thus $S^1$ is compact.

In the unusual topology on $X=\mathbb R^2\setminus\{0\}$, a proper closed set is a finite union of punctured lines through the origin. Take any nonempty member $U$ of an open cover. Its complement is such a finite union. Each punctured line has the indiscrete subspace topology, because every other vector subspace meets it only at the removed origin, and is therefore compact. Finitely many finite subcovers, together with $U$, cover $X$. Hence **$X$ is compact**.

## 13A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="13a/a">a</h3>

↑ **Parent:** [13A](#13a)

<h4 id="13a/a/solution">Solution</h4>

↑ **Parent:** [A](#13a/a)

The integrand

$$
F(z)=\frac{e^{iz^2/(4\pi)}}{e^{z/2}-e^{-z/2}}
$$

has one pole inside the rectangle, at $z=0$, with residue $1$. The [residue theorem](../../../analysis.md#residue-theorem) therefore gives $\int_CF(z)\,dz=2\pi i$. The vertical-side integrals tend to zero as $R\to\infty$.

On the horizontal sides, direct substitution $z=x\pm\pi i$, with the upper side oppositely oriented, shows that their sum is

$$
i e^{-i\pi/4}\int_{-R}^{R}e^{ix^2/(4\pi)}
\left(\frac1{1+e^x}+\frac{e^x}{1+e^x}\right)dx.
$$

Taking the limit and comparing with $2\pi i$ gives

$$
\boxed{\lim_{R\to\infty}\int_{-R}^{R}e^{ix^2/(4\pi)}\,dx
=2\pi e^{i\pi/4}.}
$$

<h3 id="13a/b">b</h3>

↑ **Parent:** [13A](#13a)

<h4 id="13a/b/solution">Solution</h4>

↑ **Parent:** [B](#13a/b)

Integrate $ze^{i\pi z}/(z^2+a^2)$ over the upper semicircle. [Jordan lemma](../../../complex-analysis.md#jordan-s-lemma) removes the arc, and the pole at $z=ia$ has residue $e^{-\pi a}/2$. Hence

$$
\int_{-\infty}^{\infty}\frac{x e^{i\pi x}}{x^2+a^2}\,dx
=\pi i e^{-\pi a}.
$$

The cosine contribution is odd, while the sine contribution is even. Therefore

$$
\boxed{\int_0^\infty\frac{x\sin(\pi x)}{x^2+a^2}\,dx
=\frac\pi2e^{-\pi a}.}
$$

## 14C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="14c/solution">Solution</h3>

↑ **Parent:** [14C](#14c)

The [convolution](../../../fourier-analysis.md#convolution) is $(f*g)(x)=\int_{-\infty}^{\infty}f(y)g(x-y)\,dy$. Under the usual integrability hypotheses, [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem) and $u=x-y$ give

$$
\begin{aligned}
\widetilde{f*g}(k)
&=\iint e^{-ikx}f(y)g(x-y)\,dy\,dx\\
&=\left(\int e^{-iky}f(y)\,dy\right)
\left(\int e^{-iku}g(u)\,du\right)
=\boxed{\widetilde f(k)\widetilde g(k)}.
\end{aligned}
$$

The supplied transform and the [Fourier shift theorem](../../../analysis.md#fourier-shift-theorem) give

$$
\mathcal F\!\left(\frac{\sin x}{x}\right)
=\begin{cases}\pi,&|k|<1,\\0,&|k|>1.\end{cases}
$$

Since

$$
\frac{\sin x}{x^2}=\frac{\cos x}{x}-\frac d{dx}\left(\frac{\sin x}{x}\right),
$$

the shift and differentiation rules yield

$$
\boxed{
\mathcal F\!\left(\frac{\sin x}{x^2}\right)(k)
=\begin{cases}
-i\pi k,&|k|\leq1,\\
-i\pi\,\operatorname{sgn}k,&|k|\geq1.
\end{cases}}
$$

The coincident boundary values make the endpoint convention immaterial.

## 15B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="15b/solution">Solution</h3>

↑ **Parent:** [15B](#15b)

For an [S wave](../../../wave-equation.md#s-wave), put $u(r)=r\psi(r)$. A bound state has $E=-\varepsilon<0$, and the radial Schrödinger equation gives

$$
u(r)=
\begin{cases}
A\sin(kr),&r<a,\\
Be^{-\kappa r},&r>a,
\end{cases}
$$

where

$$
k^2=\frac{2m(U-\varepsilon)}{\hbar^2},
\qquad
\kappa^2=\frac{2m\varepsilon}{\hbar^2}.
$$

Continuity of $u,u'$ at $a$ gives

$$
\boxed{k\cot(ka)=-\kappa,\qquad
k^2+\kappa^2=\frac{2mU}{\hbar^2}.}
$$

The first bound state appears at threshold $\kappa\downarrow0$, where $ka=\pi/2$. The zero-energy threshold itself is not normalizable, so a deuteron bound state exists precisely when

$$
\boxed{U>\frac{\pi^2\hbar^2}{8ma^2}.}
$$

The wavefunction is $\psi=u/r$, with normalization fixing the remaining constant.

## 16C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="16c/solution">Solution</h3>

↑ **Parent:** [16C](#16c)

For a localized steady current, define

$$
\mathbf m=\frac12\int\mathbf r\times\mathbf J(\mathbf r)\,dV.
$$

Assume the external field varies negligibly across the current distribution. Expanding it to first order, the uniform term gives no net force because $\int\mathbf J\,dV=0$. Using the supplied integral identity and $\nabla\cdot\mathbf B=0$, the first-order term in $\int\mathbf J\times\mathbf B\,dV$ reduces to

$$
\mathbf F=\nabla(\mathbf m\cdot\mathbf B).
$$

Since $\mathbf F=-\nabla U$, the [magnetic dipole potential energy](../../../electromagnetism.md#magnetic-dipole-potential-energy) is

$$
\boxed{U=-\mathbf m\cdot\mathbf B.}
$$

Here

$$
|\mathbf B|=\sqrt{B_0^2+B_1^2(x^2+y^2)}
$$

increases away from the $z$-axis. A dipole parallel to $\mathbf B$ has energy $-m|\mathbf B|$ and is drawn toward stronger field, hence outward from the axis. An antiparallel dipole has energy $+m|\mathbf B|$ and is driven toward the weak-field axis. The field therefore spatially separates the two orientations.

## 17D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="17d/a">a</h3>

↑ **Parent:** [17D](#17d)

<h4 id="17d/a/solution">Solution</h4>

↑ **Parent:** [A](#17d/a)

Take $x$ vertically downward along the wall and $y$ normally outward, with the wall at $y=0$ and free surface at $y=h$. The expected steady velocity is $\mathbf u=u(y)\mathbf e_x$: it vanishes at the wall and is opposed by an upward air shear $ku(h)$ at the surface. Gravity supplies the downward body force $\rho g\mathbf e_x$, while the surface normal stress is the atmospheric pressure $p_0$.

<h3 id="17d/b">b</h3>

↑ **Parent:** [17D](#17d)

<h4 id="17d/b/solution">Solution</h4>

↑ **Parent:** [B](#17d/b)

The steady parallel-flow [Navier-Stokes equations](../../../viscous-fluid-flow.md#navier-stokes-equation) reduce to

$$
p_y=0,\qquad \mu u''+\rho g=0.
$$

The boundary conditions are

$$
p(h)=p_0,\qquad u(0)=0,\qquad \mu u'(h)=-ku(h).
$$

The last condition balances the liquid's tangential traction with the opposing air stress. Hence $p=p_0$ and

$$
\boxed{
u(y)=-\frac{\rho g}{2\mu}y^2
+\frac{\rho gh}{\mu+kh}\left(1+\frac{kh}{2\mu}\right)y.}
$$

<h3 id="17d/c">c</h3>

↑ **Parent:** [17D](#17d)

<h4 id="17d/c/solution">Solution</h4>

↑ **Parent:** [C](#17d/c)

Substitution of $y=h$ gives

$$
\boxed{u(h)=\frac{\rho gh^2}{2\mu}
\left(1+\frac{kh}{\mu}\right)^{-1}.}
$$

<h3 id="17d/d">d</h3>

↑ **Parent:** [17D](#17d)

<h4 id="17d/d/solution">Solution</h4>

↑ **Parent:** [D](#17d/d)

The [volume flux per unit width](../../../fluid-mechanics.md#volume-flux-per-unit-width) is

$$
Q=\int_0^hu(y)\,dy
=\boxed{\frac{\rho gh^3}{12\mu}
\frac{4+kh/\mu}{1+kh/\mu}.}
$$

Therefore

$$
\boxed{Q\longrightarrow\frac{\rho gh^3}{3\mu}\quad(k\to0),\qquad
Q\longrightarrow\frac{\rho gh^3}{12\mu}\quad(k\to\infty).}
$$

The first is the stress-free film; the second has an effectively immobilized free surface.

## 18D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="18d/solution">Solution</h3>

↑ **Parent:** [18D](#18d)

Let $P=uu^T/\|u\|^2$. This is an [orthogonal projection matrix](../../../linear-algebra.md#orthogonal-projection-matrix), so $P^T=P$ and $P^2=P$. Therefore the [Householder transformation](../../../linear-algebra.md#householder-transformation)

$$
H_u=I-2P
$$

satisfies $H_u^TH_u=(I-2P)^2=I$. If $\|a\|=\|b\|$ and $a\ne b$, then

$$
\|a-b\|^2=2(a-b)^Ta,
$$

and hence $H_{a-b}a=a-(a-b)=b$.

Apply a Householder transformation to the first column of $A$ to map it to a multiple of $e_1$, then apply transformations supported on the trailing coordinates to clear each later column below its diagonal. Their product is orthogonal and produces $R$; reversing the product gives $A=QR$.

For the displayed matrix, one resulting factorization is

$$
\boxed{
Q=\frac12\begin{pmatrix}
1&-1&1&1\\
1&1&-1&1\\
1&1&1&-1\\
1&-1&-1&-1
\end{pmatrix},
\qquad
R=\begin{pmatrix}
2&3&2\\
0&5&-2\\
0&0&4\\
0&0&0
\end{pmatrix}.}
$$

Direct multiplication gives the stated $A$, and $Q^TQ=I$.

## 19H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="19h/a">a</h3>

↑ **Parent:** [19H](#19h)

<h4 id="19h/a/solution">Solution</h4>

↑ **Parent:** [A](#19h/a)

Minimizing $\|Y-X\theta\|^2$ gives the [normal equations](../../../statistical-modelling.md#normal-equation) $X^TX\widehat\theta=X^TY$. Full column rank makes $X^TX$ invertible, so

$$
\boxed{\widehat\theta=(X^TX)^{-1}X^TY.}
$$

With the [hat matrix](../../../statistical-modelling.md#hat-matrix) $H=X(X^TX)^{-1}X^T$, the residual is $\widehat\varepsilon=(I-H)\varepsilon$. The symmetric projection $I-H$ has rank $n-p$, hence

$$
\boxed{\frac{\widehat\varepsilon^T\widehat\varepsilon}{\sigma^2}
\sim\chi^2_{n-p},\qquad
\widehat{\sigma}^2=\frac{\widehat\varepsilon^T\widehat\varepsilon}{n-p}}
$$

and the latter estimator is unbiased.

<h3 id="19h/b">b</h3>

↑ **Parent:** [19H](#19h)

<h4 id="19h/b/i">i</h4>

↑ **Parent:** [B](#19h/b)

<h5 id="19h/b/i/solution">Solution</h5>

↑ **Parent:** [I](#19h/b/i)

With

$$
Y=(Z_1,Z_2,Z_3,Z_4-2\pi)^T,\qquad
\theta=(\theta_1,\theta_2,\theta_3)^T,
$$

the model has

$$
\boxed{
X=\begin{pmatrix}
1&0&0\\0&1&0\\0&0&1\\-1&-1&-1
\end{pmatrix},\qquad
Y=X\theta+\varepsilon.}
$$

<h4 id="19h/b/ii">ii</h4>

↑ **Parent:** [B](#19h/b)

<h5 id="19h/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#19h/b/ii)

Let $D=Z_1+Z_2+Z_3+Z_4-2\pi$ be the observed closure error. Solving the normal equations gives

$$
\boxed{\widehat\theta_i=Z_i-\frac D4,\qquad i=1,2,3.}
$$

<h4 id="19h/b/iii">iii</h4>

↑ **Parent:** [B](#19h/b)

<h5 id="19h/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#19h/b/iii)

Every residual equals $D/4$, so the residual sum of squares is $D^2/4$. There is one residual degree of freedom, and therefore

$$
\boxed{\widehat{\sigma}^2=\frac{D^2}{4},\qquad
\frac{\widehat{\sigma}^2}{\sigma^2}\sim\chi^2_1.}
$$

## 20H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="20h/solution">Solution</h3>

↑ **Parent:** [20H](#20h)

Let the [Markov chain](../../../markov-process.md#markov-chain) state after each toss be $(S,I)$, where $S$ is player $A_1$'s net winnings and $I$ is the next player to toss. From $(S,i)$ it moves to $(S+1,1)$ with probability $p_i$ and to $(S-1,2)$ with probability $q_i=1-p_i$. The initial state is $(0,1)$, and a return means hitting any state with $S=0$ at positive time.

From $(1,1)$, the probability of hitting zero is

$$
r_+=\begin{cases}1,&p_1+p_2\leq1,\\q_1/p_2,&p_1+p_2>1.\end{cases}
$$

Indeed, in the positive-drift case the bounded harmonic solution of

$$
h_1(x)=p_1h_1(x+1)+q_1h_2(x-1),\qquad
h_2(x)=p_2h_1(x+1)+q_2h_2(x-1)
$$

uses the decaying root $q_2/p_1$ and boundary value $h_2(0)=1$, yielding $h_1(1)=q_1/p_2$; with nonpositive drift the walk hits zero surely. By the reflected argument, from $(-1,2)$ the probability is

$$
r_-=\begin{cases}p_2/q_1,&p_1+p_2<1,\\1,&p_1+p_2\geq1.\end{cases}
$$

Conditioning on the first toss, the required return probability is

$$
\boxed{
p_1r_++q_1r_-=
\begin{cases}
p_1+p_2,&p_1+p_2\leq1,\\[3pt]
\dfrac{(1-p_1)(p_1+p_2)}{p_2},&p_1+p_2\geq1.
\end{cases}}
$$

Both formulas equal one at the boundary $p_1+p_2=1$.

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
