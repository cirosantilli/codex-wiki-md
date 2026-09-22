# Paper 5

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_5.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_5.pdf)

**Table of contents**

- [1](#1)
  - [1](#1/1)
    - [a](#1/1/a)
      - [Solution](#1/1/a/solution)
    - [b](#1/1/b)
      - [Solution](#1/1/b/solution)
    - [c](#1/1/c)
      - [Solution](#1/1/c/solution)
  - [2](#1/2)
    - [a](#1/2/a)
      - [Solution](#1/2/a/solution)
    - [b](#1/2/b)
      - [Solution](#1/2/b/solution)
  - [3](#1/3)
    - [a](#1/3/a)
      - [Solution](#1/3/a/solution)
    - [b](#1/3/b)
      - [Solution](#1/3/b/solution)
    - [c](#1/3/c)
      - [Solution](#1/3/c/solution)
    - [d](#1/3/d)
      - [Solution](#1/3/d/solution)
    - [e](#1/3/e)
      - [Solution](#1/3/e/solution)
    - [f](#1/3/f)
      - [Solution](#1/3/f/solution)
    - [g](#1/3/g)
      - [Solution](#1/3/g/solution)
- [2](#2)
  - [1](#2/1)
    - [Solution](#2/1/solution)
  - [2](#2/2)
    - [Solution](#2/2/solution)
  - [3](#2/3)
    - [Solution](#2/3/solution)
  - [4](#2/4)
    - [Solution](#2/4/solution)
  - [5](#2/5)
    - [Solution](#2/5/solution)
  - [6](#2/6)
    - [Solution](#2/6/solution)
  - [7](#2/7)
    - [Solution](#2/7/solution)
  - [8](#2/8)
    - [Solution](#2/8/solution)
  - [9](#2/9)
    - [Solution](#2/9/solution)
  - [10](#2/10)
    - [Solution](#2/10/solution)
  - [11](#2/11)
    - [Solution](#2/11/solution)
  - [12](#2/12)
    - [Solution](#2/12/solution)
- [3](#3)
  - [1](#3/1)
    - [a](#3/1/a)
      - [Solution](#3/1/a/solution)
    - [b](#3/1/b)
      - [Solution](#3/1/b/solution)
    - [c](#3/1/c)
      - [Solution](#3/1/c/solution)
    - [d](#3/1/d)
      - [Solution](#3/1/d/solution)
  - [2](#3/2)
    - [a](#3/2/a)
      - [Solution](#3/2/a/solution)
    - [b](#3/2/b)
      - [Solution](#3/2/b/solution)
  - [3](#3/3)
    - [a](#3/3/a)
      - [Solution](#3/3/a/solution)
    - [b](#3/3/b)
      - [Solution](#3/3/b/solution)
    - [c](#3/3/c)
      - [Solution](#3/3/c/solution)
    - [d](#3/3/d)
      - [Solution](#3/3/d/solution)

## 1

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="1/1">1</h3>

↑ **Parent:** [1](#1)

<h4 id="1/1/a">a</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/a/solution">Solution</h5>

↑ **Parent:** [A](#1/1/a)

A [weak solution](../../../partial-differential-equation.md#weak-solution) is an [equivalence class](../../../set-theory.md#equivalence-class) $u\in L^\infty((0,\infty)\times\mathbb R)$ satisfying, for every [test function](../../../distribution-theory.md#test-function) $\varphi\in C_c^\infty([0,\infty)\times\mathbb R)$,

$$
\boxed{\int_0^\infty\!\int_{\mathbb R}u\bigl(\varphi_t+\partial_x(c\varphi)\bigr)\,dx\,dt+\int_{\mathbb R}u_0(x)\varphi(0,x)\,dx=0.}
$$

This is [integration by parts](../../../calculus.md#integration-by-parts) for the nonconservative [transport equation](../../../partial-differential-equation.md#transport-equation). In particular, the [weak formulation](../../../partial-differential-equation.md#weak-formulation) contains $c_x\varphi$ as well as $c\varphi_x$. The last integral encodes the [initial condition](../../../differential-equation.md#initial-condition); a pointwise boundary value of an arbitrary [Lebesgue space](../../../measure-theory.md#lp-space) representative is not the definition. Compact support of the [test function](../../../distribution-theory.md#test-function) makes the identity meaningful even if $c$ is unbounded.

<h4 id="1/1/b">b</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/b/solution">Solution</h5>

↑ **Parent:** [B](#1/1/b)

The [characteristic curves](../../../partial-differential-equation.md#characteristic-curve) solve $\dot X=X$, hence $X(t,\xi)=e^t\xi$. By the [chain rule](../../../calculus.md#chain-rule), $d[u(t,X(t,\xi))]/dt=0$. Pulling back along the [characteristic flow map](../../../partial-differential-equation.md#characteristic-flow-map) gives

$$
\boxed{u(t,x)=u_0(e^{-t}x).}
$$

For $u_0\in C^1$, this is a [classical solution](../../../partial-differential-equation.md#classical-solution): $u_t=-e^{-t}x u_0'(e^{-t}x)$ and $u_x=e^{-t}u_0'(e^{-t}x)$ cancel in the [transport equation](../../../partial-differential-equation.md#transport-equation), and at $t=0$ the [initial condition](../../../differential-equation.md#initial-condition) holds. Conversely, constancy along every [characteristic curve](../../../partial-differential-equation.md#characteristic-curve) forces this formula.

<h4 id="1/1/c">c</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/c/solution">Solution</h5>

↑ **Parent:** [C](#1/1/c)

Use the same formula for a measurable representative of $u_0$. Dilation preserves null sets and gives $\|u\|_{L^\infty}=\|u_0\|_{L^\infty}$. To check the [weak formulation](../../../partial-differential-equation.md#weak-formulation), change variables $x=e^t y$ and set $\psi(t,y)=e^t\varphi(t,e^t y)$. Then

$$
e^t(\varphi_t+x\varphi_x+\varphi)(t,e^t y)=\psi_t(t,y).
$$

The spacetime integral becomes $\int u_0(y)\psi_t(t,y)\,dy\,dt=-\int u_0(y)\varphi(0,y)\,dy$, as required.

For uniqueness, take any bounded [weak solution](../../../partial-differential-equation.md#weak-solution) and write $v(t,y)=u(t,e^t y)$. Choosing $\varphi(t,x)=e^{-t}\psi(t,e^{-t}x)$ in the [weak formulation](../../../partial-differential-equation.md#weak-formulation) gives

$$
\int v\psi_t\,dy\,dt+\int u_0(y)\psi(0,y)\,dy=0.
$$

For tensor [test functions](../../../distribution-theory.md#test-function) $\psi(t,y)=\eta(t)\theta(y)$, this says that $\int v(t,y)\theta(y)\,dy$ is distributionally constant and has value $\int u_0\theta$. A countable dense family of spatial [test functions](../../../distribution-theory.md#test-function) identifies $v=u_0$ [almost everywhere](../../../measure-theory.md#almost-everywhere). Thus **the displayed solution is the unique bounded weak solution**.

<h3 id="1/2">2</h3>

↑ **Parent:** [1](#1)

<h4 id="1/2/a">a</h4>

↑ **Parent:** [2](#1/2)

<h5 id="1/2/a/solution">Solution</h5>

↑ **Parent:** [A](#1/2/a)

A [characteristic curve](../../../partial-differential-equation.md#characteristic-curve) has $x-at$ constant. Backtracking reaches the initial line if $x\ge at$ and the inflow boundary otherwise. Hence

$$
\boxed{u(t,x)=\begin{cases}u_0(x-at),&x\ge at,\\ f(t-x/a),&0\le x<at.\end{cases}}
$$

Values on the dividing [characteristic curve](../../../partial-differential-equation.md#characteristic-curve) are immaterial for bounded [weak solutions](../../../partial-differential-equation.md#weak-solution).

For a [classical solution](../../../partial-differential-equation.md#classical-solution) on the closed quadrant, choose $u_0,f\in C^1([0,\infty))$ and impose the [corner compatibility for constant-speed transport](../../../partial-differential-equation.md#corner-compatibility-for-constant-speed-transport)

$$
\boxed{f(0)=u_0(0),\qquad f'(0)=-a u_0'(0).}
$$

These make the values and both first derivatives agree across $x=at$; each branch solves the [transport equation](../../../partial-differential-equation.md#transport-equation). They are also necessary for a $C^1$ solution up to the initial and inflow boundaries.

Spatial $C^\infty$ regularity for every $t\ge0$, up to $x=0$, holds precisely for smooth data with all matching jets:

$$
\boxed{f^{(n)}(0)=(-a)^n u_0^{(n)}(0)\quad(n=0,1,2,\ldots).}
$$

Indeed the spatial derivatives of order $n$ at $x=at$ are $u_0^{(n)}(0)$ and $(-1/a)^n f^{(n)}(0)$. Necessity of smooth $u_0$ follows at $t=0$; smoothness of $f$ on any finite interval follows by reading the boundary branch in a spatial slice at a larger time.

<h4 id="1/2/b">b</h4>

↑ **Parent:** [2](#1/2)

<h5 id="1/2/b/solution">Solution</h5>

↑ **Parent:** [B](#1/2/b)

For the [inflow transport boundary condition](../../../partial-differential-equation.md#inflow-transport-boundary-condition), the [weak formulation](../../../partial-differential-equation.md#weak-formulation) is

$$
\int_0^\infty\!\int_0^\infty u(\varphi_t+a\varphi_x)\,dx\,dt+\int_0^\infty u_0(x)\varphi(0,x)\,dx+a\int_0^\infty f(t)\varphi(t,0)\,dt=0.
$$

Here $\varphi$ is a smooth compactly supported [test function](../../../distribution-theory.md#test-function) on the closed quadrant. Put $z=x-at$ and $\psi(t,z)=\varphi(t,z+at)$. The transformed region is $t>\tau(z):=\max(0,-z/a)$. The formula in the preceding solution is $v(t,z)=b(z)$, with $b(z)=u_0(z)$ for $z\ge0$ and $b(z)=f(-z/a)$ for $z<0$. Consequently the first integral equals $-\int b(z)\psi(\tau(z),z)\,dz$. Its positive-$z$ portion cancels the initial integral; the substitution $z=-at$ in its negative-$z$ portion cancels the inflow integral, including the factor $a$. This proves weak existence for arbitrary bounded data without corner compatibility.

For uniqueness, subtract two [weak solutions](../../../partial-differential-equation.md#weak-solution). Interior [test functions](../../../distribution-theory.md#test-function) in these [characteristic coordinates](../../../partial-differential-equation.md#characteristic-coordinate) give $\partial_t v=0$ distributionally, so $v(t,z)=b(z)$ on each vertical ray. This follows first on rectangles compactly contained in $t>\tau(z)$ using tensor [test functions](../../../distribution-theory.md#test-function), and then on the whole region by overlapping rectangles. In the full [weak formulation](../../../partial-differential-equation.md#weak-formulation) the remaining lower-boundary term is $-\int b(z)\psi(\tau(z),z)\,dz=0$. Arbitrary smooth traces supported separately on $z>0$ and $z<0$ force $b=0$ there. The single point $z=0$ has zero measure. Thus **the two-branch formula is the unique bounded weak solution**.

<h3 id="1/3">3</h3>

↑ **Parent:** [1](#1)

<h4 id="1/3/a">a</h4>

↑ **Parent:** [3](#1/3)

<h5 id="1/3/a/solution">Solution</h5>

↑ **Parent:** [A](#1/3/a)

For the [scalar conservation law](../../../partial-differential-equation.md#scalar-conservation-law), put $v_0(\xi)=f'(u_0(\xi))$ and $m=\min_\xi v_0'(\xi)=\min_\xi f''(u_0(\xi))u_0'(\xi)$. The [concave-flux characteristic lifespan](../../../partial-differential-equation.md#concave-flux-characteristic-lifespan) and [characteristic flow map](../../../partial-differential-equation.md#characteristic-flow-map) are

$$
\boxed{t^*=\begin{cases}-1/m,&m<0,\\ \infty,&m\ge0,\end{cases}\qquad X_t(\xi)=\xi+t f'(u_0(\xi)),\qquad u(t,X_t(\xi))=u_0(\xi).}
$$

For $t<t^*$, $X_t'=1+t v_0'>0$, and $X_t(\xi)=\xi+ct$ outside the support of $u_0$. Thus $X_t$ is a global smooth [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) and the formula is $u(t,x)=u_0(X_t^{-1}(x))$. The [method of characteristics](../../../partial-differential-equation.md#method-of-characteristics) proves existence and uniqueness among smooth solutions.

If $m<0$, at a minimizer $\xi_*$ the numerator $u_0'(\xi_*)$ is nonzero, since its product with $f''(u_0(\xi_*))$ is negative. Therefore

$$
u_x(t,X_t(\xi_*))=\frac{u_0'(\xi_*)}{1+t v_0'(\xi_*)}
$$

blows up as $t\uparrow t^*$, showing that this is the maximal smooth lifespan. Strict [concavity](../../../real-analysis.md#concave-function) alone does not require $f''$ to be negative at every point; the argument uses no such extra hypothesis.

<h4 id="1/3/b">b</h4>

↑ **Parent:** [3](#1/3)

<h5 id="1/3/b/solution">Solution</h5>

↑ **Parent:** [B](#1/3/b)

The [inverse function theorem](../../../calculus.md#inverse-function-theorem) applied to $X_t$ makes $u_0\circ X_t^{-1}$ smooth. Since $u_0(\pm A)=0$, $X_t(\pm A)=\pm A+ct$. Monotonicity of the [characteristic flow map](../../../partial-differential-equation.md#characteristic-flow-map) and the vanishing of $u_0$ outside $[-A,A]$ imply

$$
\boxed{\operatorname{supp}u(t,\cdot)\subset[-A+ct,A+ct]\quad(0<t<t^*).}
$$

Thus the solution is a [smooth function](../../../analysis.md#smooth-function) with compact support at each such time. The fact that some interior [characteristic speeds](../../../partial-differential-equation.md#characteristic-speed) differ from $c$ causes no difficulty: they cannot cross the two exterior [characteristic curves](../../../partial-differential-equation.md#characteristic-curve) before $t^*$.

<h4 id="1/3/c">c</h4>

↑ **Parent:** [3](#1/3)

<h5 id="1/3/c/solution">Solution</h5>

↑ **Parent:** [C](#1/3/c)

The compact support just established and $f(0)=0$ permit differentiation of the [antiderivative](../../../calculus.md#antiderivative) and integration of the [scalar conservation law](../../../partial-differential-equation.md#scalar-conservation-law) from $-\infty$:

$$
U_x=u,\qquad U_t=-f(u),\qquad \boxed{U_t+f(U_x)=0,\quad U(0,x)=\int_{-\infty}^x u_0(y)\,dy.}
$$

This is a [Hamilton-Jacobi equation](../../../classical-mechanics.md#hamilton-jacobi-equation). There is no arbitrary function of time: the normalization at $-\infty$ and the zero exterior flux determine it.

<h4 id="1/3/d">d</h4>

↑ **Parent:** [3](#1/3)

<h5 id="1/3/d/solution">Solution</h5>

↑ **Parent:** [D](#1/3/d)

The tangent-line inequality for a differentiable [concave function](../../../real-analysis.md#concave-function) is $f(r)\le f(s)+f'(s)(r-s)$. Taking $r=u=U_x$ and using the [Hamilton-Jacobi equation](../../../classical-mechanics.md#hamilton-jacobi-equation) yields

$$
U_t+f'(s)U_x=f'(s)u-f(u)\ge sf'(s)-f(s).
$$

Along $x(\tau)=x_0+\tau f'(s)$, the [chain rule](../../../calculus.md#chain-rule) identifies the left side with $dU(\tau,x(\tau))/d\tau$. Integrating gives

$$
\boxed{U(t,x_0+t f'(s))-U(0,x_0)\ge t\bigl(sf'(s)-f(s)\bigr).}
$$

Strict [concavity](../../../real-analysis.md#concave-function) makes equality possible exactly when $u=s$ along the line, which will select the maximizing [characteristic curve](../../../partial-differential-equation.md#characteristic-curve).

<h4 id="1/3/e">e</h4>

↑ **Parent:** [3](#1/3)

<h5 id="1/3/e/solution">Solution</h5>

↑ **Parent:** [E](#1/3/e)

Because $f'$ is a decreasing bijection, its inverse $h$ exists and is continuous. For any $y$, choose $s=h((x-y)/t)$ in the preceding inequality. The line from $(0,y)$ then reaches $(t,x)$, giving $U(t,x)\ge U(0,y)+t g((x-y)/t)$.

Now let $x_0=X_t^{-1}(x)$ and $s=u_0(x_0)$. On this [characteristic curve](../../../partial-differential-equation.md#characteristic-curve), $u=s$, so the tangent-line inequality is an equality throughout. This proves attainment and

$$
\boxed{U(t,x)=\max_{y\in\mathbb R}\left\{U(0,y)+t g\left(\frac{x-y}{t}\right)\right\},\qquad u(t,x)=h\left(\frac{x-x_0}{t}\right).}
$$

In fact the maximizing foot is unique. The [concave Legendre dual](../../../convex-optimization.md#concave-legendre-dual) can be written $g(z)=\inf_s(zs-f(s))$ and satisfies $g'(z)=h(z)$: compare the minimizing values at $z$ and $z+\varepsilon$ and use continuity of $h$. This avoids assuming differentiability of $h$, which strict [concavity](../../../real-analysis.md#concave-function) by itself does not guarantee. Differentiating the maximizing expression with respect to $y$ gives $u_0(y)-h((x-y)/t)=0$, hence $X_t(y)=x$ and $y=x_0$. The [maximum representation for a concave conservation law](../../../partial-differential-equation.md#maximum-representation-for-a-concave-conservation-law) therefore reproduces the [characteristic solution of a scalar conservation law](../../../partial-differential-equation.md#characteristic-solution-of-a-scalar-conservation-law) throughout the smooth lifespan.

<h4 id="1/3/f">f</h4>

↑ **Parent:** [3](#1/3)

<h5 id="1/3/f/solution">Solution</h5>

↑ **Parent:** [F](#1/3/f)

**The printed linear ordering is false for $z<c$.** For example, $f(s)=-s^2/2$, $c=0$, $h(z)=-z$, $k_-=-3/4$, $k_+=-1/4$ satisfy the derivative hypothesis, but at $z=-1$ the printed lower bound would require $3/4\le1/2$.

The correct [inverse-flux quadratic bounds](../../../convex-optimization.md#inverse-flux-quadratic-bounds) are

$$
\boxed{\begin{aligned}
k_-(z-c)&\le h(z)/2\le k_+(z-c)&& (z\ge c),\\
k_+(z-c)&\le h(z)/2\le k_-(z-c)&& (z\le c),\\
k_-(z-c)^2&\le g(z)\le k_+(z-c)^2&& (z\in\mathbb R).
\end{aligned}}
$$

Indeed $h(c)=0$ and $h(z)/2=\int_c^z h'(r)/2\,dr$; reversing the integration limits reverses the linear inequalities. Equivalently, for $z\ne c$, $k_-\le h(z)/(2(z-c))\le k_+$. Since $g(c)=0$ and $g'=h$, integration once more gives the quadratic inequalities on both sides of $c$. A useful sign-independent consequence is $|h(z)|\le-2k_-|z-c|$.

<h4 id="1/3/g">g</h4>

↑ **Parent:** [3](#1/3)

<h5 id="1/3/g/solution">Solution</h5>

↑ **Parent:** [G](#1/3/g)

Write $M=\|u_0\|_{L^1}$. Since $|U(0,y)|\le M$, choosing $y=x-ct$ gives $g((x-y)/t)=g(c)=0$ and $\max_yG_{t,x}(y)\ge-M$. At the maximizing foot $x_0$, the [inverse-flux quadratic bounds](../../../convex-optimization.md#inverse-flux-quadratic-bounds) give

$$
\max_yG_{t,x}(y)=U(0,x_0)+t g\left(\frac{x-x_0}{t}\right)\le M+\frac{k_+}{t}(x-x_0-ct)^2.
$$

Combining the two estimates and dividing by $-k_+>0$ gives

$$
\boxed{\left|\frac{x-x_0}{t}-c\right|\le\sqrt{\frac{2M}{-k_+t}},\qquad |u(t,x)|\le\frac{-2k_-}{\sqrt t}\sqrt{\frac{2M}{-k_+}}.}
$$

The last step uses $u=h((x-x_0)/t)$ and the sign-independent bound on $h$. This is [square-root decay before characteristic crossing](../../../partial-differential-equation.md#square-root-decay-before-characteristic-crossing); it is proved only for $0<t<t^*$. No continuation past [characteristic crossing](../../../partial-differential-equation.md#characteristic-crossing) or global-time smoothness is assumed. If $M=0$, the initial function and the solution vanish.

<h2 id="2">2</h2>

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="2/1">1</h3>

↑ **Parent:** [2](#2)

<h4 id="2/1/solution">Solution</h4>

↑ **Parent:** [1](#2/1)

Throughout this question the [Banach spaces](../../../banach-space.md) and [Hilbert spaces](../../../hilbert-space.md) are complex. Separability is an additional standing hypothesis, not part of the general definition of a [Hilbert space](../../../hilbert-space.md). Here and below [unit ball](../../../functional-analysis.md#unit-ball) means the closed unit ball. An open unit ball in positive finite dimension is not compact. In finite dimension, equivalence of [norms](../../../functional-analysis.md#norm) identifies the closed unit ball with a closed bounded subset of Euclidean space, so the [Heine-Borel theorem](../../../topology.md#heine-borel-theorem) gives compactness in the [norm topology](../../../functional-analysis.md#norm-topology).

In an infinite-dimensional [Hilbert space](../../../hilbert-space.md), the [Gram-Schmidt process](../../../linear-algebra.md#gram-schmidt-process) constructs an infinite [orthonormal sequence](../../../hilbert-space.md#orthonormal-sequence) $(e_n)$. Put $f_n=e_n/\sqrt2$. Then $\|f_n\|=1/\sqrt2\le1$ and, for $m\ne n$, $\|f_n-f_m\|^2=(1+1)/2=1$. No subsequence is a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence), contradicting [sequential compactness](../../../geometry-and-topology.md#sequentially-compact-space). Thus **the closed unit ball is norm compact exactly in finite dimension**.

<h3 id="2/2">2</h3>

↑ **Parent:** [2](#2)

<h4 id="2/2/solution">Solution</h4>

↑ **Parent:** [2](#2/2)

The finite-dimensional implication again follows from equivalence of [norms](../../../functional-analysis.md#norm) and the [Heine-Borel theorem](../../../topology.md#heine-borel-theorem). In an infinite-dimensional [Banach space](../../../banach-space.md), inductively apply [Riesz lemma](../../../banach-space.md#riesz-s-lemma) to the proper closed finite-dimensional [linear span](../../../vector-space.md#linear-span) $Y_n=\operatorname{span}(f_1,\ldots,f_n)$ to obtain a unit vector $f_{n+1}$ with $\operatorname{dist}(f_{n+1},Y_n)>1/2$. Therefore $\|f_n-f_m\|>1/2$ for distinct indices, precluding a [Cauchy subsequence](../../../real-analysis.md#cauchy-subsequence).

For completeness, [Riesz lemma](../../../banach-space.md#riesz-s-lemma) here follows by taking $z\notin Y$, setting $d=\operatorname{dist}(z,Y)>0$, choosing $y\in Y$ with $\|z-y\|<2d$, and putting $f=(z-y)/\|z-y\|$. Its distance from $Y$ exceeds $1/2$. This proves **the closed unit ball is norm compact if and only if the Banach space is finite-dimensional**. The printed hint's equality of all pairwise distances is unnecessary; the separation inequality is what the argument supplies.

<h3 id="2/3">3</h3>

↑ **Parent:** [2](#2)

<h4 id="2/3/solution">Solution</h4>

↑ **Parent:** [3](#2/3)

Use the assumed separability of the [Hilbert space](../../../hilbert-space.md) to choose a countable [Hilbertian basis](../../../hilbert-space.md#hilbertian-basis) $(e_j)$. For $\|f_n\|\le M$, every scalar sequence $\langle f_n,e_j\rangle$ is bounded. Repeated extraction followed by the [diagonal subsequence argument](../../../real-analysis.md#diagonal-subsequence-argument) gives one subsequence with all these coordinates converging, say to $a_j$. The [Bessel inequality](../../../hilbert-space.md#bessel-s-inequality) gives $\sum_{j\le N}|a_j|^2\le M^2$ for every $N$, so $g=\sum_ja_je_j$ exists and $\|g\|\le M$.

For $h\in H$, let $h_N$ be its finite basis truncation. Coordinate convergence gives $\langle f_{\varphi(n)}-g,h_N\rangle\to0$, while the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) bounds the remaining inner product by $2M\|h-h_N\|$, uniformly in $n$. First choose $N$ large, then $n$ large. Thus

$$
\boxed{f_{\varphi(n)}\rightharpoonup g.}
$$

This proves the asserted sequential conclusion. To obtain actual compactness for the [weak topology](../../../weak-topology.md), note that on a bounded ball it is induced by the metric

$$
d(v,w)=\sum_{j=1}^\infty2^{-j}\frac{|\langle v-w,e_j\rangle|}{1+|\langle v-w,e_j\rangle|}.
$$

Finite coordinates and the uniformly small tail show that $d$ gives coordinate convergence; uniform boundedness of the ball extends this to every inner product as above. Hence this metric induces exactly the restricted [weak topology](../../../weak-topology.md). In a [metric space](../../../topological-analysis.md#metric-space), sequential compactness implies compactness. The closed unit ball is therefore **weakly compact**, and the limit remains inside it.

<h3 id="2/4">4</h3>

↑ **Parent:** [2](#2)

<h4 id="2/4/solution">Solution</h4>

↑ **Parent:** [4](#2/4)

**No.** On the complex [l2 sequence space](../../../banach-space.md#l2-sequence-space), let $L(x_n)=(x_n/n)$. This is a bounded [self-adjoint operator](../../../linear-operator-theory.md#self-adjoint-operator). At $\lambda=0$, $\ker L=\{0\}$, so zero is not an [eigenvalue](../../../linear-operator-theory.md#eigenvalue) (an eigenvector must be nonzero). But $y=(1/n)\in\ell^2$ has no preimage in $\ell^2$: its only formal preimage is the constant-one sequence. Thus $L$ is not surjective and

$$
\boxed{0\in\Sigma(L)\quad\hbox{but}\quad0\notin\sigma_{\mathrm p}(L).}
$$

Alternatively $\|Le_n\|=1/n\to0$ excludes a bounded inverse. This example separates the [spectrum of a bounded operator](../../../linear-operator-theory.md#spectrum-of-a-bounded-operator) from its [point spectrum](../../../linear-operator-theory.md#point-spectrum).

<h3 id="2/5">5</h3>

↑ **Parent:** [2](#2)

<h4 id="2/5/solution">Solution</h4>

↑ **Parent:** [5](#2/5)

The intended [self-adjoint operator](../../../linear-operator-theory.md#self-adjoint-operator) identity is $\langle Lf,g\rangle=\langle f,Lg\rangle$, with the [inner product](../../../linear-algebra.md#inner-product) linear in its first argument. The printed second $Lf$ must be $Lg$. Taken literally, the printed identity forces $L=0$: put $g=0$ and then vary $g$. Its spectral conclusion is then trivial, but it does not define self-adjointness.

For the corrected identity, $\langle Lv,v\rangle$ is real. If $\operatorname{Im}\lambda\ne0$, the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives

$$
\|(L-\lambda I)v\|\|v\|\ge|\operatorname{Im}\langle(L-\lambda I)v,v\rangle|=|\operatorname{Im}\lambda|\|v\|^2.
$$

Thus $L-\lambda I$ is injective and bounded below, so its range is closed: a convergent image sequence has a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) of preimages. Its range is dense because its [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) is $\ker(L-\bar\lambda I)$, also zero by the same lower bound. Hence it is surjective with inverse norm at most $1/|\operatorname{Im}\lambda|$. Therefore

$$
\boxed{\Sigma(L)\subset\mathbb R.}
$$

<h3 id="2/6">6</h3>

↑ **Parent:** [2](#2)

<h4 id="2/6/solution">Solution</h4>

↑ **Parent:** [6](#2/6)

For a bounded [self-adjoint operator](../../../linear-operator-theory.md#self-adjoint-operator), $g$ is orthogonal to its range exactly when $\langle Lf,g\rangle=\langle f,Lg\rangle=0$ for every $f$, or equivalently $Lg=0$. Consequently

$$
\boxed{\overline{\operatorname{ran}L}=(\ker L)^{\perp}=H\quad\hbox{if }\ker L=\{0\}.}
$$

This is [image-kernel orthogonality for an adjoint](../../../hilbert-space.md#image-kernel-orthogonality-for-an-adjoint). Taking the double [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) gives the closure; it does not assert that the range itself is closed.

<h3 id="2/7">7</h3>

↑ **Parent:** [2](#2)

<h4 id="2/7/solution">Solution</h4>

↑ **Parent:** [7](#2/7)

If unit vectors $f_n$ satisfy $(L-\lambda I)f_n\to0$, a bounded inverse would give $1\le\|(L-\lambda I)^{-1}\|\|(L-\lambda I)f_n\|\to0$. Hence $\lambda$ belongs to the [spectrum of a bounded operator](../../../linear-operator-theory.md#spectrum-of-a-bounded-operator).

Conversely a spectral point is real by the preceding argument. Put $A=L-\lambda I$, again a [self-adjoint operator](../../../linear-operator-theory.md#self-adjoint-operator). If $\inf_{\|f\|=1}\|Af\|>0$, then $A$ is injective with closed range. Its range is dense by [image-kernel orthogonality for an adjoint](../../../hilbert-space.md#image-kernel-orthogonality-for-an-adjoint), so it is bijective with a bounded inverse, a contradiction. Thus this infimum is zero; choose unit $f_n$ with $\|Af_n\|<1/n$. We have proved

$$
\boxed{\lambda\in\Sigma(L)\iff\exists(f_n):\ \|f_n\|=1,\quad(L-\lambda I)f_n\to0.}
$$

Such a sequence is a [spectral Weyl sequence](../../../linear-operator-theory.md#spectral-weyl-sequence). No weak convergence is required here; nonreal $\lambda$ are ruled out by the lower bound in the preceding solution.

<h3 id="2/8">8</h3>

↑ **Parent:** [2](#2)

<h4 id="2/8/solution">Solution</h4>

↑ **Parent:** [8](#2/8)

**No.** Reuse the [diagonal operator on sequence space](../../../functional-analysis.md#diagonal-operator-on-sequence-space) $L(x_n)=(x_n/n)$ on $\ell^2$. Its kernel is zero, hence finite-dimensional. Let $y^{(N)}$ be the truncation of $(1/n)$ to its first $N$ coordinates. Each $y^{(N)}=L(1,\ldots,1,0,\ldots)$ lies in the range, while $y^{(N)}\to(1/n)$ in $\ell^2$. The limit is not in the range because its formal preimage is not square summable. Thus **finite-dimensional kernel does not imply closed range**. Equivalently the unit vectors $e_n\in(\ker L)^\perp$ violate every positive [closed-range bound on the kernel complement](../../../functional-analysis.md#closed-range-bound-on-the-kernel-complement).

<h3 id="2/9">9</h3>

↑ **Parent:** [2](#2)

<h4 id="2/9/solution">Solution</h4>

↑ **Parent:** [9](#2/9)

For the subsequent [essential spectrum](../../../functional-analysis.md#essential-spectrum-of-a-closed-operator) arguments, the discrete-spectrum definition must use $\operatorname{ran}(L-\lambda I)$ closed, rather than the printed unshifted range. With that correction, $0\notin\Sigma_{\mathrm e}(L)$ means exactly that $N=\ker L$ is finite-dimensional and $\operatorname{ran}L$ is closed; this includes the case $0$ is in the [resolvent set](../../../functional-analysis.md#resolvent-set-of-an-operator).

A [closed-range bound on the kernel complement](../../../functional-analysis.md#closed-range-bound-on-the-kernel-complement) supplies the useful equivalence

$$
\operatorname{ran}L\text{ closed}\iff\exists b>0:\ \|Lv\|\ge b\|v\|\quad(v\in N^\perp).
$$

For the forward implication, $L:N^\perp\to\operatorname{ran}L$ is a bounded bijection between [Banach spaces](../../../banach-space.md), so the [bounded inverse theorem](../../../functional-analysis.md#bounded-inverse-theorem) applies. For the reverse implication, any [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) of image points has a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) of preimages in $N^\perp$, and completeness gives a preimage of its limit.

Now decompose a bounded sequence as $f_n=p_n+v_n$ with $p_n\in N$, $v_n\in N^\perp$. If $Lf_n$ converges, the lower bound makes $(v_n)$ a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence). The [finite-dimensional vector space](../../../vector-space.md#finite-dimensional-vector-space) $N$ makes the bounded $p_n$ have a convergent subsequence. Their sum has a norm-convergent subsequence.

Conversely, if every bounded sequence with convergent images has a norm-convergent subsequence, the kernel cannot be infinite-dimensional: an [orthonormal sequence](../../../hilbert-space.md#orthonormal-sequence) in it would have zero images and no convergent subsequence. If the range were not closed, the lower-bound equivalence would provide unit vectors $v_n\in N^\perp$ with $Lv_n\to0$. Any norm limit would lie in both $N$ and $N^\perp$, hence be zero, contradicting its unit norm. This proves **the required [sequential properness for a self-adjoint operator](../../../functional-analysis.md#sequential-properness-for-a-self-adjoint-operator) equivalence**.

The spectral-shift repair is essential for later parts. On $\ell^2$, take $L=\operatorname{diag}(2,1,1/2,1/3,\ldots)$. Its range is not closed, but $2$ is an isolated eigenvalue with one-dimensional eigenspace and closed shifted range. The printed definition would incorrectly place $2$ in the [essential spectrum](../../../functional-analysis.md#essential-spectrum-of-a-closed-operator), although no [singular Weyl sequence](../../../linear-operator-theory.md#singular-weyl-sequence) exists there: on the complement of that eigenspace, $\|(L-2I)v\|\ge\|v\|$.

<h3 id="2/10">10</h3>

↑ **Parent:** [2](#2)

<h4 id="2/10/solution">Solution</h4>

↑ **Parent:** [10](#2/10)

Use the corrected [essential spectrum of a bounded self-adjoint operator](../../../functional-analysis.md#essential-spectrum-of-a-bounded-self-adjoint-operator) and put $A=L-\lambda I$. Essential spectral points are real. If $\ker A$ is infinite-dimensional, choose an [orthonormal sequence](../../../hilbert-space.md#orthonormal-sequence) in the kernel. It converges weakly to zero by the [Bessel inequality](../../../hilbert-space.md#bessel-s-inequality), and its residuals vanish.

If $\ker A$ is finite-dimensional, membership in the [essential spectrum](../../../functional-analysis.md#essential-spectrum-of-a-closed-operator) means the range is not closed. Choose unit $v_n\in(\ker A)^\perp$ with $Av_n\to0$, using the [closed-range bound on the kernel complement](../../../functional-analysis.md#closed-range-bound-on-the-kernel-complement). A bounded [Hilbert space](../../../hilbert-space.md) sequence has a weakly convergent subsequence. Its weak limit $v$ satisfies $Av=0$ because bounded operators preserve [weak convergence](../../../weak-topology.md#weak-convergence), and $v\in(\ker A)^\perp$; hence $v=0$. This subsequence is a [singular Weyl sequence](../../../linear-operator-theory.md#singular-weyl-sequence).

Conversely a [singular Weyl sequence](../../../linear-operator-theory.md#singular-weyl-sequence) first places $\lambda$ in the [spectrum of a bounded operator](../../../linear-operator-theory.md#spectrum-of-a-bounded-operator). If it were not essential, the [sequential properness for a self-adjoint operator](../../../functional-analysis.md#sequential-properness-for-a-self-adjoint-operator) equivalence for $A$ would yield a norm-convergent subsequence. Its weak limit is zero, whereas norm convergence of unit vectors gives a unit norm limit, a contradiction. Therefore

$$
\boxed{\lambda\in\Sigma_{\mathrm e}(L)\iff\exists(f_n):\ \|f_n\|=1,\ f_n\rightharpoonup0,\ (L-\lambda I)f_n\to0.}
$$

For nonreal $\lambda$, the resolvent lower bound excludes such a sequence, so the equivalence covers all $\lambda\in\mathbb C$.

<h3 id="2/11">11</h3>

↑ **Parent:** [2](#2)

<h4 id="2/11/solution">Solution</h4>

↑ **Parent:** [11](#2/11)

Suppose $K$ is a [compact operator](../../../compact-operator.md) and $f_n\rightharpoonup f$. The [Uniform boundedness principle](../../../banach-space.md#uniform-boundedness-principle) makes $(f_n)$ bounded. If $Kf_n$ did not converge in norm to $Kf$, some subsequence would stay a fixed positive distance away. Compactness provides a further norm-convergent subsequence, say to $g$. On the other hand, for every $h$, $\langle Kf_n,h\rangle=\langle f_n,K^*h\rangle\to\langle Kf,h\rangle$, so its norm limit must be $Kf$, a contradiction.

Conversely, if $K$ sends every weakly convergent sequence to a norm-convergent sequence, take any sequence in the closed [unit ball](../../../functional-analysis.md#unit-ball). Weak compactness of that ball supplies a weakly convergent subsequence, whose images converge in norm by hypothesis. Thus every sequence in the image has a convergent subsequence in $H$. Its closure is also sequentially compact: approximate its $n$th member by an image point within $1/n$. Since $H$ is a [metric space](../../../topological-analysis.md#metric-space), that closure is compact. We conclude

$$
\boxed{K\text{ compact}\iff f_n\rightharpoonup f\Longrightarrow\|Kf_n-Kf\|\to0.}
$$

This is the principle that [compact operators send weak convergence to norm convergence](../../../compact-operator.md#compact-operators-send-weak-convergence-to-norm-convergence).

<h3 id="2/12">12</h3>

↑ **Parent:** [2](#2)

<h4 id="2/12/solution">Solution</h4>

↑ **Parent:** [12](#2/12)

Let $(f_n)$ be a [singular Weyl sequence](../../../linear-operator-theory.md#singular-weyl-sequence) for $L$ at $\lambda\in\Sigma_{\mathrm e}(L)$. Since $K$ is compact and $f_n\rightharpoonup0$, the preceding result gives $Kf_n\to0$. Therefore

$$
(L+K-\lambda I)f_n=(L-\lambda I)f_n+Kf_n\to0.
$$

The norms remain one and the weak limit remains zero. The [singular Weyl sequence](../../../linear-operator-theory.md#singular-weyl-sequence) criterion yields $\lambda\in\Sigma_{\mathrm e}(L+K)$. Apply the same argument to $L+K$ and the compact [self-adjoint operator](../../../linear-operator-theory.md#self-adjoint-operator) $-K$ for the reverse inclusion. Both operators are bounded and self-adjoint. Thus the [Weyl theorem for compact self-adjoint perturbations](../../../functional-analysis.md#weyl-theorem-for-compact-self-adjoint-perturbations) is

$$
\boxed{\Sigma_{\mathrm e}(L+K)=\Sigma_{\mathrm e}(L).}
$$

The corrected shifted-range definition is necessary. For the diagonal example in the preceding solutions, a rank-one perturbation changing the entry $2$ to $0$ removes $2$ from the spectrum. The unshifted printed definition had classified $2$ as essential merely because the original range was not closed, so it would make this invariance false.

<h2 id="3">3</h2>

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="3/1">1</h3>

↑ **Parent:** [3](#3)

<h4 id="3/1/a">a</h4>

↑ **Parent:** [1](#3/1)

<h5 id="3/1/a/solution">Solution</h5>

↑ **Parent:** [A](#3/1/a)

For $I=(-a,a)$, the [first-order Sobolev space](../../../sobolev-space.md#first-order-sobolev-space) is

$$
\boxed{H^1(I)=\{u\in L^2(I):\exists v\in L^2(I),\ \int_Iu\varphi'=-\int_Iv\varphi\text{ for every }\varphi\in C_c^\infty(I)\}.}
$$

The [weak derivative](../../../distribution-theory.md#weak-derivative) $v=u'$ is unique as an [equivalence class](../../../set-theory.md#equivalence-class) modulo equality [almost everywhere](../../../measure-theory.md#almost-everywhere). We use the standard [Sobolev norm](../../../sobolev-space.md#sobolev-norm) $\|u\|_{H^1(I)}^2=\|u\|_{L^2(I)}^2+\|u'\|_{L^2(I)}^2$. Pointwise values of an arbitrary representative have no intrinsic meaning; the [one-dimensional Sobolev representative](../../../sobolev-space.md#one-dimensional-sobolev-representative) supplies the continuous representative used later.

<h4 id="3/1/b">b</h4>

↑ **Parent:** [1](#3/1)

<h5 id="3/1/b/solution">Solution</h5>

↑ **Parent:** [B](#3/1/b)

Reflect $u$ across the two endpoints of $I$ into a slightly larger interval, giving an $H^1$ extension, and multiply by a smooth [cutoff function](../../../distribution-theory.md#cutoff-function) equal to one near $\overline I$. Convolve the resulting function on $\mathbb R$ with a [mollifier](../../../distribution-theory.md#mollifier). The convolutions $u_\varepsilon$ are smooth; differentiation commutes with convolution of the [weak derivative](../../../distribution-theory.md#weak-derivative). Continuity of translations in $L^2$ proves both $u_\varepsilon\to u$ and $u_\varepsilon'\to u'$ in $L^2(I)$, hence convergence in the [Sobolev norm](../../../sobolev-space.md#sobolev-norm).

To obtain convergence [almost everywhere](../../../measure-theory.md#almost-everywhere), select a sequence with $\|u_n-u\|_2\le2^{-n}$. Then $\int\sum_n|u_n-u|^2<\infty$, so the summands tend to zero almost everywhere. Thus **a smooth approximating sequence converges both in $H^1$ and almost everywhere**. This is [density of smooth functions in a Sobolev space](../../../sobolev-space.md#density-of-smooth-functions-in-a-sobolev-space); smooth functions need not vanish at the endpoints.

<h4 id="3/1/c">c</h4>

↑ **Parent:** [1](#3/1)

<h5 id="3/1/c/solution">Solution</h5>

↑ **Parent:** [C](#3/1/c)

For a smooth approximation, the [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) and [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) give

$$
|u_n(x)-u_n(y)|\le\int_{[x,y]}|u_n'|\le|x-y|^{1/2}\|u_n'\|_{L^2(I)}.
$$

Let $E\subset I$ be one full-measure set on which $u_n\to u$. Passing to the limit for all $x,y\in E$ gives

$$
\boxed{\mathop{\mathrm{ess\,sup}}_{x\ne y}\frac{|u(x)-u(y)|}{|x-y|^{1/2}}\le\|u'\|_2\le\|u\|_{H^1(I)}.}
$$

The full-measure set $E$ is dense, and the estimate extends its representative uniquely to a $1/2$-[Hölder continuous function](../../../sobolev-space.md#holder-condition) on $\overline I$. Its classical [Hölder seminorm](../../../sobolev-space.md#holder-seminorm) satisfies the same bound. Changing the original representative on a null set does not affect the [essential supremum](../../../measure-theory.md#essential-supremum) in the assertion.

<h4 id="3/1/d">d</h4>

↑ **Parent:** [1](#3/1)

<h5 id="3/1/d/solution">Solution</h5>

↑ **Parent:** [D](#3/1/d)

**With the standard Sobolev norm, the printed constant one is not valid for arbitrary $a$.** The constant function $u=1$ has supremum norm one and $H^1$ norm $\sqrt{2a}$, which is smaller when $a<1/2$.

For the continuous [one-dimensional Sobolev representative](../../../sobolev-space.md#one-dimensional-sobolev-representative), let $\bar u=(2a)^{-1}\int_Iu$. The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives $|\bar u|\le(2a)^{-1/2}\|u\|_2$. Using the preceding [Hölder seminorm](../../../sobolev-space.md#holder-seminorm) estimate,

$$
|u(x)-\bar u|\le\frac1{2a}\int_I|u(x)-u(y)|\,dy\le\sqrt{2a}\|u'\|_2.
$$

Consequently the corrected [interval Sobolev supremum estimate](../../../sobolev-space.md#interval-sobolev-supremum-estimate) is

$$
\boxed{\|u\|_\infty\le(2a)^{-1/2}\|u\|_2+\sqrt{2a}\|u'\|_2\le\sqrt{(2a)^{-1}+2a}\,\|u\|_{H^1(I)}.}
$$

One may first prove this for smooth approximations and pass on the full-measure convergence set. Averaging differences also handles complex-valued functions without assuming that a function takes its complex average at some point. At the fixed interval used below the constant is absolute, which suffices for the intended interior estimate.

<h3 id="3/2">2</h3>

↑ **Parent:** [3](#3)

<h4 id="3/2/a">a</h4>

↑ **Parent:** [2](#3/2)

<h5 id="3/2/a/solution">Solution</h5>

↑ **Parent:** [A](#3/2/a)

Write $R=\Lambda/\lambda$. The coefficient is measurable, so interpret the [divergence-form elliptic operator](../../../elliptic-boundary-value-problem.md#divergence-form-elliptic-operator) weakly: $\int A u'\phi'=0$ for compactly supported $H^1$ tests. Testing with $\phi=\zeta^2u$ gives

$$
\lambda\int\zeta^2|u'|^2\le2\Lambda\int\zeta|u'||u||\zeta'|\le2\Lambda\left(\int\zeta^2|u'|^2\right)^{1/2}\left(\int u^2|\zeta'|^2\right)^{1/2}.
$$

Divide if the first integral is positive; the zero case is immediate. Since $\zeta=1$ on the inner interval,

$$
\boxed{\int_{-1/2}^{1/2}|u'|^2\le4R^2\int_{-1}^1u^2|\zeta'|^2.}
$$

This [Caccioppoli inequality](../../../partial-differential-equation.md#caccioppoli-inequality) applies in particular to the smooth solutions in the question. No derivative of $A$ is taken.

<h4 id="3/2/b">b</h4>

↑ **Parent:** [2](#3/2)

<h5 id="3/2/b/solution">Solution</h5>

↑ **Parent:** [B](#3/2/b)

Choose a fixed smooth [cutoff function](../../../distribution-theory.md#cutoff-function) with $\|\zeta'\|_\infty=C_0$ and set $J=(-1/2,1/2)$. The [Caccioppoli inequality](../../../partial-differential-equation.md#caccioppoli-inequality) gives $\|u'\|_{L^2(J)}\le2RC_0\|u\|_{L^2(-1,1)}$. Since the length of $J$ is one, the corrected [interval Sobolev supremum estimate](../../../sobolev-space.md#interval-sobolev-supremum-estimate) yields $\|u\|_{L^\infty(J)}\le\|u\|_{L^2(J)}+\|u'\|_{L^2(J)}$, and the [Hölder seminorm](../../../sobolev-space.md#holder-seminorm) is at most $\|u'\|_{L^2(J)}$. Therefore

$$
\boxed{\|u\|_{L^\infty(J)}+[u]_{C^{0,1/2}(J)}\le(1+4RC_0)\|u\|_{L^2(-1,1)}.}
$$

For locally $H^1$ [weak solutions](../../../partial-differential-equation.md#weak-solution) with $u\in L^2(-1,1)$, [density of smooth functions in a Sobolev space](../../../sobolev-space.md#density-of-smooth-functions-in-a-sobolev-space) justifies the test $\zeta^2u$, and the previous representative estimates already apply to $H^1$. Mollifying a solution need not preserve the equation with the same measurable coefficient, so approximation is used for admissible tests and Sobolev estimates, not to assert that the mollified function solves the original equation. The required constant depends only on $R$.

<h3 id="3/3">3</h3>

↑ **Parent:** [3](#3)

<h4 id="3/3/a">a</h4>

↑ **Parent:** [3](#3/3)

<h5 id="3/3/a/solution">Solution</h5>

↑ **Parent:** [A](#3/3/a)

For a real [weak solution](../../../partial-differential-equation.md#weak-solution) $u\in H^1_{\mathrm{loc}}(B_1)$, $\int A\nabla u\cdot\nabla\phi=0$ for compactly supported $H^1$ tests. The symmetric coefficient bounds give $A\xi\cdot\xi\ge\lambda|\xi|^2$ and $|A\xi|\le\Lambda|\xi|$. Test with $\phi=\zeta^2u$ and apply the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality):

$$
\lambda E\le2\Lambda E^{1/2}I^{1/2},\qquad E=\int\zeta^2|\nabla u|^2,\quad I=\int u^2|\nabla\zeta|^2.
$$

Thus $E\le4R^2 I$, including $E=0$. As $\zeta=1$ on $B_{r_1}$ and has support in $B_{r_2}$,

$$
\boxed{\int_{B_{r_1}}|\nabla u|^2\le4R^2\int_{B_{r_2}}u^2|\nabla\zeta|^2.}
$$

This [Caccioppoli inequality](../../../partial-differential-equation.md#caccioppoli-inequality) is valid for smooth solutions and, by density of admissible tests, for locally $H^1$ [weak solutions](../../../partial-differential-equation.md#weak-solution) with bounded measurable coefficients.

<h4 id="3/3/b">b</h4>

↑ **Parent:** [3](#3/3)

<h5 id="3/3/b/solution">Solution</h5>

↑ **Parent:** [B](#3/3/b)

Take $\alpha=1+1/\ell>1$. Then $2\alpha<p^*$ in every $\ell\ge2$, including $p^*=\infty$ for $\ell=2$. The supplied [Sobolev embedding theorem](../../../sobolev-space.md#sobolev-embedding-theorem), by the fixed scaling from $B_{1/2}$ to $B_1$, gives $\|w\|_{L^{2\alpha}(B_1)}\le C_\ell\|w\|_{H^1(B_1)}$.

Choose $0\le\zeta\le1$, equal to one on $B_{r_1}$, supported in $B_{r_2}$, with $|\nabla\zeta|\le C/(r_2-r_1)$. Extend $w=\zeta u$ by zero to $B_1$. The [Caccioppoli inequality](../../../partial-differential-equation.md#caccioppoli-inequality) before discarding the cutoff weight gives

$$
\|\nabla w\|_2\le\|\zeta\nabla u\|_2+\|u\nabla\zeta\|_2\le(2R+1)\|u\nabla\zeta\|_2.
$$

Also $\|w\|_2\le\|u\|_{L^2(B_{r_2})}$. Since $R>1$ and $r_2-r_1\le1$, both terms are controlled by $C R(r_2-r_1)^{-1}\|u\|_2$. Applying the [Sobolev embedding theorem](../../../sobolev-space.md#sobolev-embedding-theorem) to $w$ gives

$$
\boxed{\|u\|_{L^{2\alpha}(B_{r_1})}\le\frac{C_\ell R}{r_2-r_1}\|u\|_{L^2(B_{r_2})},\qquad\alpha=1+1/\ell.}
$$

Using a fixed ambient ball prevents the Sobolev constant from acquiring an unintended dependence on either radius.

<h4 id="3/3/c">c</h4>

↑ **Parent:** [3](#3/3)

<h5 id="3/3/c/solution">Solution</h5>

↑ **Parent:** [C](#3/3/c)

The original PDF assumes $u\ge0$ at the beginning of this question; the TeX conversion omits that hypothesis. First replace a smooth nonnegative solution by $v=u+\varepsilon>0$, which solves the same [homogeneous divergence-form elliptic equation](../../../elliptic-boundary-value-problem.md#homogeneous-divergence-form-elliptic-equation). For $w=v^{q/2}$, the [chain rule](../../../calculus.md#chain-rule) gives the favorable term

$$
\operatorname{div}(A\nabla w)=\frac q2\left(\frac q2-1\right)v^{q/2-2}A\nabla v\cdot\nabla v\ge0
$$

in the distributional sense. Thus $w$ is a [weak subsolution](../../../elliptic-boundary-value-problem.md#weak-subsolution-of-a-divergence-form-elliptic-equation). Testing its subsolution inequality with $\zeta^2w$ yields the same [Caccioppoli inequality](../../../partial-differential-equation.md#caccioppoli-inequality) as before. More precisely, testing the equation for $v$ with $\zeta^2v^{q-1}$ gives

$$
\int\zeta^2|\nabla v^{q/2}|^2\le\frac{q^2}{(q-1)^2}R^2\int v^q|\nabla\zeta|^2\le4R^2\int v^q|\nabla\zeta|^2.
$$

Indeed the main term is at least $(q-1)\lambda\int\zeta^2v^{q-2}|\nabla v|^2$, and the cross term is bounded by twice $\Lambda$ times the square roots of this weighted gradient integral and $\int v^q|\nabla\zeta|^2$. Let $\varepsilon\downarrow0$ to obtain the stated power [energy estimate](../../../partial-differential-equation.md#energy-estimate).

Apply the fixed-domain [Sobolev embedding theorem](../../../sobolev-space.md#sobolev-embedding-theorem) to $\zeta u^{q/2}$. The crucial constant stays uniform before taking the $2/q$ power:

$$
\boxed{\|u\|_{L^{q\alpha}(B_{r_1})}\le\left[\frac{D_\ell R}{r_2-r_1}\right]^{2/q}\|u\|_{L^q(B_{r_2})}\quad(q\ge2),}
$$

where $D_\ell\ge1$ is independent of $q$. This is [uniform power gain for elliptic solutions](../../../partial-differential-equation.md#uniform-power-gain-for-elliptic-solutions). The exponent is $q\alpha$, not the TeX conversion's $q^\alpha$. The PDF's weaker prefactor $C_\ell$ outside the $2/q$ power follows from this stronger estimate, but that weaker form alone cannot be iterated infinitely.

For completeness, the estimate also extends to nonnegative locally $H^1$ [weak solutions](../../../partial-differential-equation.md#weak-solution) without assuming they are already bounded. For $s\ge0$ define $F_M(s)=s^{q/2}$ up to $M$ and continue it linearly with slope $(q/2)M^{q/2-1}$ above $M$; set $\Psi_M(s)=\int_0^sF_M'(r)^2\,dr$. Both have bounded derivatives for fixed $M$. Direct calculation gives $\Psi_M/F_M'\le F_M$ and $F_M(s)\le(q/2)s^{q/2}$. Test the weak equation with $\zeta^2\Psi_M(u)$, using smooth approximations to these [Sobolev chain rule](../../../distribution-theory.md#sobolev-chain-rule) functions if needed. The resulting weighted energy bound is $\int\zeta^2|\nabla F_M(u)|^2\le4R^2\int F_M(u)^2|\nabla\zeta|^2$. If $u\in L^q(B_{r_2})$, dominated convergence on the right and the [Fatou lemma](../../../measure-theory.md#fatou-s-lemma) on the Sobolev left give the boxed gain as $M\to\infty$, with the same uniform constant. Starting with $q=2$, this justifies every subsequent iteration step.

<h4 id="3/3/d">d</h4>

↑ **Parent:** [3](#3/3)

<h5 id="3/3/d/solution">Solution</h5>

↑ **Parent:** [D](#3/3/d)

Set $q_i=2\alpha^i$, $r_i=1/2+2^{-i-1}$ and $N_i=\|u\|_{L^{q_i}(B_{r_i})}$. Then $r_0=1$, $r_i-r_{i+1}=2^{-i-2}$, and the sharper [uniform power gain for elliptic solutions](../../../partial-differential-equation.md#uniform-power-gain-for-elliptic-solutions) gives

$$
N_{i+1}\le\bigl[D_\ell R\,2^{i+2}\bigr]^{\alpha^{-i}}N_i.
$$

The [Moser product on geometric radii](../../../elliptic-boundary-value-problem.md#moser-product-on-geometric-radii) converges because

$$
S_0=\sum_{i\ge0}\alpha^{-i}=\frac\alpha{\alpha-1},\qquad S_1=\sum_{i\ge0}(i+2)\alpha^{-i}=\frac\alpha{(\alpha-1)^2}+\frac{2\alpha}{\alpha-1}.
$$

Thus every $N_i$ is at most $B=(D_\ell R)^{S_0}2^{S_1}\|u\|_{L^2(B_1)}$. Since $B_{1/2}\subset B_{r_i}$, its $L^{q_i}$ norms are also bounded by $B$. If $u>B+\delta$ on a set of positive measure $m$ in $B_{1/2}$, these norms are at least $(B+\delta)m^{1/q_i}$, tending to $B+\delta$, a contradiction. Hence

$$
\boxed{\|u\|_{L^\infty(B_{1/2})}\le(D_\ell R)^{\alpha/(\alpha-1)}2^{\alpha/(\alpha-1)^2+2\alpha/(\alpha-1)}\|u\|_{L^2(B_1)}.}
$$

This is the required [Moser iteration](../../../elliptic-boundary-value-problem.md#moser-iteration) estimate, with a finite constant depending only on $\ell$ and $R$. The weak-test truncation argument in the preceding solution makes the conclusion valid for locally $H^1$ [weak solutions](../../../partial-differential-equation.md#weak-solution) with $u\in L^2(B_1)$ and measurable uniformly elliptic coefficients. No differentiability of $A$ or unproved smooth approximation of solutions is required.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
