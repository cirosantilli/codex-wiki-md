# Paper 157

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_157.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_157.pdf)

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
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 157](paper-157.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A family $\mathcal F$ of holomorphic or meromorphic functions on a domain $U$ is a [normal family](../../../complex-dynamics.md#normal-family) if every sequence in $\mathcal F$ has a subsequence converging locally uniformly in the spherical metric to a meromorphic function or to infinity. [Montel theorem](../../../complex-dynamics.md#montel-s-theorem) states that a family of meromorphic functions omitting three fixed points of the Riemann sphere is normal; for plane-valued holomorphic functions, two omitted values suffice.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Suppose first that $|E|\geq3$. Complete invariance implies that every iterate maps $\widehat{\mathbb C}\setminus E$ into itself. Hence the family $\{f^n\}$ omits the same three points of $E$ on this open set. By [Montel theorem](../../../complex-dynamics.md#montel-s-theorem),

$$
\widehat{\mathbb C}\setminus E\subseteq F(f),
$$

so

$$
\boxed{J(f)\subseteq E}.
$$

If $E$ consists of one or two points, complete invariance makes $f$ permute those points and makes every preimage of them remain in $E$. Some iterate fixes each point and is totally ramified there. In a local coordinate it therefore has the form $w\mapsto aw^m+O(w^{m+1})$ with $m\geq2$, so the point is superattracting for that iterate and belongs to the [Fatou set](../../../complex-dynamics.md#fatou-set). This proves the [completely invariant closed set of a rational map](../../../complex-dynamics.md#completely-invariant-closed-set-of-a-rational-map) dichotomy.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let $J'$ be the set of accumulation points of $J(f)$. It is closed. Since a rational map is open and has finite local degree, images and preimages of convergent sequences of distinct Julia points show that

$$
f^{-1}(J')=J'.
$$

Thus $J'$ is completely invariant. If $J'$ were a proper subset of $J(f)$, part b would imply $|J'|\leq2$ and $J'\subseteq F(f)$. Since $J'\subseteq J(f)$, this forces $J'=\varnothing$.

On the other hand, $J(f)$ is infinite: if it had at most two points, applying part b to the completely invariant set $J(f)$ would put it inside the Fatou set. Every infinite compact subset of the sphere has an accumulation point, so $J'\ne\varnothing$. This contradiction proves that $J'=J(f)$ and hence the [Julia set has no isolated points](../../../complex-dynamics.md#julia-set-has-no-isolated-points).

## 2

↑ **Parent:** [Paper 157](paper-157.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $z_0$ be attracting and let $U$ be its immediate basin. If $z_0$ itself is critical there is nothing to prove. Otherwise suppose $U$ contains no critical point. The restriction $f:U\to U$ is then an unbranched covering. Since the complement of $U$ contains the Julia set and hence at least three points, $U$ is hyperbolic. Lift the covering to the universal cover $\mathbb D\to U$, choosing a lift that fixes a point above $z_0$. Because both maps are universal coverings, the lift is an automorphism of $\mathbb D$. A disc automorphism fixing an interior point has derivative of hyperbolic norm one there, whereas the multiplier at $z_0$ has modulus strictly below one. This contradiction proves that $U$ contains a critical point, whose orbit converges to $z_0$. Thus every [attracting fixed point attracts a critical point](../../../complex-dynamics.md#attracting-fixed-point-attracts-a-critical-point).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [fixed Fatou component classification](../../../complex-dynamics.md#fixed-fatou-component-classification) has four cases:

- An immediate attracting or superattracting basin contains a critical point whose forward orbit converges to the attracting cycle.
- An immediate parabolic basin contains a critical point whose forward orbit converges to the parabolic cycle along an attracting direction.
- A Siegel disc is conformally conjugate to an irrational rotation of a disc. It contains no critical point, and its boundary is contained in the closure of the [postcritical set](../../../complex-dynamics.md#postcritical-set).
- A Herman ring is conformally conjugate to an irrational rotation of an annulus. It contains no critical point, and both boundary components are contained in the closure of the postcritical set.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Choose a $d$th root of unity $r\ne1$ far enough from one that $d|1-r|>1$, put $a=1-r$, and define

$$
f(z)=1-\frac a{z^d}.
$$

This map has degree $d$ and only two critical points, $0$ and infinity, each of multiplicity $d-1$. Their orbits are

$$
0\longmapsto\infty\longmapsto1\longmapsto r\longmapsto r.
$$

The multiplier at $r$ is

$$
f'(r)=\frac{ad}{r^{d+1}}=\frac{d(1-r)}r,
$$

whose modulus exceeds one. Thus every critical orbit lands at a repelling fixed point.

An attracting or parabolic periodic Fatou component would capture a critical orbit, contrary to the displayed dynamics. A Siegel disc or Herman ring would have boundary in the closure of the postcritical set, but that set is finite and contained in the repelling grand orbit, whereas a rotation-domain boundary is infinite. By the [Sullivan no-wandering-domain theorem](../../../complex-dynamics.md#no-wandering-domain-theorem), every Fatou component is eventually periodic, so the classification leaves no Fatou component. Therefore this [rational map with Julia set equal to the Riemann sphere](../../../complex-dynamics.md#rational-map-with-julia-set-equal-to-the-riemann-sphere) satisfies

$$
\boxed{J(f)=\widehat{\mathbb C}}.
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Take the degree-$d$ [Chebyshev polynomial](../../../numerical-analysis.md#chebyshev-polynomial) $T_d$, characterized by

$$
T_d(\cos\theta)=\cos(d\theta).
$$

Its Julia set is the interval $[-1,1]$. The complement $\widehat{\mathbb C}\setminus[-1,1]$ is connected, and it is exactly the basin of infinity. Hence $T_d$ has exactly one Fatou component. This is the [Chebyshev polynomial Julia set](../../../complex-dynamics.md#chebyshev-polynomial-julia-set) example.

## 3

↑ **Parent:** [Paper 157](paper-157.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For $f(z)=a_dz^d+\cdots$, the [Böttcher coordinate](../../../complex-dynamics.md#bottcher-coordinate) at infinity is the conformal coordinate $\phi_f$ defined near infinity by

$$
\phi_f(f(z))=\phi_f(z)^d,
\qquad
\phi_f(z)\sim a_d^{1/(d-1)}z.
$$

Its modulus has a dynamically natural extension to the entire basin of infinity

$$
A_\infty(f)=\{z:f^n(z)\to\infty\}.
$$

The [escape-rate Green function of a polynomial](../../../complex-dynamics.md#escape-rate-green-function-of-a-polynomial) is

$$
G_f(z)=\lim_{n\to\infty}\frac1{d^n}\log^+|f^n(z)|.
$$

It is zero on the filled Julia set $K(f)$, positive and harmonic on $A_\infty(f)$, and satisfies $G_f(f(z))=dG_f(z)$. Near infinity,

$$
G_f(z)=\log|\phi_f(z)|,
$$

so $e^{G_f}$ is precisely the extension of $|\phi_f|$ throughout the basin.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Assume $J(f)$ is connected. Then the filled Julia set $K(f)$ is connected and full, so its complement $A_\infty(f)$ is simply connected. The local Bottcher coordinate therefore extends by the functional equation to a conformal isomorphism

$$
\phi_f:A_\infty(f)\longrightarrow\{w:|w|>1\}.
$$

If a finite critical point $c$ lay in $A_\infty(f)$, differentiating

$$
\phi_f(f(z))=\phi_f(z)^d
$$

at $c$ would give

$$
0=d\phi_f(c)^{d-1}\phi_f'(c).
$$

Neither factor on the right vanishes on the exterior disc under a conformal coordinate, a contradiction. Hence every finite critical point lies in $K(f)$. This is one direction of the [connected Julia set criterion for a polynomial](../../../complex-dynamics.md#connected-julia-set-criterion-for-a-polynomial).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For $f_c(z)=z^2+c$, the Mandelbrot set is the set of parameters for which the critical orbit of zero is bounded. If $c$ lies outside it, the critical value $c$ is in the basin of infinity and one defines the parameter Bottcher map

$$
\Phi(c)=\phi_c(c).
$$

The dynamical functional equation, holomorphic dependence on $c$, and the normalization at infinity show that $\Phi$ is a proper degree-one holomorphic map

$$
\mathbb C\setminus M\longrightarrow\mathbb C\setminus\overline{\mathbb D}.
$$

It is therefore a conformal isomorphism. Since the exterior disc is connected and simply connected, the complement of $M$ has no bounded component; equivalently, the [Mandelbrot set connectedness from the parameter Böttcher coordinate](../../../complex-dynamics.md#mandelbrot-set-connectedness-from-the-parameter-bottcher-coordinate) proves that $M$ is connected.

## 4

↑ **Parent:** [Paper 157](paper-157.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [holomorphic fixed-point index](../../../complex-dynamics.md#holomorphic-fixed-point-index), or residue index, is

$$
\iota(f,z_0)=\operatorname*{Res}_{z=z_0}\frac1{z-f(z)}.
$$

For a simple fixed point with multiplier $\lambda\ne1$ it equals $1/(1-\lambda)$. Three distinct fixed points of a quadratic rational map are simple, and the rational fixed-point formula gives

$$
\frac1{1-\lambda_0}+\frac1{1-\lambda_1}+\frac1{1-\lambda_2}=1.
$$

If, say, $\lambda_0\lambda_1=1$, then

$$
\frac1{1-\lambda_0}+\frac1{1-\lambda_0^{-1}}=1.
$$

The remaining term would have to be zero, which is impossible. Thus the [multiplier relation for three distinct fixed points of a quadratic rational map](../../../complex-dynamics.md#multiplier-relation-for-three-distinct-fixed-points-of-a-quadratic-rational-map) is

$$
\boxed{\lambda_i\lambda_j\ne1\quad(i\ne j)}.
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The parabolic basin $A$ is open and lies in $F(g)$. Suppose $z\in\partial A\cap F(g)$ and let $U$ be the Fatou component containing $z$. A small neighborhood of $z$ in $U$ meets $A$. On one point of $U$, the iterates eventually enter the chosen attracting petal and converge to zero along its attracting vector. Normality and the identity theorem for the limiting iterates make the same true throughout the connected component $U$. Hence $U\subseteq A$, which is impossible for a boundary point. Therefore the [parabolic basin](../../../complex-dynamics.md#parabolic-basin) satisfies

$$
\boxed{\partial A\subseteq J(g)}.
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Let $p$ be prime and define

$$
P_p(c)=f_c^p(0).
$$

The recursion $P_{n+1}=P_n^2+c$ shows that $P_p$ has degree $2^{p-1}$. Moreover $P_p(c)=c+O(c^2)$ at zero, so $c=0$ is a simple root. Since the degree is greater than one, $P_p$ has a nonzero root $c_0$. At $c_0$, the critical point zero is periodic with period dividing $p$. It is not fixed because $c_0\ne0$, so primality makes its exact period $p$. Thus $c_0$ is the center of a [hyperbolic component](../../../complex-dynamics.md#hyperbolic-component) of exact period $p$.

The multiplier map on this component covers the unit disc. Move to its boundary along parameters whose attracting-cycle multiplier tends to $-1$. Compactness of the Mandelbrot set gives a limiting parameter $c_*$. The periodic cycle persists with exact period $p$: at multiplier $-1$, every point is a simple root of $f_{c_*}^p(z)-z$, so no collision to a lower-period orbit occurs. Its multiplier is the root of unity $-1$, and hence it is a [parabolic cycle](../../../complex-dynamics.md#parabolic-cycle) after squaring the return map. We have produced a parabolic cycle of exact period $p$ for every prime $p$. Therefore the [parabolic periods in the quadratic family](../../../complex-dynamics.md#parabolic-periods-in-the-quadratic-family) form an infinite set.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
