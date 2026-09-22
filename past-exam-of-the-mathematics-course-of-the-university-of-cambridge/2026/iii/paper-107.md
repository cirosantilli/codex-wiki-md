# Paper 107

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20107.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20107.pdf)

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
  - [e](#4/e)
    - [Solution](#4/e/solution)

## 1

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [mean value property for harmonic functions](../../../partial-differential-equation.md#mean-value-property-for-harmonic-functions) says that whenever $\overline{B_r(x_0)}\subset\Omega$,

$$
u(x_0)=\frac1{|B_r|}\int_{B_r(x_0)}u
=\frac1{|\partial B_r|}\int_{\partial B_r(x_0)}u.
$$

If $u$ attains its maximum $M$ at an interior point, the average of the nonnegative function $M-u$ over every sufficiently small centred ball is zero. Continuity makes $u=M$ on each such ball, and connectedness propagates this equality throughout the domain. Applying the same argument to $-u$ proves the [strong maximum principle for harmonic functions](../../../partial-differential-equation.md#strong-maximum-principle-for-harmonic-functions).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Differentiate the ball mean-value formula and use the [divergence theorem](../../../calculus.md#divergence-theorem):

$$
Du(x_0)=\frac1{|B_r|}\int_{B_r(x_0)}Du
=\frac1{|B_r|}\int_{\partial B_r(x_0)}u\nu.
$$

Consequently

$$
|Du(x_0)|\leq\frac{|\partial B_r|}{|B_r|}\sup_{B_r(x_0)}|u|
=\frac nr\sup_{B_r(x_0)}|u|.
$$

**Thus one may take $C(n)=n$.**

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Iteration gives the [interior derivative estimate for a harmonic function](../../../partial-differential-equation.md#interior-derivative-estimate-for-a-harmonic-function)

$$
|D^{k+1}u(x_0)|\leq C(n,k)R^{-(k+1)}\sup_{B_R(x_0)}|u|.
$$

The growth hypothesis bounds the right side by $C'R^{\alpha-1}+o(1)$, which tends to zero as $R\to\infty$. Thus every derivative of order $k+1$ vanishes everywhere. The [Taylor theorem](../../../calculus.md#taylor-theorem) makes $u$ a polynomial of degree at most $k$, proving the [polynomial-growth Liouville theorem for harmonic functions](../../../partial-differential-equation.md#polynomial-growth-liouville-theorem-for-harmonic-functions).

## 2

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Join the [Laplace operator](../../../partial-differential-equation.md#laplace-operator) to the target operator by

$$
L_tu=((1-t)\delta_{ij}+ta_{ij})\partial_{ij}u,
\qquad0\leq t\leq1.
$$

The family has one ellipticity constant. The global [Schauder estimate](../../../elliptic-boundary-value-problem.md#schauder-estimates) and the maximum principle give, uniformly in $t$,

$$
\lVert u\rVert_{C^{2,\alpha}(\overline\Omega)}
\leq C\lVert L_tu\rVert_{C^\alpha(\overline\Omega)}
$$

for zero boundary data. Let $I$ contain those $t$ for which $L_t:C_0^{2,\alpha}\to C^\alpha$ is onto. The assumed Laplace solvability gives $0\in I$; the [bounded inverse theorem](../../../functional-analysis.md#bounded-inverse-theorem) and small perturbations make $I$ open; and the uniform estimate plus compactness of lower Hölder embeddings makes $I$ closed. The [method of continuity](../../../elliptic-boundary-value-problem.md#method-of-continuity) yields $I=[0,1]$. At $t=1$ this gives the required solution, and the maximum principle gives uniqueness.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The strict maximum principle applied to $a_{ij}\partial_{ij}u=f>0$ with zero boundary data gives $u<0$ in $\Omega$. On $\Omega'$ set $w=v-u$. Then $a_{ij}\partial_{ij}w=0$, while $w=-u\geq0$ on $\partial\Omega'$ and this boundary value is positive somewhere because $\Omega'$ is proper. Hence $w>0$ inside and $w(y_0)=0$. The [Hopf boundary point lemma](../../../elliptic-boundary-value-problem.md#hopf-lemma) at this boundary minimum gives

$$
D_\nu w(y_0)<0.
$$

**Therefore $D_\nu v(y_0)-D_\nu u(y_0)<0$, proving the normal derivatives are unequal.**

## 3

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [Campanato space](../../../sobolev-space.md#campanato-space) $\mathcal L^{p,\mu}(\Omega)$ consists of $f\in L^p(\Omega)$ for which

$$
[f]_{\mathcal L^{p,\mu}}^p
=\sup_{x_0,r}r^{-\mu}\int_{\Omega\cap B_r(x_0)}
|f-f_{\Omega\cap B_r(x_0)}|^p<\infty,
$$

where $f_E=|E|^{-1}\int_Ef$. On a smooth bounded domain,

$$
\mathcal L^{p,n+p\alpha}(\Omega)=C^{0,\alpha}(\overline\Omega)
$$

with equivalent norms for $0<\alpha\leq1$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Fix $B_R(x_0)\subset B_1$, put $A_0=A(x_0)$, and let $v$ have the same boundary values as $u$ while solving $\operatorname{div}(A_0\nabla v)=0$. Then $w=u-v\in W_0^{1,2}(B_R)$ satisfies

$$
\operatorname{div}(A_0\nabla w)
=\operatorname{div}((A_0-A(x))\nabla u).
$$

Since $u\in C^1$ gives $|Du|\leq L$ locally, the supplied energy estimate and [Hölder continuity](../../../sobolev-space.md#holder-space) of $A$ yield

$$
\int_{B_R}|\nabla w|^2\leq C L^2[A]_{C^\alpha}^2R^{n+2\alpha}.
$$

The constant-coefficient decay estimate gives

$$
\int_{B_\rho}|\nabla v-(\nabla v)_{B_\rho}|^2
\leq C(\rho/R)^{n+2}
\int_{B_R}|\nabla v-(\nabla v)_{B_R}|^2.
$$

Thus, for $\Phi(r)=\int_{B_r}|\nabla u-(\nabla u)_{B_r}|^2$,

$$
\Phi(\rho)\leq C(\rho/R)^{n+2}\Phi(R)+CR^{n+2\alpha}.
$$

Because $n+2>n+2\alpha$, the [Campanato iteration lemma](../../../sobolev-space.md#campanato-iteration-lemma) gives $\Phi(\rho)\leq C\rho^{n+2\alpha}$ on balls in $B_{1/2}$. Hence $\nabla u\in\mathcal L^{2,n+2\alpha}=C^{0,\alpha}$ and $u\in C^{1,\alpha}(B_{1/2})$.

## 4

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A minimizing sequence in $\operatorname{Lip}_g(\Omega,k)$ is uniformly bounded and equi-Lipschitz. The [Arzelà-Ascoli theorem](../../../topological-analysis.md#arzela-ascoli-theorem) gives a uniformly convergent subsequence with limit $u$ having the same boundary data and Lipschitz constant at most $k$. Its gradients have a weak-star convergent subsequence in $L^\infty$, with limit $Du$. Convexity of $F$ makes the integral functional weak-star lower semicontinuous, so

$$
\mathcal F[u]\leq\liminf_j\mathcal F[u_j].
$$

**Thus $u$ attains the infimum by the [direct method in the calculus of variations](../../../calculus-of-variations.md#direct-method-in-the-calculus-of-variations).**

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let $L=\operatorname{Lip}(u)<k$ and take $v\in\operatorname{Lip}_g(\Omega)$. For small $t>0$, $u_t=(1-t)u+tv$ has Lipschitz constant at most $(1-t)L+t\operatorname{Lip}(v)<k$. Constrained minimality and convexity give

$$
\mathcal F[u]\leq\mathcal F[u_t]
\leq(1-t)\mathcal F[u]+t\mathcal F[v].
$$

Cancellation gives $\mathcal F[u]\leq\mathcal F[v]$, so $u$ is an unconstrained minimizer.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Let $H=\sup_{\overline B_1}\lVert D^2g\rVert$. For $x,x_0\in\partial B_1$, the [Taylor theorem with Lagrange remainder](../../../calculus.md#taylor-theorem-with-lagrange-remainder) and $|x-x_0|^2=2x_0\mathbin\cdot(x_0-x)$ give

$$
|g(x)-g(x_0)-Dg(x_0)\mathbin\cdot(x-x_0)|
\leq Hx_0\mathbin\cdot(x_0-x).
$$

Therefore

$$
b_{x_0}^{\pm}(x)=g(x_0)+Dg(x_0)\mathbin\cdot(x-x_0)
\pm Hx_0\mathbin\cdot(x_0-x)
$$

are affine upper and lower barriers, agree with $g$ at $x_0$, and have Lipschitz constant at most $K=\sup_{\overline B_1}|Dg|+H$. Thus $g$ has the [bounded slope condition](../../../calculus-of-variations.md#bounded-slope-condition).

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

For $y\in\partial\Omega$, let $b_y^-\leq g\leq b_y^+$ be the affine barriers from the [bounded slope condition](../../../calculus-of-variations.md#bounded-slope-condition). Their constant gradients satisfy the [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation), so they minimize the autonomous convex functional for their own boundary values. The [comparison principle](../../../calculus-of-variations.md#comparison-principle-for-convex-variational-integrals) gives

$$
b_y^-(x)\leq u(x)\leq b_y^+(x).
$$

Since both barriers equal $u(y)$ at $y$ and are $K$-Lipschitz,

$$
|u(x)-u(y)|\leq K|x-y|
$$

for $x\in\Omega$ and $y\in\partial\Omega$. The supplied boundary-to-interior criterion now gives $\operatorname{Lip}(u)\leq K$.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Part c supplies a [bounded slope condition](../../../calculus-of-variations.md#bounded-slope-condition) constant $K$. Choose $k>K$. Parts a and d give a constrained minimizer with $\operatorname{Lip}(u)\leq K<k$, and part b makes it a minimizer over all of $\operatorname{Lip}_g(B_1)$.

For $F(\xi)=\sqrt{1+|\xi|^2}$, the [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) is the [minimal surface equation for a graph](../../../second-fundamental-form.md#minimal-surface-equation-for-a-graph)

$$
\operatorname{div}\left(\frac{Du}{\sqrt{1+|Du|^2}}\right)=0.
$$

The Lipschitz bound confines $Du$ to a compact set on which $D^2F$ is uniformly positive definite, so the equation is uniformly elliptic. Interior regularity gives $C^{1,\alpha}$ first, and repeated [Schauder estimates](../../../elliptic-boundary-value-problem.md#schauder-estimates) then give smoothness in the interior.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
