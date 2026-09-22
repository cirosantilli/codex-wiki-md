# Paper 1

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2019/paperib_1_2019.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2019/paperib_1_2019.pdf)

**Table of contents**

- [1F](#1f)
  - [Solution](#1f/solution)
- [2F](#2f)
  - [Solution](#2f/solution)
- [3E](#3e)
  - [Solution](#3e/solution)
- [4A](#4a)
  - [Solution](#4a/solution)
- [5C](#5c)
  - [Solution](#5c/solution)
- [6C](#6c)
  - [Solution](#6c/solution)
- [7H](#7h)
  - [a](#7h/a)
    - [Solution](#7h/a/solution)
  - [b](#7h/b)
    - [Solution](#7h/b/solution)
- [8H](#8h)
  - [Solution](#8h/solution)
- [9F](#9f)
  - [a](#9f/a)
    - [Solution](#9f/a/solution)
  - [b](#9f/b)
    - [Solution](#9f/b/solution)
  - [c](#9f/c)
    - [Solution](#9f/c/solution)
- [10G](#10g)
  - [a](#10g/a)
    - [Solution](#10g/a/solution)
  - [b](#10g/b)
    - [Solution](#10g/b/solution)
  - [c](#10g/c)
    - [Solution](#10g/c/solution)
- [11E](#11e)
  - [a](#11e/a)
    - [Solution](#11e/a/solution)
  - [b](#11e/b)
    - [Solution](#11e/b/solution)
- [12G](#12g)
  - [a](#12g/a)
    - [Solution](#12g/a/solution)
  - [b](#12g/b)
    - [Solution](#12g/b/solution)
  - [c](#12g/c)
    - [Solution](#12g/c/solution)
- [13F](#13f)
  - [Solution](#13f/solution)
- [14B](#14b)
  - [Solution](#14b/solution)
- [15B](#15b)
  - [Solution](#15b/solution)
- [16A](#16a)
  - [Solution](#16a/solution)
- [17C](#17c)
  - [Solution](#17c/solution)
- [18C](#18c)
  - [a](#18c/a)
    - [Solution](#18c/a/solution)
  - [b](#18c/b)
    - [Solution](#18c/b/solution)
- [19H](#19h)
  - [a](#19h/a)
    - [Solution](#19h/a/solution)
  - [b](#19h/b)
    - [Solution](#19h/b/solution)
  - [c](#19h/c)
    - [Solution](#19h/c/solution)
- [20H](#20h)
  - [a](#20h/a)
    - [Solution](#20h/a/solution)
  - [b](#20h/b)
    - [Solution](#20h/b/solution)
  - [c](#20h/c)
    - [Solution](#20h/c/solution)

## 1F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1f/solution">Solution</h3>

↑ **Parent:** [1F](#1f)

A [basis](../../../vector-space.md#basis) of a [vector space](../../../vector-space.md) $V$ is a family of vectors that is both [linearly independent](../../../vector-space.md#linear-independence) and a [spanning set](../../../vector-space.md#spanning-set) of $V$.

Write the given finite basis as $\mathcal B=\{v_1,\ldots,v_n\}$. First, any other basis $\mathcal B'$ must also be finite. Each $v_i$ is a finite [linear combination](../../../vector-space.md#linear-combination) of elements of $\mathcal B'$, so the union $S$ of the finitely many elements of $\mathcal B'$ occurring in these $n$ expressions is finite. Since $S$ spans every $v_i$, it spans $V$. If some $w\in\mathcal B'\setminus S$ existed, then $w$ would lie in the span of $S$, contradicting the [linear independence](../../../vector-space.md#linear-independence) of $\mathcal B'$. Hence $\mathcal B'=S$; write $|\mathcal B'|=m$.

It remains to prove the elementary [Steinitz exchange lemma](../../../vector-space.md#steinitz-exchange-lemma) directly. If independent vectors $w_1,\ldots,w_r$ lie in the span of $v_1,\ldots,v_n$, express $w_1$ in terms of the $v_i$. Some coefficient is nonzero, so the corresponding $v_i$ can be solved for in terms of $w_1$ and the other $v_i$; replacing it by $w_1$ preserves the span. Inductively, after replacing $k$ of the $v_i$ by $w_1,\ldots,w_k$, the expression for $w_{k+1}$ must have a nonzero coefficient on one of the unreplaced $v_i$, since otherwise $w_{k+1}$ would be a linear combination of $w_1,\ldots,w_k$. That $v_i$ can again be replaced. There are only $n$ original vectors to replace, so $r\leq n$.

Apply this argument first to the independent family $\mathcal B'$ and the spanning family $\mathcal B$ to obtain $m\leq n$, and then with the two bases interchanged to obtain $n\leq m$. Therefore

$$
\boxed{|\mathcal B'|=|\mathcal B|}.
$$

## 2F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2f/solution">Solution</h3>

↑ **Parent:** [2F](#2f)

A [Laurent series](../../../analysis.md#laurent-series) about $a$ is an expansion

$$
f(z)=\sum_{n=-\infty}^{\infty}c_n(z-a)^n
$$

that converges to $f$ on an [annulus](../../../topology.md#annulus-mathematics) $r<|z-a|<R$.

The [partial fraction decomposition](../../../isolated-singularity.md#partial-fraction-decomposition) is

$$
\frac{10}{(z+2)(z^2+1)}
=\frac2{z+2}+\frac{4-2z}{z^2+1}.
$$

For $0<|z|<1$, expand both denominators by the [geometric series](../../../real-analysis.md#geometric-series):

$$
\boxed{f(z)=\sum_{n=0}^{\infty}\frac{(-1)^n}{2^n}z^n
+(4-2z)\sum_{k=0}^{\infty}(-1)^kz^{2k}}.
$$

This is actually a [Taylor series](../../../calculus.md#taylor-series) at zero, since the apparent puncture at zero contains no singularity.

For $1<|z|<2$, the $z+2$ term still expands in nonnegative powers, while the quadratic term must be expanded in negative powers:

$$
\frac{4-2z}{z^2+1}
=(4z^{-2}-2z^{-1})\frac1{1+z^{-2}}.
$$

Hence

$$
\boxed{f(z)=\sum_{n=0}^{\infty}\frac{(-1)^n}{2^n}z^n
+(4z^{-2}-2z^{-1})\sum_{k=0}^{\infty}(-1)^kz^{-2k}}.
$$

## 3E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3e/solution">Solution</h3>

↑ **Parent:** [3E](#3e)

The [Poincare disc model](../../../geometry-and-topology.md#poincare-disk-model) is

$$
D=\{z\in\mathbb C:|z|<1\},
\qquad
ds^2=\frac{4|dz|^2}{(1-|z|^2)^2}.
$$

This [Riemannian metric](../../../differential-geometry.md#riemannian-metric) has constant Gaussian curvature $-1$.

For $a\in D$ and $|\eta|=1$, the [Möbius transformation](../../../group-theory.md#mobius-transformation)

$$
T_{a,\eta}(z)=\eta\frac{z-a}{1-\overline a z}
$$

is an [isometry](../../../riemannian-geometry.md#isometry) of the disc, and every orientation-preserving disc isometry has this form. In particular, $T_{z_1,1}$ sends $z_1$ to zero and $z_2$ to a point of modulus

$$
\rho=\left|\frac{z_2-z_1}{1-\overline{z_1}z_2}\right|.
$$

Rotations are also isometries, so it remains only to integrate the metric along a radial geodesic from $0$ to $\rho$:

$$
d(0,\rho)=\int_0^\rho\frac{2\,dr}{1-r^2}
=2\operatorname{artanh}\rho.
$$

Thus the [Hyperbolic distance in the Poincare disc](../../../geometry-and-topology.md#hyperbolic-distance-in-the-poincare-disc) is

$$
\boxed{d(z_1,z_2)=2\operatorname{artanh}\left|\frac{z_2-z_1}{1-\overline{z_1}z_2}\right|
=\log\frac{1+\rho}{1-\rho}}.
$$

## 4A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4a/solution">Solution</h3>

↑ **Parent:** [4A](#4a)

Introduce the orthogonal coordinates

$$
u=\frac{x-z}{\sqrt2},
\qquad
v=\frac{x+z}{\sqrt2}.
$$

Then the constraint and objective become

$$
u^2+v^2+2y^2=1,
\qquad
\phi=\sqrt2uy.
$$

The [Lagrange multiplier](../../../mathematical-optimization.md#lagrange-multiplier) equations for a [stationary point](../../../calculus-of-variations.md#stationary-point) are

$$
\sqrt2y=2\lambda u,
\qquad
\sqrt2u=4\lambda y,
\qquad
0=2\lambda v.
$$

If $\lambda=0$, then $u=y=0$ and $v=\pm1$, giving

$$
(x,y,z)=\left(\frac1{\sqrt2},0,\frac1{\sqrt2}\right),
\quad
\left(-\frac1{\sqrt2},0,-\frac1{\sqrt2}\right).
$$

If $\lambda\ne0$, then $v=0$. The first two equations and the constraint imply

$$
\lambda=\pm\frac12,
\qquad
u=\pm\frac1{\sqrt2},
\qquad
y=\sqrt2\lambda u.
$$

Converting back to $(x,y,z)$ gives the other four points. Therefore all stationary points are

$$
\boxed{\left(\pm\frac1{\sqrt2},0,\pm\frac1{\sqrt2}\right)}
$$

with matching signs, together with

$$
\boxed{\left(\frac12,\frac12,-\frac12\right),
\left(-\frac12,-\frac12,\frac12\right),
\left(\frac12,-\frac12,-\frac12\right),
\left(-\frac12,\frac12,\frac12\right)}.
$$

The middle pair has $\phi=1/2$, the last pair has $\phi=-1/2$, and the first pair has $\phi=0$.

## 5C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5c/solution">Solution</h3>

↑ **Parent:** [5C](#5c)

Take $x$ down the plane and $y$ normally away from it, with the solid at $y=0$ and the [free surface](../../../fluid-mechanics.md#free-surface) at $y=h$. A steady unidirectional [falling film flow](../../../viscous-fluid-flow.md#falling-film-flow) has velocity $\mathbf u=u(y)\mathbf e_x$. The streamwise [Navier-Stokes equation](../../../viscous-fluid-flow.md#navier-stokes-equation) reduces to

$$
\nu u''=-g\sin\alpha,
$$

where $\nu$ is the [kinematic viscosity](../../../fluid-mechanics.md#kinematic-viscosity). The lower [no-slip boundary condition](../../../viscous-fluid-flow.md#no-slip-boundary-condition) and upper [stress-free boundary condition](../../../viscous-fluid-flow.md#stress-free-boundary-condition) are

$$
u(0)=0,
\qquad
u'(h)=0.
$$

Integrating gives the velocity profile

$$
\boxed{u(y)=\frac{g\sin\alpha}{\nu}\left(hy-\frac{y^2}{2}\right)}.
$$

The [volume flux](../../../fluid-mechanics.md#volumetric-flow-rate) per unit width is

$$
\boxed{Q=\int_0^hu(y)\,dy=\frac{g h^3\sin\alpha}{3\nu}}.
$$

If the upper surface is replaced by a stationary solid plane, the second boundary condition becomes $u(h)=0$. The resulting plane-channel profile and flux are

$$
u(y)=\frac{g\sin\alpha}{2\nu}y(h-y),
\qquad
\boxed{Q_{\rm closed}=\frac{g h^3\sin\alpha}{12\nu}=\frac14Q}.
$$

The free surface exerts no tangential [shear stress](../../../viscous-fluid-flow.md#shear-stress), whereas the stationary upper wall enforces no slip and exerts a retarding shear. This additional drag accounts for the reduced flux.

## 6C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6c/solution">Solution</h3>

↑ **Parent:** [6C](#6c)

For distinct [interpolation nodes](../../../numerical-analysis.md#interpolation-node) $x_0,\ldots,x_m$, define the degree-$m$ [divided difference](../../../numerical-analysis.md#divided-difference) by

$$
f[x_0,\ldots,x_m]
=\sum_{j=0}^m\frac{f(x_j)}{\prod_{\substack{0\leq k\leq m\\k\ne j}}(x_j-x_k)}.
$$

It is the leading coefficient of the unique degree-at-most-$m$ [interpolating polynomial](../../../numerical-analysis.md#polynomial-interpolation) through those data.

Define

$$
p_n(x)=f[x_0]+\sum_{m=1}^nf[x_0,\ldots,x_m]\prod_{i=0}^{m-1}(x-x_i).
$$

The partial polynomial $p_m$ agrees with $p_{m-1}$ at $x_0,\ldots,x_{m-1}$. Moreover, the explicit formula for the divided difference gives

$$
f[x_0,\ldots,x_m]
=\frac{f(x_m)-p_{m-1}(x_m)}{\prod_{i=0}^{m-1}(x_m-x_i)},
$$

so $p_m(x_m)=f(x_m)$. Induction shows that $p_n(x_j)=f(x_j)$ for every $j$. By uniqueness of [polynomial interpolation](../../../numerical-analysis.md#polynomial-interpolation), this is the required [Newton interpolation polynomial](../../../numerical-analysis.md#newton-polynomial).

For the recursion, substitute the explicit formulas for $f[x_1,\ldots,x_m]$ and $f[x_0,\ldots,x_{m-1}]$. For an interior index $j$, the coefficient of $f(x_j)$ in their difference is

$$
\frac1{(x_j-x_m)\prod_{\substack{1\leq k\leq m-1\\k\ne j}}(x_j-x_k)}
-\frac1{(x_j-x_0)\prod_{\substack{1\leq k\leq m-1\\k\ne j}}(x_j-x_k)}
=\frac{x_m-x_0}{\prod_{\substack{0\leq k\leq m\\k\ne j}}(x_j-x_k)}.
$$

The endpoint terms satisfy the same identity directly. Dividing by $x_m-x_0$ therefore gives

$$
\boxed{f[x_0,\ldots,x_m]
=\frac{f[x_1,\ldots,x_m]-f[x_0,\ldots,x_{m-1}]}{x_m-x_0}}.
$$

## 7H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7h/a">a</h3>

↑ **Parent:** [7H](#7h)

<h4 id="7h/a/solution">Solution</h4>

↑ **Parent:** [A](#7h/a)

For observations $x_1,\ldots,x_n$, the [log-likelihood](../../../statistical-modelling.md#log-likelihood) of the [normal distribution](../../../probability-theory.md#normal-distribution) model is

$$
\ell(\mu,\sigma^2)
=-\frac n2\log(2\pi\sigma^2)
-\frac1{2\sigma^2}\sum_{i=1}^n(x_i-\mu)^2.
$$

Differentiating first with respect to $\mu$ gives $\widehat\mu=\overline x$. Substituting this value and differentiating with respect to $\sigma^2$ gives the [normal mean and variance maximum-likelihood estimators](../../../statistical-modelling.md#normal-mean-and-variance-maximum-likelihood-estimators)

$$
\boxed{\widehat\mu=\overline X=\frac1n\sum_{i=1}^nX_i,
\qquad
\widehat{\sigma}^2=\frac1n\sum_{i=1}^n(X_i-\overline X)^2}.
$$

<h3 id="7h/b">b</h3>

↑ **Parent:** [7H](#7h)

<h4 id="7h/b/solution">Solution</h4>

↑ **Parent:** [B](#7h/b)

An [unbiased estimator](../../../statistical-modelling.md#unbiased-estimator) $T$ of a parameter $\theta$ satisfies $\mathbb E_\theta[T]=\theta$ for every permissible value of $\theta$. Since the [sample mean](../../../variance.md#sample-mean) is linear,

$$
\mathbb E[\widehat\mu]=\frac1n\sum_{i=1}^n\mathbb E[X_i]=\mu,
$$

so $\widehat\mu$ is unbiased.

Use the identity

$$
\sum_{i=1}^n(X_i-\overline X)^2
=\sum_{i=1}^n(X_i-\mu)^2-n(\overline X-\mu)^2.
$$

The two expectations on the right are $n\sigma^2$ and $n\operatorname{Var}(\overline X)=\sigma^2$, respectively. Hence

$$
\mathbb E[\widehat{\sigma}^2]=\frac{n-1}{n}\sigma^2.
$$

Thus

$$
\boxed{\widehat\mu\text{ is unbiased},
\qquad
\widehat{\sigma}^2\text{ has bias }-\frac{\sigma^2}{n}}.
$$

The unbiased [sample variance](../../../statistical-inference.md#sample-variance) instead divides the same sum of squares by $n-1$.

## 8H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8h/solution">Solution</h3>

↑ **Parent:** [8H](#8h)

Because $x^*$ is an interior minimizer of the differentiable function $f$, it satisfies $f'(x^*)=0$. Apply the [Taylor theorem with Lagrange remainder](../../../calculus.md#taylor-theorem-with-lagrange-remainder) to $f'$ about $x_n$. For some $y_n$ between $x_n$ and $x^*$,

$$
0=f'(x^*)
=f'(x_n)+f''(x_n)(x^*-x_n)
+\frac12f'''(y_n)(x^*-x_n)^2.
$$

The lower bound on $|f''|$ ensures that every step of the [Newton method](../../../mathematical-optimization.md#newton-s-method-in-optimization) is defined. Divide by $f''(x_n)$ and use

$$
x_{n+1}=x_n-\frac{f'(x_n)}{f''(x_n)}
$$

to obtain the exact error relation

$$
x^*-x_{n+1}
=-\frac{f'''(y_n)}{2f''(x_n)}(x^*-x_n)^2.
$$

The assumed derivative bounds now give the [quadratic convergence bound for Newton's method](../../../mathematical-optimization.md#quadratic-convergence-bound-for-newton-s-method)

$$
\boxed{|x^*-x_{n+1}|
\leq\frac{C_2}{2C_1}|x^*-x_n|^2}
$$

for every $n$.

## 9F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9f/a">a</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/a/solution">Solution</h4>

↑ **Parent:** [A](#9f/a)

The [adjugate matrix](../../../linear-algebra.md#adjugate-matrix) is the transpose of the cofactor matrix, and it satisfies

$$
M\operatorname{adj}(M)=\operatorname{adj}(M)M=(\det M)I.
$$

Put $M=tI-A$ and substitute the two given expansions into this identity:

$$
(tI-A)\sum_{i=0}^{n-1}B_it^{n-1-i}
=\sum_{j=0}^nc_jt^{n-j}I.
$$

Comparing coefficients of powers of $t$ gives

$$
\boxed{B_0=c_0I=I,
\qquad B_i=AB_{i-1}+c_iI\quad(1\leq i\leq n-1),
\qquad -AB_{n-1}=c_nI}.
$$

Here $c_0=1$ because the [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) is monic.

<h3 id="9f/b">b</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/b/solution">Solution</h4>

↑ **Parent:** [B](#9f/b)

Let $M(t_1,\ldots,t_n)=\operatorname{diag}(t_1,\ldots,t_n)-A$. Expanding the [determinant](../../../linear-algebra.md#determinant) along row $i$ shows that

$$
\frac{\partial p}{\partial t_i}=C_{ii}(M),
$$

where $C_{ii}$ is the corresponding cofactor. Since a diagonal entry of the [adjugate matrix](../../../linear-algebra.md#adjugate-matrix) is that same cofactor, the multivariable [chain rule](../../../calculus.md#chain-rule) along the diagonal $t_1=\cdots=t_n=t$ yields

$$
\frac d{dt}\det(tI-A)
=\sum_{i=1}^n\left.\frac{\partial p}{\partial t_i}\right|_{(t,\ldots,t)}
=\sum_{i=1}^n[\operatorname{adj}(tI-A)]_{ii}.
$$

Therefore

$$
\boxed{\frac d{dt}\det(tI-A)=\operatorname{Tr}(\operatorname{adj}(tI-A))}.
$$

<h3 id="9f/c">c</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/c/solution">Solution</h4>

↑ **Parent:** [C](#9f/c)

Taking the [matrix trace](../../../linear-algebra.md#matrix-trace) of the adjugate expansion and using part (b) gives

$$
\sum_{i=0}^{n-1}\operatorname{Tr}(B_i)t^{n-1-i}
=\sum_{i=0}^{n-1}(n-i)c_it^{n-1-i}.
$$

Hence $\operatorname{Tr}(B_i)=(n-i)c_i$. Taking traces in $B_i=AB_{i-1}+c_iI$ gives, for $1\leq i<n$,

$$
c_i=-\frac1i\operatorname{Tr}(AB_{i-1}).
$$

For $i=n$, the same formula follows by taking the trace of $-AB_{n-1}=c_nI$. Iterating the recursion from part (a) also gives

$$
B_{i-1}=A^{i-1}+c_1A^{i-2}+\cdots+c_{i-1}I.
$$

Consequently the [Faddeev–LeVerrier algorithm](../../../linear-operator-theory.md#faddeev-leverrier-algorithm) is

$$
\boxed{c_i=-\frac1i\left[\operatorname{Tr}(A^i)
+c_1\operatorname{Tr}(A^{i-1})+\cdots+c_{i-1}\operatorname{Tr}(A)\right],
\quad1\leq i\leq n}.
$$

Starting with $c_0=1$, this recursively expresses every $c_i$ using only $\operatorname{Tr}(A),\ldots,\operatorname{Tr}(A^i)$; these are the [Newton identities](../../../polynomial.md#newton-s-identities) for the [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial).

## 10G

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10g/a">a</h3>

↑ **Parent:** [10G](#10g)

<h4 id="10g/a/solution">Solution</h4>

↑ **Parent:** [A](#10g/a)

The group $G$ is a nontrivial [finite p-group](../../../finite-group-theory.md#finite-p-group), so the [nontrivial center of a finite p-group](../../../finite-group-theory.md#nontrivial-center-of-a-finite-p-group) gives $Z(G)\ne\{e\}$. If $Z(G)\ne G$, then $Z(G)$ is already a nontrivial proper [normal subgroup](../../../group-theory.md#normal-subgroup), so $G$ is not a [simple group](../../../finite-group-theory.md#simple-group). If $Z(G)=G$, then $G$ is [abelian](../../../group.md#abelian-group). By [Cauchy's theorem for finite groups](../../../finite-group-theory.md#cauchy-theorem-for-groups), it has a subgroup of order $p$; every subgroup of an abelian group is normal, and this subgroup is nontrivial and proper because $|G|=p^4$. Thus in every case

$$
\boxed{G\text{ is not simple}}.
$$

<h3 id="10g/b">b</h3>

↑ **Parent:** [10G](#10g)

<h4 id="10g/b/solution">Solution</h4>

↑ **Parent:** [B](#10g/b)

The [Sylow theorems](../../../finite-group-theory.md#sylow-theorems) state that if $|G|=p^am$ with $p\nmid m$, then:

- $G$ has a [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup) of order $p^a$;
- every $p$-subgroup is contained in a Sylow $p$-subgroup;
- all Sylow $p$-subgroups are conjugate;
- their number $n_p$ satisfies $n_p\mid m$ and $n_p\equiv1\pmod p$.

<h3 id="10g/c">c</h3>

↑ **Parent:** [10G](#10g)

<h4 id="10g/c/solution">Solution</h4>

↑ **Parent:** [C](#10g/c)

Interchange the two primes if necessary so that $p<q$. By the [Sylow theorems](../../../finite-group-theory.md#sylow-theorems), the number $n_q$ of Sylow $q$-subgroups satisfies

$$
n_q\mid p^2,
\qquad
n_q\equiv1\pmod q.
$$

If $n_q\ne1$, then $n_q$ is $p$ or $p^2$. The first is impossible because $1<p<q$. The second would imply

$$
q\mid p^2-1=(p-1)(p+1).
$$

Since $q>p$ is prime, it cannot divide $p-1$, so it must divide $p+1$. But $q>p$ then forces $q=p+1$, impossible because $p$ and $q$ are both odd. Therefore $n_q=1$. The unique Sylow $q$-subgroup is a nontrivial proper [normal subgroup](../../../group-theory.md#normal-subgroup), and hence

$$
\boxed{G\text{ is not simple}}.
$$

## 11E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="11e/a">a</h3>

↑ **Parent:** [11E](#11e)

<h4 id="11e/a/solution">Solution</h4>

↑ **Parent:** [A](#11e/a)

A map $f:A\to\mathbb R^m$ is differentiable at $p\in A$ when there is a [linear map](../../../vector-space.md#linear-map) $Df(p):\mathbb R^n\to\mathbb R^m$ such that

$$
f(p+h)=f(p)+Df(p)h+r(h),
\qquad
\frac{|r(h)|}{|h|}\longrightarrow0.
$$

The linear map $Df(p)$ is the [Fréchet derivative](../../../calculus.md#frechet-derivative) of $f$ at $p$.

The multivariable [chain rule](../../../calculus.md#chain-rule) states that if $f$ is differentiable at $p$ and $g$ is differentiable at $f(p)$, then

$$
\boxed{D(g\circ f)(p)=Dg(f(p))\circ Df(p)}.
$$

Indeed, write $f(p+h)=f(p)+Ah+r(h)$ and $g(f(p)+k)=g(f(p))+Bk+s(k)$, where $r(h)=o(|h|)$ and $s(k)=o(|k|)$. Since $k=Ah+r(h)=O(|h|)$,

$$
g(f(p+h))=g(f(p))+BAh+Br(h)+s(Ah+r(h)),
$$

and the last two terms are $o(|h|)$. This proves the formula.

For matrix inversion near the [identity matrix](../../../vector-space.md#identity-matrix),

$$
(I+h)^{-1}=I-h+h^2(I+h)^{-1}.
$$

The last term is $O(\|h\|^2)$ because inversion is bounded near $I$. Therefore the inversion map is differentiable at $I$ and

$$
\boxed{Df(I)(h)=-h}.
$$

<h3 id="11e/b">b</h3>

↑ **Parent:** [11E](#11e)

<h4 id="11e/b/solution">Solution</h4>

↑ **Parent:** [B](#11e/b)

For every invertible matrix $A$,

$$
(r_C\circ f\circ l_C)(A)
=r_C((CA)^{-1})
=A^{-1}C^{-1}C
=A^{-1}=f(A).
$$

The maps $l_C$ and $r_C$ are linear. Differentiate this identity at $A=I$ and use the [chain rule](../../../calculus.md#chain-rule) and part (a):

$$
r_C\bigl(Df(C)(Ch)\bigr)=-h.
$$

Thus $Df(C)(Ch)C=-h$. Given an arbitrary increment $k$, set $h=C^{-1}k$ to obtain the [derivative of matrix inversion](../../../calculus.md#derivative-of-matrix-inversion)

$$
\boxed{Df(C)(k)=-C^{-1}kC^{-1}}.
$$

This also proves differentiability at every $C\in V$.

## 12G

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12g/a">a</h3>

↑ **Parent:** [12G](#12g)

<h4 id="12g/a/solution">Solution</h4>

↑ **Parent:** [A](#12g/a)

Nonnegativity and symmetry are immediate. Moreover, $d(x,y)=0$ exactly when $n_{\min}(x,y)=\infty$, which means $x_n=y_n$ for every $n$.

For three sequences $x,y,z$, if $x$ and $y$ agree through coordinate $r-1$ and $y$ and $z$ agree through coordinate $s-1$, then $x$ and $z$ agree through coordinate $\min(r,s)-1$. Hence

$$
n_{\min}(x,z)\geq\min\{n_{\min}(x,y),n_{\min}(y,z)\},
$$

and therefore

$$
d(x,z)\leq\max\{d(x,y),d(y,z)\}\leq d(x,y)+d(y,z).
$$

**Thus $d$ is a [metric](../../../topological-analysis.md#metric); in fact, the stronger first inequality makes it an [ultrametric](../../../topological-analysis.md#ultrametric).**

<h3 id="12g/b">b</h3>

↑ **Parent:** [12G](#12g)

<h4 id="12g/b/solution">Solution</h4>

↑ **Parent:** [B](#12g/b)

A [metric space](../../../topological-analysis.md#metric-space) is [complete](../../../topological-analysis.md#completeness) when every [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) converges to a point of the space.

Let $x^{(1)},x^{(2)},\ldots$ be a Cauchy sequence in $X$, where $x^{(j)}=(x^{(j)}_1,x^{(j)}_2,\ldots)$. For each positive integer $N$, choose $J_N$ such that

$$
d(x^{(j)},x^{(k)})<2^{-N}
\qquad(j,k\geq J_N).
$$

This inequality says that the first $N$ coordinates of $x^{(j)}$ and $x^{(k)}$ agree. Consequently each coordinate $x_n^{(j)}$ is eventually constant. Let $x_n$ be its eventual value and put $x=(x_1,x_2,\ldots)\in X$.

For $j\geq J_N$, the first $N$ coordinates of $x^{(j)}$ agree with those of $x$, so

$$
d(x^{(j)},x)<2^{-N}.
$$

As $N$ is arbitrary, $x^{(j)}\to x$. Therefore

$$
\boxed{(X,d)\text{ is complete}}.
$$

<h3 id="12g/c">c</h3>

↑ **Parent:** [12G](#12g)

<h4 id="12g/c/solution">Solution</h4>

↑ **Parent:** [C](#12g/c)

For each $k$, the coordinate projection

$$
\pi_k:X\to\mathbb Z,
\qquad
\pi_k((x_n))=x_k,
$$

is continuous when $\mathbb Z$ has the [discrete topology](../../../topology.md#discrete-space): if $d(x,y)<2^{-k}$, then $x_k=y_k$.

If $\gamma:[0,1]\to X$ were a [continuous path](../../../geometry-and-topology.md#continuous-path), then $\pi_k\circ\gamma$ would be a continuous map from the connected interval $[0,1]$ to a discrete space, so it would be constant. This holds for every $k$, and therefore $\gamma$ itself must be constant. Since $X$ contains distinct points, no path joins every pair. Hence

$$
\boxed{(X,d)\text{ is not path connected};}
$$

indeed, every path component is a singleton.

## 13F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="13f/solution">Solution</h3>

↑ **Parent:** [13F](#13f)

[Jordan lemma](../../../complex-analysis.md#jordan-s-lemma) states that if $a>0$ and $g$ is analytic in the upper half-plane outside a fixed circle, with

$$
M_R=\max_{0\leq\theta\leq\pi}|g(Re^{i\theta})|\longrightarrow0,
$$

then on the upper semicircle $C_R$,

$$
\int_{C_R}e^{iaz}g(z)\,dz\longrightarrow0.
$$

Indeed, $|e^{iaRe^{i\theta}}|=e^{-aR\sin\theta}$. Using symmetry and $\sin\theta\geq2\theta/\pi$ on $0\leq\theta\leq\pi/2$ gives

$$
\left|\int_{C_R}e^{iaz}g(z)\,dz\right|
\leq2RM_R\int_0^{\pi/2}e^{-2aR\theta/\pi}\,d\theta
\leq\frac{\pi M_R}{a}\longrightarrow0.
$$

The [residue](../../../analysis.md#residue) of $f$ at an isolated singularity $a$ is the coefficient of $(z-a)^{-1}$ in its [Laurent series](../../../analysis.md#laurent-series), equivalently

$$
\operatorname{Res}(f,a)=\frac1{2\pi i}\oint f(z)\,dz.
$$

If $f(z)=g(z)/(z-a)^k$, the Taylor expansion of the analytic function $g$ shows that

$$
\boxed{\operatorname{Res}(f,a)=\frac{g^{(k-1)}(a)}{(k-1)!}}.
$$

For the real integral, apply [contour integration](../../../complex-analysis.md#contour-integration) in the upper half-plane to

$$
F(z)=\frac{z^3e^{iz}}{(1+z^2)^2}.
$$

Jordan's lemma removes the semicircular arc. The only enclosed singularity is the double pole at $z=i$, whose residue is

$$
\operatorname{Res}(F,i)
=\left.\frac d{dz}\left(\frac{z^3e^{iz}}{(z+i)^2}\right)\right|_{z=i}
=\frac1{4e}.
$$

The [residue theorem](../../../analysis.md#residue-theorem) therefore gives

$$
\int_{-\infty}^{\infty}\frac{x^3e^{ix}}{(1+x^2)^2}\,dx
=\frac{\pi i}{2e}.
$$

Its real part vanishes because $x^3\cos x/(1+x^2)^2$ is an [odd function](../../../calculus.md#odd-function), while its imaginary part is the requested integral. Hence

$$
\boxed{\int_{-\infty}^{\infty}\frac{x^3\sin x}{(1+x^2)^2}\,dx=\frac\pi{2e}}.
$$

## 14B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="14b/solution">Solution</h3>

↑ **Parent:** [14B](#14b)

Since $x=r\cos\theta$, the function on the left of the defining expansion is $e^{ix}$. Therefore

$$
(\nabla^2+1)e^{ir\cos\theta}
=(\partial_x^2+\partial_y^2+1)e^{ix}=0,
$$

which is the two-dimensional [Helmholtz equation](../../../partial-differential-equation.md#helmholtz-equation).

In polar coordinates,

$$
\nabla^2=\frac{\partial^2}{\partial r^2}
+\frac1r\frac\partial{\partial r}
+\frac1{r^2}\frac{\partial^2}{\partial\theta^2}.
$$

Substitute the defining [Fourier cosine series](../../../fourier-series.md#fourier-cosine-series) and equate the coefficient of each $\cos(n\theta)$. Its angular second derivative contributes $-n^2$, so every [Bessel function](../../../analysis.md#bessel-function) $J_n$ satisfies

$$
J_n''+\frac1rJ_n'+\left(1-\frac{n^2}{r^2}\right)J_n=0,
$$

or equivalently the [Bessel differential equation](../../../analysis.md#bessel-differential-equation)

$$
\boxed{r^2J_n''+rJ_n'+(r^2-n^2)J_n=0}.
$$

Expand the exponential through cubic order and use

$$
\cos^2\theta=\frac{1+\cos2\theta}{2},
\qquad
\cos^3\theta=\frac{3\cos\theta+\cos3\theta}{4}.
$$

This gives

$$
e^{ir\cos\theta}
=1-\frac{r^2}{4}
+i\left(r-\frac{r^3}{8}\right)\cos\theta
-\frac{r^2}{4}\cos2\theta
-\frac{ir^3}{24}\cos3\theta+O(r^4).
$$

Comparing with $J_0+2\sum_{n\geq1}i^nJ_n\cos(n\theta)$ yields

$$
\boxed{J_0(r)=1-\frac{r^2}{4}+O(r^4)},
$$



$$
\boxed{J_1(r)=\frac r2-\frac{r^3}{16}+O(r^5),
\quad J_2(r)=\frac{r^2}{8}+O(r^4),
\quad J_3(r)=\frac{r^3}{48}+O(r^5)}.
$$

## 15B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="15b/solution">Solution</h3>

↑ **Parent:** [15B](#15b)

The [Time-dependent Schrödinger equation](../../../physics.md#time-dependent-schrodinger-equation) for the one-dimensional [Quantum harmonic oscillator](../../../quantum-mechanics.md#quantum-harmonic-oscillator) is

$$
i\hbar\frac{\partial\Psi}{\partial t}
=\left(-\frac{\hbar^2}{2m}\frac{\partial^2}{\partial x^2}
+\frac12m\omega^2x^2\right)\Psi.
$$

A [stationary state](../../../quantum-mechanics.md#stationary-state) has $\Psi(x,t)=\psi(x)e^{-iEt/\hbar}$, so cancellation of the common time factor gives

$$
-\frac{\hbar^2}{2m}\psi''+\frac12m\omega^2x^2\psi=E\psi.
$$

Set

$$
y=\sqrt{\frac{m\omega}{\hbar}}x,
\qquad
\epsilon=\frac{2E}{\hbar\omega}.
$$

The equation becomes

$$
\boxed{-\frac{d^2\psi}{dy^2}+y^2\psi=\epsilon\psi}.
$$

With $\psi=f(y)e^{-y^2/2}$,

$$
\psi''=\left[f''-2yf'+(y^2-1)f\right]e^{-y^2/2},
$$

and hence $f$ obeys the [Hermite differential equation](../../../analysis.md#hermite-differential-equation)

$$
\boxed{f''-2yf'+(\epsilon-1)f=0}.
$$

If $f$ is monic of degree $N$, the coefficient of $y^N$ in this equation is $\epsilon-1-2N$. It must vanish, so

$$
\boxed{\epsilon=2N+1,
\qquad E=\hbar\omega\left(N+\frac12\right)}.
$$

Writing $f=\sum_{k=0}^Na_ky^k$ gives the recurrence

$$
a_{k+2}=\frac{2(k-N)}{(k+2)(k+1)}a_k.
$$

The coefficient of $y^{N-1}$ first gives $a_{N-1}=0$, and the recurrence preserves parity. If $N$ is even, every odd coefficient vanishes, so $f$ is an [even function](../../../calculus.md#even-function). The Gaussian factor is also even; therefore the stationary state $\psi$ has even [parity](../../../quantum-mechanics.md#parity).

## 16A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="16a/solution">Solution</h3>

↑ **Parent:** [16A](#16a)

Use $\mathbf E=-\nabla\phi$ and [Gauss's law](../../../electromagnetism.md#gauss-s-law) $\nabla\cdot\mathbf E=\rho/\epsilon_0$. The [divergence theorem](../../../calculus.md#divergence-theorem) and the decay at infinity give

$$
\int\rho\phi\,dV
=\epsilon_0\int\phi\nabla\cdot\mathbf E\,dV
=\epsilon_0\int\nabla\cdot(\phi\mathbf E)\,dV
-\epsilon_0\int\mathbf E\cdot\nabla\phi\,dV
=\epsilon_0\int|\mathbf E|^2\,dV.
$$

Multiplying by $1/2$ proves that the two expressions for the [electrostatic energy](../../../electromagnetism.md#electrostatic-energy) agree.

The uniform volume charge density in the thick shell is

$$
\rho_0=\frac{3Q}{4\pi(b^3-a^3)}.
$$

Spherical symmetry and the integral form of Gauss's law give

$$
\boxed{
\mathbf E(r)=
\begin{cases}
0,&0\leq r<a,\\[2mm]
\displaystyle\frac{Q}{4\pi\epsilon_0}
\frac{r^3-a^3}{(b^3-a^3)r^2}\,\widehat{\mathbf r},&a\leq r\leq b,\\[3mm]
\displaystyle\frac{Q}{4\pi\epsilon_0r^2}\,\widehat{\mathbf r},&r>b.
\end{cases}}
$$

Thus $|\mathbf E|$ is zero inside, rises continuously through the charged region, reaches $Q/(4\pi\epsilon_0b^2)$ at $b$, and then decays as $r^{-2}$. Taking $\phi(\infty)=0$ and integrating $E=-d\phi/dr$ gives

$$
\phi(r)=
\begin{cases}
\phi(a),&r<a,\\[1mm]
\displaystyle\frac{Q}{4\pi\epsilon_0}\left[\frac1b+
\frac{(b^2-r^2)/2+a^3(1/b-1/r)}{b^3-a^3}\right],&a\leq r\leq b,\\[3mm]
\displaystyle\frac{Q}{4\pi\epsilon_0r},&r>b.
\end{cases}
$$

The [electric potential](../../../electromagnetism.md#electric-potential) is continuous, constant inside, decreases smoothly across the charge, and continues as $1/r$ outside.

As $b\to a$, the charge becomes a surface shell. Then

$$
\mathbf E=\begin{cases}0,&r<a,\\ Q\widehat{\mathbf r}/(4\pi\epsilon_0r^2),&r>a,
\end{cases}
\qquad
\phi=\begin{cases}Q/(4\pi\epsilon_0a),&r\leq a,\\ Q/(4\pi\epsilon_0r),&r\geq a.
\end{cases}
$$

The potential remains continuous, but the normal electric field jumps by $Q/(4\pi\epsilon_0a^2)$ across the [surface charge density](../../../electromagnetism.md#surface-charge-density).

The field-energy expression gives

$$
U=\frac{\epsilon_0}{2}\int_a^\infty
\left(\frac{Q}{4\pi\epsilon_0r^2}\right)^2,4\pi r^2\,dr
=\frac{Q^2}{8\pi\epsilon_0a}
=\frac12Q\phi(a).
$$

The charge-potential expression gives the same result directly because the entire charge lies where the potential equals $\phi(a)$:

$$
U=\frac12\int\rho\phi\,dV=\frac12Q\phi(a).
$$

This is the [electrostatic energy of a uniformly charged spherical shell](../../../electromagnetism.md#electrostatic-energy-of-a-uniformly-charged-spherical-shell).

Since $\phi(a)=Q/(4\pi\epsilon_0a)$ is proportional to $Q$,

$$
\delta U=\delta\left(\frac{Q^2}{8\pi\epsilon_0a}\right)
=\boxed{\phi(a)\,\delta Q}
$$

to first order. This is the [work](../../../classical-mechanics.md#work) required to bring the additional charge $\delta Q$ from infinity to the potential created by the charge already present.

## 17C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="17c/solution">Solution</h3>

↑ **Parent:** [17C](#17c)

For an [incompressible flow](../../../fluid-mechanics.md#incompressible-flow), $\nabla\cdot\mathbf u=0$. If the flow is also irrotational, then locally $\mathbf u=\nabla\phi$ for a [velocity potential](../../../fluid-mechanics.md#velocity-potential), and therefore

$$
\nabla^2\phi=\nabla\cdot\mathbf u=0.
$$

The boundary conditions are

$$
\left.\frac{\partial\phi}{\partial r}\right|_{r=a}=0,
\qquad
\nabla\phi\longrightarrow U\mathbf e_x\quad(r\to\infty),
\qquad
\int_0^{2\pi}\frac{\partial\phi}{\partial\theta}\,d\theta=\kappa.
$$

The fluid region is not simply connected, so a potential may change by the constant $\kappa$ after one circuit while its gradient remains single-valued. Superposing uniform flow, the cylinder doublet, and the circulation gives the [potential flow around a circular cylinder with circulation](../../../fluid-mechanics.md#potential-flow-around-a-circular-cylinder-with-circulation)

$$
\boxed{\phi(r,\theta)=U\left(r+\frac{a^2}{r}\right)\cos\theta+\frac\kappa{2\pi}\theta}.
$$

Its velocity components are

$$
u_r=U\left(1-\frac{a^2}{r^2}\right)\cos\theta,
\qquad
u_\theta=-U\left(1+\frac{a^2}{r^2}\right)\sin\theta+\frac\kappa{2\pi r}.
$$

On $r=a$, $u_r=0$ and, with $\lambda=\kappa/(4\pi Ua)$,

$$
u_\theta=2U(\lambda-\sin\theta).
$$

The [Bernoulli equation](../../../fluid-mechanics.md#bernoulli-equation) gives $p=p_\infty+\rho(U^2-u_\theta^2)/2$. The pressure force per unit length on the cylinder is

$$
\mathbf F=-a\int_0^{2\pi}p\,\mathbf e_r\,d\theta
=\frac{\rho a}{2}\int_0^{2\pi}u_\theta^2(\cos\theta\,\mathbf e_x+\sin\theta\,\mathbf e_y)\,d\theta.
$$

The $x$ component vanishes by symmetry, while $\int_0^{2\pi}\sin^2\theta\,d\theta=\pi$ gives

$$
\boxed{\mathbf F=-4\pi\rho aU^2\lambda\,\mathbf e_y=-\rho\kappa U\,\mathbf e_y},
$$

in agreement with the [Kutta–Joukowski theorem](../../../fluid-mechanics.md#kutta-joukowski-theorem).

A [stagnation point](../../../fluid-mechanics.md#stagnation-point) satisfies $u_r=u_\theta=0$. On the cylinder this means $\sin\theta=\lambda$. Thus $|\lambda|<1$ gives two surface stagnation points, $|\lambda|=1$ gives one coincident surface point, and $|\lambda|>1$ gives none on the surface. Away from the cylinder, $u_r=0$ requires $\cos\theta=0$. Solving $u_\theta=0$ then gives one physical exterior root when $|\lambda|>1$:

$$
\boxed{r=a\left(|\lambda|+\sqrt{\lambda^2-1}\right),
\qquad
\theta=\begin{cases}\pi/2,&\lambda>1,\\3\pi/2,&\lambda<-1.
\end{cases}}
$$

At $|\lambda|=1$ this root lies on $r=a$ and agrees with the single surface point.

## 18C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="18c/a">a</h3>

↑ **Parent:** [18C](#18c)

<h4 id="18c/a/solution">Solution</h4>

↑ **Parent:** [A](#18c/a)

Insert the exact solution into the [linear multistep method](../../../numerical-analysis.md#linear-multistep-method) and expand about $t_n$. Its defect is

$$
\sum_{l=0}^s\rho_l y(t_n+lh)-h\sum_{l=0}^s\sigma_l y'(t_n+lh).
$$

The coefficient of $h^k y^{(k)}(t_n)$ is

$$
\frac1{k!}\sum_l\rho_l l^k-\frac1{(k-1)!}\sum_l\sigma_l l^{k-1}
$$

for $k\geq1$, while the constant coefficient is $\sum_l\rho_l$. The method has order at least $p$ exactly when these coefficients vanish for $0\leq k\leq p$.

On the other hand,

$$
\rho(e^z)-z\sigma(e^z)
=\sum_l\rho_l e^{lz}-z\sum_l\sigma_l e^{lz}.
$$

The coefficient of $z^k$ in this expression is precisely the preceding order-condition coefficient. Therefore all coefficients through degree $p$ vanish exactly when

$$
\boxed{\rho(e^z)-z\sigma(e^z)=O(z^{p+1})},
$$

which proves the equivalence.

<h3 id="18c/b">b</h3>

↑ **Parent:** [18C](#18c)

<h4 id="18c/b/solution">Solution</h4>

↑ **Parent:** [B](#18c/b)

For this [Adams–Moulton method](../../../numerical-analysis.md#adams-moulton-method), the [characteristic polynomials of a linear multistep method](../../../numerical-analysis.md#characteristic-polynomials-of-a-linear-multistep-method) are

$$
\rho(w)=w^2-w,
\qquad
\sigma(w)=\frac{5w^2+8w-1}{12}.
$$

Expansion at zero gives

$$
\rho(e^z)-z\sigma(e^z)=-\frac1{24}z^4+O(z^5).
$$

Part (a) therefore shows that the method has order exactly three.

It is consistent because its order is at least one. The roots of $\rho(w)=w(w-1)$ are $0$ and $1$; both lie in the closed unit disk, and the only unit-modulus root is simple. Thus the method is [zero-stable](../../../numerical-analysis.md#zero-stability). By the [Dahlquist equivalence theorem](../../../numerical-analysis.md#dahlquist-equivalence-theorem), consistency and zero stability imply convergence. Hence the method is

$$
\boxed{\text{third-order and convergent}}.
$$

## 19H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="19h/a">a</h3>

↑ **Parent:** [19H](#19h)

<h4 id="19h/a/solution">Solution</h4>

↑ **Parent:** [A](#19h/a)

The [Neyman-Pearson lemma](../../../statistical-modelling.md#neyman-pearson-lemma) says that for simple hypotheses with densities $f_0,f_1$, a size-$\alpha$ test that rejects where $f_1/f_0>k$ and accepts where $f_1/f_0<k$, with possible randomization on equality to attain size $\alpha$, is most powerful among all tests of size at most $\alpha$. To prove it, let $\varphi^*$ be this test and $\varphi$ any competing test. Pointwise,

$$
(\varphi^*-\varphi)(f_1-kf_0)\geq0.
$$

After integration,

$$
\mathbb E_1\varphi^*-\mathbb E_1\varphi
\geq k(\mathbb E_0\varphi^*-\mathbb E_0\varphi)\geq0,
$$

which proves maximal power.

For the exponential sample, with $S=\sum_iX_i=n\overline X$,

$$
\frac{L(\lambda_1)}{L(\lambda_0)}
=\left(\frac{\lambda_1}{\lambda_0}\right)^n
\exp\bigl((\lambda_0-\lambda_1)S\bigr).
$$

Since $\lambda_1<\lambda_0$, this ratio is increasing in $S$. The [likelihood-ratio test](../../../statistical-modelling.md#likelihood-ratio-test) therefore rejects for large $\overline X$:

$$
\boxed{R_\alpha=\{\overline X>c_\alpha\},
\qquad
1-G_{n,\lambda_0}(nc_\alpha)=\alpha},
$$

where $G_{n,\lambda}$ is the distribution function of the rate-parameterized [Gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution) $\Gamma(n,\lambda)$.

<h3 id="19h/b">b</h3>

↑ **Parent:** [19H](#19h)

<h4 id="19h/b/solution">Solution</h4>

↑ **Parent:** [B](#19h/b)

The [power function](../../../statistical-modelling.md#power-function-of-a-statistical-test) of a test is the probability of rejection as a function of the true parameter. Since $S=n\overline X\sim\Gamma(n,\lambda)$,

$$
\boxed{\beta(\lambda)=\mathbb P_\lambda(\overline X>c_\alpha)
=1-G_{n,\lambda}(nc_\alpha)}.
$$

At the null value, $\beta(\lambda_0)=\alpha$.

<h3 id="19h/c">c</h3>

↑ **Parent:** [19H](#19h)

<h4 id="19h/c/solution">Solution</h4>

↑ **Parent:** [C](#19h/c)

A level-$\alpha$ test is [uniformly most powerful](../../../statistical-modelling.md#uniformly-most-powerful-test) for a composite alternative when its power is at least that of every other level-$\alpha$ test at every parameter value in that alternative.

For every fixed $\lambda_1<\lambda_0$, the likelihood ratio is increasing in the same statistic $S$, and the size-$\alpha$ threshold is always the null quantile $nc_\alpha$, independent of $\lambda_1$. The [Neyman-Pearson lemma](../../../statistical-modelling.md#neyman-pearson-lemma) therefore makes the test from part (a) most powerful against every individual $\lambda_1<\lambda_0$. Consequently it is

$$
\boxed{\text{uniformly most powerful for }H_0:\lambda=\lambda_0
\text{ against }\widetilde H_1:\lambda<\lambda_0}.
$$

## 20H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="20h/a">a</h3>

↑ **Parent:** [20H](#20h)

<h4 id="20h/a/solution">Solution</h4>

↑ **Parent:** [A](#20h/a)

By the definition of conditional probability and [stationarity](../../../markov-process.md#stationary-distribution),

$$
P^*(x,y)
=\frac{\mathbb P(X_0=y,X_1=x)}{\mathbb P(X_1=x)}
=\boxed{\frac{\pi(y)P(y,x)}{\pi(x)}}.
$$

This is the transition matrix of the [time-reversed Markov chain](../../../markov-process.md#time-reversed-markov-chain).

<h3 id="20h/b">b</h3>

↑ **Parent:** [20H](#20h)

<h4 id="20h/b/solution">Solution</h4>

↑ **Parent:** [B](#20h/b)

Conditional on $X_0=x$, the random variable $T$ is the [first return time](../../../markov-process.md#first-return-time) $T_x^+$. The [Kac's lemma](../../../probability-and-statistics.md#kac-s-lemma) mean-recurrence formula for a finite [irreducible Markov chain](../../../markov-process.md#irreducible-markov-chain) gives

$$
\mathbb E_xT_x^+=\frac1{\pi(x)}.
$$

Averaging over $X_0\sim\pi$ therefore yields

$$
\boxed{\mathbb E[T]=\sum_x\pi(x)\frac1{\pi(x)}=N}.
$$

<h3 id="20h/c">c</h3>

↑ **Parent:** [20H](#20h)

<h4 id="20h/c/solution">Solution</h4>

↑ **Parent:** [C](#20h/c)

Let the common initial state be $x$ and the robber's final state be $y$. Part (a) gives their joint distribution as

$$
\pi(x)P^*(x,y)=\pi(y)P(y,x).
$$

Let $\tau_y=\min\{n\geq0:X_n=y\}$ be the cop's [hitting time](../../../markov-process.md#first-passage-time) of $y$ when starting from $x$. For a chain started from $y$, condition on its first step to obtain

$$
\mathbb E_yT_y^+=1+\sum_xP(y,x)\mathbb E_x\tau_y.
$$

Hence the expected catch time, averaged over the displayed joint law, is

$$
\sum_{x,y}\pi(y)P(y,x)\mathbb E_x\tau_y
=\sum_y\pi(y)\left(\mathbb E_yT_y^+-1\right).
$$

Using [Kac's lemma](../../../probability-and-statistics.md#kac-s-lemma) once more gives

$$
\boxed{\mathbb E[\text{catch time}]
=\sum_y\pi(y)\left(\frac1{\pi(y)}-1\right)=N-1}.
$$

The convention $\tau_y=0$ correctly counts an immediate catch when the robber's reverse step leaves it at the common starting state.

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
