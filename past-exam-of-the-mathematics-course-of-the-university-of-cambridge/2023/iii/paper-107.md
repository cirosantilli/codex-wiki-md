# Paper 107

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_107.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_107.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [Solution](#2/solution)
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
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
    - [iii](#3/b/iii)
      - [Solution](#3/b/iii/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)
    - [iii](#4/b/iii)
      - [Solution](#4/b/iii/solution)
    - [iv](#4/b/iv)
      - [Solution](#4/b/iv/solution)
    - [v](#4/b/v)
      - [Solution](#4/b/v/solution)
    - [vi](#4/b/vi)
      - [Solution](#4/b/vi/solution)

## 1

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Fix $x\in\Omega$ and $R<\operatorname{dist}(x,\partial\Omega)$. The [mean value property for harmonic functions](../../../partial-differential-equation.md#mean-value-property-for-harmonic-functions) is

$$
u(x)=\frac1{|\partial B_r|}\int_{\partial B_r(x)}u\,dS
=\frac1{|B_r|}\int_{B_r(x)}u\,dy
\qquad(0<r\leq R).
$$

To prove the spherical identity, translate $x$ to the origin and put $F(r)=|S^{n-1}|^{-1}\int_{S^{n-1}}u(r\theta)\,dS_\theta$. The [divergence theorem](../../../calculus.md#divergence-theorem) gives

$$
F'(r)=\frac1{|S^{n-1}|r^{n-1}}\int_{B_r}\Delta u\,dy=0.
$$

**Hence $F(r)=\lim_{s\downarrow0}F(s)=u(0)$. Integrating the spherical identity in polar coordinates gives the ball identity.**

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

Choose $0<r<\operatorname{dist}(x,\partial\Omega)$. Differentiating the ball mean-value formula with respect to its centre and then using the [divergence theorem](../../../calculus.md#divergence-theorem) gives

$$
D_i u(x)=\frac1{|B_r|}\int_{B_r(x)}D_i u(y)\,dy
=\frac1{|B_r|}\int_{\partial B_r(x)}u(y)\nu_i(y)\,dS_y.
$$

Consequently the [interior derivative estimate for a harmonic function](../../../partial-differential-equation.md#interior-derivative-estimate-for-a-harmonic-function) yields

$$
|\nabla u(x)|\leq \frac{C_n}{r}\sup_{B_r(x)}|u|
\leq \frac{C_n}{r}\sup_\Omega|u|.
$$

The constant may depend on $x$ and its distance from the boundary, but it is independent of $u$.

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

Take a nonnegative radial [mollifier](../../../distribution-theory.md#mollifier) $\eta_\varepsilon$ supported in $B_\varepsilon(0)$, with $\varepsilon<\operatorname{dist}(x,\partial\Omega)$. Writing the convolution in polar coordinates and applying the spherical [mean value property for harmonic functions](../../../partial-differential-equation.md#mean-value-property-for-harmonic-functions) at every radius shows directly that

$$
(u*\eta_\varepsilon)(x)=u(x).
$$

The convolution is [smooth](../../../analysis.md#smooth-function), so $u$ agrees locally with a smooth function. Since $x$ was arbitrary, $u\in C^\infty(\Omega)$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Choose a [cutoff function](../../../distribution-theory.md#cutoff-function) $\eta$ supported in $B_\rho(x)$, equal to one on $B_{\rho'}(x)$, and satisfying $|D\eta|\leq(\rho-\rho')^{-1}$. Use $\eta^2u$ as a [test function](../../../distribution-theory.md#test-function) in the [weak formulation](../../../partial-differential-equation.md#weak-formulation):

$$
0=\int D u\mathbin\cdot D(\eta^2u)
=\int\eta^2|Du|^2+2\int\eta u,Du\mathbin\cdot D\eta.
$$

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) followed by [Young inequality](../../../nonlinear-analysis.md#young-s-inequality-for-products) gives

$$
\int\eta^2|Du|^2\leq4\int u^2|D\eta|^2,
$$

and hence

$$
\int_{B_{\rho'}(x)}|Du|^2
\leq\frac{4}{(\rho-\rho')^2}\int_{B_\rho(x)}|u|^2.
$$

This is the [Caccioppoli inequality](../../../partial-differential-equation.md#caccioppoli-inequality). The numerical constant is convention-dependent and is normally absorbed into the displayed estimate; replacing the radii by fixed intermediate radii gives the stated form with one universal constant.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

On a relatively compact ball, mollification commutes with the [Laplacian](../../../calculus.md#laplacian), so $u_\varepsilon=u*\eta_\varepsilon$ is a smooth harmonic function. Repeated [interior derivative estimates](../../../partial-differential-equation.md#interior-derivative-estimate-for-a-harmonic-function), together with the [Caccioppoli inequality](../../../partial-differential-equation.md#caccioppoli-inequality), bound every derivative of $u_\varepsilon$ on a smaller ball by the local $L^2$ norm of $u$, uniformly as $\varepsilon\downarrow0$. The [Arzelà-Ascoli theorem](../../../topological-analysis.md#arzela-ascoli-theorem) and a diagonal argument give a smooth local limit, while mollification gives $u_\varepsilon\to u$ in $L^2_{\rm loc}$. Thus the limit equals $u$ almost everywhere. After choosing this smooth representative, $u$ is harmonic pointwise. This is the [Weyl lemma](../../../partial-differential-equation.md#weyl-lemma) for an $H^1$ weak solution.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For $u\in L^2_{\rm loc}(\Omega)$, the correct formulation is the [distributional identity](../../../distribution-theory.md#distributional-identity)

$$
\int_\Omega u\,\Delta\varphi\,dx=0
\qquad\text{for every }\varphi\in C_c^\infty(\Omega).
$$

**Thus $\Delta u=0$ as a [distribution](../../../distribution-theory.md#distribution-mathematical-analysis). The [Weyl lemma](../../../partial-differential-equation.md#weyl-lemma) applies already to locally integrable distributions, so $u$ agrees almost everywhere with a smooth harmonic function.**

## 2

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Uniform ellipticity means that there is $\lambda>0$ such that the symmetric part of the principal coefficient matrix satisfies

$$
a^{ij}(x)\xi_i\xi_j\geq\lambda|\xi|^2
$$

for every $x\in\Omega$ and $\xi\in\mathbb R^n$. This is the defining coercive bound for a [uniformly elliptic operator](../../../elliptic-boundary-value-problem.md#uniformly-elliptic-operator).

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Assume $c\leq0$, the coefficients are bounded, and $u$ is bounded above. Choose $\kappa$ so large that the bounded positive function $q(y)=e^{\kappa y}$ satisfies

$$
Lq=(a^{nn}\kappa^2+y\kappa+c)q\geq m>0.
$$

Also set $\psi(x)=\log(1+|x|^2)$. Boundedness of the coefficients, $x\mathbin\cdot D\psi\leq2$, and $c\leq0$ give a global upper bound $L\psi\leq C$.

For $\varepsilon>0$ and $0<\delta<\varepsilon m/C$, the function

$$
v=u+\varepsilon q-\delta\psi
$$

tends to $-\infty$ as $|x|\to\infty$ and satisfies $Lv>0$. If $v$ exceeded both zero and its values on $y=\pm1$, it would attain a positive interior maximum. At that point $Dv=0$ and $D^2v\leq0$, whence $Lv\leq cv\leq0$, a contradiction. Letting $\delta\downarrow0$ and then $\varepsilon\downarrow0$ proves

$$
\sup_\Omega u\leq\max\{0,\sup_{\partial\Omega}u\}.
$$

This is the [weak maximum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators) on the slab. The boundedness or a comparable growth condition is necessary because the domain is unbounded.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [weak maximum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators) fails without a condition at infinity. The function

$$
u(x)=x_n
$$

is harmonic on the upper half-space, continuous on its closure, and vanishes on the boundary, but it is positive and unbounded in the interior.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For $n\geq3$, the radial function

$$
u(x)=1-|x|^{2-n}
$$

is harmonic on $\mathbb R^n\setminus\overline{B_1(0)}$, vanishes on the unit sphere, and is positive in the domain. It therefore violates the [weak maximum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators). In two dimensions the corresponding counterexample is $u(x)=\log|x|$, since the [fundamental solution of the Laplace equation](../../../partial-differential-equation.md#fundamental-solution-of-the-laplace-equation) changes from a power to a logarithm.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Take

$$
L=\frac{d^4}{dx^4}-1.
$$

Its [principal symbol](../../../partial-differential-equation.md#principal-symbol-of-a-partial-differential-equation) is $\xi^4$, so it is elliptic, and $a_4a_0=-1<0$. Yet $u(x)=\sin x$ satisfies $Lu=0$ on $(0,\pi)$ and vanishes at both boundary points while remaining positive inside. Thus second-order ellipticity is essential to the usual [weak maximum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators).

## 3

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

First replace $u$ by $u+\varepsilon$ and later let $\varepsilon\downarrow0$. In the weak subsolution inequality use the admissible truncations approximating $\eta^2u^{\alpha-1}$. Uniform ellipticity, the coefficient bound, [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality), and [Young inequality](../../../nonlinear-analysis.md#young-s-inequality-for-products) give

$$
(\alpha-1)\lambda\int\eta^2u^{\alpha-2}|Du|^2
\leq2\Lambda\int\eta u^{\alpha-1}|Du||D\eta|
$$

and therefore

$$
\int|Du|^2u^{\alpha-2}\eta^2
\leq\frac{C(\lambda,\Lambda)}{(\alpha-1)^2}\int u^\alpha|D\eta|^2.
$$

Apply the [Sobolev embedding theorem](../../../sobolev-space.md#sobolev-embedding-theorem) to $w=\eta u^{\alpha/2}$. The preceding estimate yields, for concentric balls $B_r\subset B_R\subset B_1$,

$$
\|u\|_{L^{\alpha\sigma}(B_r)}
\leq\left(\frac{C\alpha^2}{(\alpha-1)^2(R-r)^2}\right)^{1/\alpha}
\|u\|_{L^\alpha(B_R)}.
$$

Starting with $\alpha=p>1$, taking $\alpha_k=p\sigma^k$, and choosing radii decreasing to $1/2$, the product of constants converges because $\sum_k\alpha_k^{-1}<\infty$. Letting $k\to\infty$ proves

$$
\sup_{B_{1/2}}u\leq C(n,\lambda,\Lambda,p)\|u\|_{L^p(B_1)}.
$$

This exponent-raising argument is [Moser iteration](../../../elliptic-boundary-value-problem.md#moser-iteration).

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

Use the [Weak Harnack inequality](../../../elliptic-boundary-value-problem.md#weak-harnack-inequality): for some $q>1$ and every nonnegative weak supersolution,

$$
\|u\|_{L^q(B_{1/2})}\leq C\inf_{B_{1/4}}u,
$$

where $C$ and $q$ depend only on $n,\lambda,\Lambda$. A weak solution is both a subsolution and a supersolution. Applying part (i), after rescaling from $B_1$ to $B_{1/2}$, and then the weak Harnack inequality gives

$$
\sup_{B_{1/4}}u
\leq C\|u\|_{L^q(B_{1/2})}
\leq C\inf_{B_{1/4}}u.
$$

This is the [Harnack inequality for uniformly elliptic divergence-form equations](../../../elliptic-boundary-value-problem.md#harnack-inequality-for-uniformly-elliptic-divergence-form-equations).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

For a compactly supported variation $v+t\phi$, differentiation of the area functional at $t=0$ gives the [first variation](../../../calculus-of-variations.md#first-variation)

$$
0=\left.\frac d{dt}\right|_{t=0}\int\sqrt{1+|D(v+t\phi)|^2}
=\int\frac{Dv\mathbin\cdot D\phi}{\sqrt{1+|Dv|^2}}.
$$

After [integration by parts](../../../calculus.md#integration-by-parts), this is the [minimal surface equation for a graph](../../../second-fundamental-form.md#minimal-surface-equation-for-a-graph)

$$
D_i\left(\frac{D_iv}{\sqrt{1+|Dv|^2}}\right)=0.
$$

For $v_R(x)=R^{-1}v(Rx)$ one has $Dv_R(x)=Dv(Rx)$. The equation is invariant under this scaling, so $v_R$ solves it on $B_1$ for every $R>0$.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

Differentiate the equation for $v_R$ with respect to $x_k$. The derivative $w=D_kv_R$ is a weak solution of

$$
D_i\bigl(a^{ij}(Dv(Rx))D_jw\bigr)=0,
$$

where

$$
a^{ij}(p)=\frac{\delta^{ij}}{\sqrt{1+|p|^2}}
-\frac{p_ip_j}{(1+|p|^2)^{3/2}}.
$$

The eigenvalue in the direction of $p$ is $(1+|p|^2)^{-3/2}$ and every orthogonal eigenvalue is $(1+|p|^2)^{-1/2}$. Thus a uniform bound on $|Dv|$ makes this a [uniformly elliptic operator](../../../elliptic-boundary-value-problem.md#uniformly-elliptic-operator) with constants independent of $R$.

<h4 id="3/b/iii">iii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/b/iii)

Suppose $|Dv|\leq M$. The coefficient matrices in part (ii) then have uniform ellipticity constants depending only on $M$. Applying the [Harnack inequality for uniformly elliptic divergence-form equations](../../../elliptic-boundary-value-problem.md#harnack-inequality-for-uniformly-elliptic-divergence-form-equations) to the nonnegative solutions $M+D_kv_R$ and $M-D_kv_R$ gives a scale-independent oscillation contraction

$$
\operatorname{osc}_{B_{1/4}}D_kv_R
\leq\theta\operatorname{osc}_{B_1}D_kv_R,
\qquad0<\theta<1.
$$

Scaling back,

$$
\operatorname{osc}_{B_{R/4}}D_kv
\leq\theta\operatorname{osc}_{B_R}D_kv.
$$

For fixed $r$, iterate this estimate with $R=4^mr$ and use the global bound $|D_kv|\leq M$ to obtain $\operatorname{osc}_{B_r}D_kv\leq2M\theta^m\to0$. Every partial derivative is therefore constant, so $v(x)=a\mathbin\cdot x+b$ is an [affine function](../../../vector-space.md#affine-function). This is a bounded-gradient Bernstein theorem for entire minimal graphs.

## 4

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Choose smooth boundary data $\varphi_j$ converging uniformly to $\varphi$, and let $v_j$ be their harmonic extensions. The [maximum principle for harmonic functions](../../../partial-differential-equation.md#maximum-principle-for-harmonic-functions) gives

$$
\|v_j-v_k\|_{C^0(\overline B)}
\leq\|\varphi_j-\varphi_k\|_{C^0(\partial B)},
$$

so $v_j$ converges uniformly on $\overline B$ to a continuous function $v$ with boundary value $\varphi$. Interior derivative estimates make the convergence smooth on compact subsets of $B$, hence $v$ is harmonic there. Uniqueness follows by applying the maximum principle to the difference of two solutions.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

Let $B\Subset\Omega$ and let $h$ be the harmonic function whose boundary values are $\max(u_1,u_2)$. The harmonic extensions $(u_i)_B$ satisfy $(u_i)_B\leq h$ by the [maximum principle for harmonic functions](../../../partial-differential-equation.md#maximum-principle-for-harmonic-functions), while subharmonicity gives $u_i\leq(u_i)_B$ in $B$. Hence $\max(u_1,u_2)\leq h$, proving that the maximum of two [subharmonic functions](../../../partial-differential-equation.md#subharmonic-function) is subharmonic.

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

The difference $u_1-u_2$ is subharmonic. If $M=\max_{\overline\Omega}(u_1-u_2)>0$, its maximum set lies in $\Omega$. At any point of this set, comparison with the harmonic replacement on a small ball and the [strong maximum principle for harmonic functions](../../../partial-differential-equation.md#strong-maximum-principle-for-harmonic-functions) show that the whole ball belongs to the maximum set. The set is therefore both open and closed in the connected domain $\Omega$, so it is all of $\Omega$, contradicting the boundary inequality. Thus $u_1\leq u_2$ throughout $\Omega$. This is the comparison principle for subharmonic and superharmonic functions.

<h4 id="4/b/iii">iii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/b/iii)

The constant $m=\min_{\partial\Omega}\varphi$ is subharmonic and lies below the boundary data, so the Perron family is nonempty. The constant $M=\max_{\partial\Omega}\varphi$ is superharmonic. Part (ii) gives $u\leq M$ for every member $u$ of the family, while the member $m$ gives the lower bound. Hence

$$
m\leq\overline u(x)\leq M,
$$

so the pointwise supremum is finite and well-defined.

<h4 id="4/b/iv">iv</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#4/b/iv)

Fix $B\Subset\Omega$ and $x_0\in B$. Choose $u_j$ in the Perron family with $u_j(x_0)\uparrow\overline u(x_0)$, replace successive terms by finite maxima using part (i), and take their harmonic lifts on $B$. The lifts remain in the family, are increasing, and are uniformly bounded. Interior estimates and the [Arzelà-Ascoli theorem](../../../topological-analysis.md#arzela-ascoli-theorem) give a harmonic limit $h$ on $B$ with $h\leq\overline u$ and $h(x_0)=\overline u(x_0)$.

If $h(y)<\overline u(y)$ somewhere in $B$, take another family member larger than $h(y)$ and repeat the maximum-and-lift construction. Its harmonic limit $H$ satisfies $H\geq h$ and $H(x_0)=h(x_0)$. The [strong minimum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#strong-minimum-principle-for-elliptic-operators) forces $H=h$, contradicting the strict inequality at $y$. Thus $h=\overline u$ on $B$. Since $B$ was arbitrary, $\overline u$ is smooth and harmonic in $\Omega$. This is the [Perron method for the Dirichlet problem](../../../analysis.md#perron-method).

<h4 id="4/b/v">v</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/v/solution">Solution</h5>

↑ **Parent:** [V](#4/b/v)

Fix $\varepsilon>0$ and choose a boundary neighbourhood $U$ of $z$ on which $|\varphi-\varphi(z)|<\varepsilon$. The positive continuous barrier $w$ has a positive minimum $m$ on the compact set $\partial\Omega\setminus U$. Choosing $A$ large enough makes

$$
\varphi(z)-\varepsilon-Aw\leq\varphi
\leq\varphi(z)+\varepsilon+Aw
$$

on all of $\partial\Omega$. The left function is subharmonic and belongs to the Perron family; the right function is superharmonic and dominates every family member by part (ii). Therefore

$$
\varphi(z)-\varepsilon-Aw(x)leq\overline u(x)
\leq\varphi(z)+\varepsilon+Aw(x).
$$

As $x\to z$, continuity gives $w(x)\to0$. Letting $\varepsilon\downarrow0$ proves $\overline u(x)\to\varphi(z)$. Such a $w$ is a [barrier for the Dirichlet problem](../../../analysis.md#barrier-for-the-dirichlet-problem), and $z$ is a [regular boundary point](../../../analysis.md#regular-boundary-point).

<h4 id="4/b/vi">vi</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/vi/solution">Solution</h5>

↑ **Parent:** [Vi](#4/b/vi)

Every boundary point of $D$ satisfies the [exterior sphere condition](../../../analysis.md#exterior-sphere-condition). For a point on the inner spherical boundary, use a smaller ball inside the removed ball and tangent at that point; for a point on the cube, use a ball in a supporting exterior half-space. If the exterior ball has centre $y$ and radius $r$, a local positive harmonic barrier is

$$
w(x)=r^{2-n}-|x-y|^{2-n}
$$

for $n\geq3$, while in two dimensions use $w(x)=\log(|x-y|/r)$. Adding a sufficiently large positive multiple of a global superharmonic function extends the local barrier across the bounded domain. Hence every boundary point is regular by part (v), and the [Perron method for the Dirichlet problem](../../../analysis.md#perron-method) produces a harmonic function attaining the prescribed continuous boundary data. The [maximum principle for harmonic functions](../../../partial-differential-equation.md#maximum-principle-for-harmonic-functions) gives uniqueness.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
