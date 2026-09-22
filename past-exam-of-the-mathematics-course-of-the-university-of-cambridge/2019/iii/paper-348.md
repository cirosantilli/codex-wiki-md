# Paper 348

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_348.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_348.pdf)

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
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
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
  - [d](#3/d)
    - [Solution](#3/d/solution)
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
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)

## 1

↑ **Parent:** [Paper 348](paper-348.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a cost $c:X\times Y\to[0,+\infty]$ that is a [Borel measurable function](../../../measure-theory.md#borel-measurable-function), a [transport map](../../../mathematical-optimization.md#transport-map) is a measurable $T:X\to Y$ whose [pushforward measure](../../../measure-theory.md#pushforward-measure) satisfies

$$
T_\#\mu=\nu,\qquad \mu(T^{-1}(B))=\nu(B)\quad\text{for every Borel }B\subseteq Y.
$$

The [Monge optimal transport problem](../../../mathematical-optimization.md#monge-optimal-transport-problem) moves every source point to one destination:

$$
\boxed{\inf_{T_\#\mu=\nu}\mathbb M(T),\qquad \mathbb M(T)=\int_X c(x,T(x))\,d\mu(x).}
$$

The [Kantorovich optimal transport problem](../../../mathematical-optimization.md#kantorovich-optimal-transport-problem) permits mass to split. Its admissible [transport plans](../../../mathematical-optimization.md#transport-plan) are the [probability measures](../../../probability-theory.md#probability-measure) on $X\times Y$ with prescribed [marginal distributions](../../../probability-theory.md#marginal-distribution):

$$
\Pi(\mu,\nu)=\{\pi:(p_X)_\#\pi=\mu,\ (p_Y)_\#\pi=\nu\},\qquad
\boxed{\inf_{\pi\in\Pi(\mu,\nu)}\mathbb K(\pi),\quad \mathbb K(\pi)=\int_{X\times Y}c\,d\pi.}
$$

Thus a [transport plan](../../../mathematical-optimization.md#transport-plan) is a [coupling of probability distributions](../../../probability-and-statistics.md#coupling). The set $\Pi(\mu,\nu)$ is never empty: it contains the [product measure](../../../probability-theory.md#product-measure) $\mu\otimes\nu$. Signed costs can also be used when their integrals are well defined, for example with an integrable lower bound of the form $a(x)+b(y)$.

On the [Polish space](../../../topological-analysis.md#polish-space) $\mathbb R$, take the [Dirac measures](../../../measure-theory.md#dirac-measure)

$$
\boxed{\mu=\delta_0,\qquad \nu=\tfrac12\delta_{-1}+\tfrac12\delta_1.}
$$

Every measurable map satisfies $T_\#\delta_0=\delta_{T(0)}$, which cannot equal $\nu$. A [transport map](../../../mathematical-optimization.md#transport-map) cannot split an [atom of a measure](../../../measure-theory.md#atom-measure-theory), whereas the [transport plan](../../../mathematical-optimization.md#transport-plan) $\tfrac12\delta_{(0,-1)}+\tfrac12\delta_{(0,1)}$ can.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Given any admissible [transport map](../../../mathematical-optimization.md#transport-map) $T$, form its graph [transport plan](../../../mathematical-optimization.md#transport-plan)

$$
\pi_T=(\operatorname{Id},T)_\#\mu.
$$

For [Borel sets](../../../measure-theory.md#borel-set) $A\subseteq X$ and $B\subseteq Y$, the definition of a [pushforward measure](../../../measure-theory.md#pushforward-measure) gives

$$
\pi_T(A\times Y)=\mu(A),\qquad
\pi_T(X\times B)=\mu(T^{-1}(B))=\nu(B).
$$

Hence $\pi_T\in\Pi(\mu,\nu)$. Integration against a [pushforward measure](../../../measure-theory.md#pushforward-measure) also gives

$$
\mathbb K(\pi_T)=\int_X c(x,T(x))\,d\mu(x)=\mathbb M(T).
$$

The [Kantorovich optimal transport problem](../../../mathematical-optimization.md#kantorovich-optimal-transport-problem) therefore has at least all the competitors of the [Monge optimal transport problem](../../../mathematical-optimization.md#monge-optimal-transport-problem), with exactly the same costs. Consequently

$$
\boxed{\inf_{T_\#\mu=\nu}\mathbb M(T)\ \geq\ \inf_{\pi\in\Pi(\mu,\nu)}\mathbb K(\pi).}
$$

If there is no admissible [transport map](../../../mathematical-optimization.md#transport-map), the left side is $+\infty$ by the convention $\inf\varnothing=+\infty$, so the conclusion still holds. No existence of an optimizer is needed.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The intended [monotone rearrangement](../../../mathematical-optimization.md#monotone-rearrangement) is

$$
\boxed{T^\dagger(x)=G^{-1}(F(x))\quad\mu\text{-almost everywhere}.}
$$

Here $G^{-1}$ is the [quantile function](../../../probability-theory.md#quantile-function) of $\nu$, agreeing with the ordinary inverse when $G$ is continuous and strictly increasing. With an [atomless measure](../../../measure-theory.md#non-atomic-measure) $\mu$, its [cumulative distribution function](../../../probability-theory.md#cumulative-distribution-function) $F$ is continuous, and the [probability integral transform](../../../probability-theory.md#probability-integral-transform) makes $F(X)$ uniform on $(0,1)$ for $X\sim\mu$. Thus $G^{-1}(F(X))\sim\nu$. The one-dimensional [monotone rearrangement](../../../mathematical-optimization.md#monotone-rearrangement) theorem says this [transport map](../../../mathematical-optimization.md#transport-map) minimizes the cost $d(x-y)$ for [convex](../../../real-analysis.md#convex-function) continuous $d$, whenever the cost integrals are well defined. Values at exceptional endpoints may be chosen arbitrarily.

**The printed assumptions omit an essential source condition.** Invertibility of $G$ alone does not ensure an admissible [transport map](../../../mathematical-optimization.md#transport-map). For example, $\mu=\delta_0$ and $\nu$ a [standard normal distribution](../../../probability-theory.md#standard-normal-distribution) satisfy the stated condition on $G$, but $T_\#\delta_0$ is always a [Dirac measure](../../../measure-theory.md#dirac-measure). There is no solution to the [Monge optimal transport problem](../../../mathematical-optimization.md#monge-optimal-transport-problem) in this example. The boxed answer therefore requires the additional assumption that $\mu$ is an [atomless measure](../../../measure-theory.md#non-atomic-measure), or an equivalent condition making the displayed map admissible. For arbitrary sources the always admissible monotone [transport plan](../../../mathematical-optimization.md#transport-plan) is $(F^{-1},G^{-1})_\#\mathcal U(0,1)$, which need not be induced by a map.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Interpret the invertibility assumption on $G$ as continuity and strict increase on the relevant range, so that $\nu$ is an [atomless measure](../../../measure-theory.md#non-atomic-measure). Suppose a non-decreasing [transport map](../../../mathematical-optimization.md#transport-map) $T$ with $T_\#\mu=\nu$ exists. Then $\mu$ is also an [atomless measure](../../../measure-theory.md#non-atomic-measure): if $\mu(\{x\})>0$, the [pushforward measure](../../../measure-theory.md#pushforward-measure) would give $\nu(\{T(x)\})\geq\mu(\{x\})>0$. Thus $F$ is continuous.

At any point $x$ where the non-decreasing representative is defined, the definition of a [monotone function](../../../calculus.md#monotonic-function) gives

$$
\{z:z\leq x\}\subseteq\{z:T(z)\leq T(x)\},\qquad
\{z:T(z)<T(x)\}\subseteq\{z:z<x\}.
$$

Using the [pushforward measure](../../../measure-theory.md#pushforward-measure) identity and continuity of the two [cumulative distribution functions](../../../probability-theory.md#cumulative-distribution-function), we obtain

$$
F(x)\leq G(T(x)),\qquad
G(T(x))=G(T(x)-)\leq F(x-)=F(x).
$$

Consequently

$$
\boxed{T(x)=G^{-1}(F(x))\quad\mu\text{-almost everywhere}.}
$$

The [monotone rearrangement](../../../mathematical-optimization.md#monotone-rearrangement) in part (c) is optimal for the [convex](../../../real-analysis.md#convex-function) difference cost, so $T$ has the same cost and solves the [Monge optimal transport problem](../../../mathematical-optimization.md#monge-optimal-transport-problem). The meaningful uniqueness is up to a $\mu$-null set; arbitrary values away from the source do not affect transport or cost. Existence of the non-decreasing [transport map](../../../mathematical-optimization.md#transport-map) supplies the source condition missing in part (c).

## 2

↑ **Parent:** [Paper 348](paper-348.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Write $J_T(x)=|\det DT(x)|$, the absolute [Jacobian determinant](../../../calculus.md#jacobian-determinant). Under the usual meaning of a $C^1$ map on domains, the injective [area formula](../../../calculus.md#area-formula-geometric-measure-theory) gives, for any nonnegative measurable $a$,

$$
\int_X a(T(x))J_T(x)\,dx=\int_Y a(y)\,dy.
$$

This version of the [change of variables formula](../../../calculus.md#change-of-variables-formula) does not require $DT$ to be nonsingular everywhere. A $C^1$ map is a [locally Lipschitz function](../../../real-analysis.md#locally-lipschitz-function), and the formula applies by exhaustion if the domains are unbounded. For non-open $X$, one needs the corresponding extension or regularity interpretation of the stated $C^1$ assumption.

First suppose $f(x)=g(T(x))J_T(x)$ almost everywhere with respect to [Lebesgue measure](../../../measure-theory.md#lebesgue-measure). For each bounded nonnegative measurable $a$,

$$
\int_X a(T(x))f(x)\,dx
=\int_X a(T(x))g(T(x))J_T(x)\,dx
=\int_Y a(y)g(y)\,dy.
$$

Taking [indicator functions](../../../measure-theory.md#indicator-function) proves $T_\#\mu=\nu$.

Conversely, the [area formula](../../../calculus.md#area-formula-geometric-measure-theory) shows that the measure $\widetilde\mu$ with [probability density function](../../../continuous-probability-distribution.md#probability-density-function) $g(T(x))J_T(x)$ has total mass one and satisfies $T_\#\widetilde\mu=\nu$. The assumed equality $T_\#\mu=\nu$ then implies $\mu=\widetilde\mu$, since the measurable [bijection](../../../function.md#bijection) $T$ has a measurable inverse on these domains. Equivalently, apply both [pushforward measure](../../../measure-theory.md#pushforward-measure) identities to $T(A)$ for each [Borel set](../../../measure-theory.md#borel-set) $A\subseteq X$. Uniqueness of the [Radon-Nikodym derivative](../../../measure-theory.md#radon-nikodym-derivative) yields

$$
\boxed{T_\#\mu=\nu\quad\Longleftrightarrow\quad f(x)=g(T(x))|\det DT(x)|\ \text{Lebesgue-almost everywhere}.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Restrict $\varphi$ to an arbitrary [line segment](../../../mathematical-optimization.md#line-segment) by defining $q(t)=\varphi((1-t)x+ty)$ for $0\leq t\leq1$. The [chain rule](../../../calculus.md#chain-rule) and the assumed [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix) condition on the [Hessian matrix](../../../calculus.md#hessian-matrix) give

$$
q''(t)=(y-x)^\top D^2\varphi((1-t)x+ty)(y-x)\geq0.
$$

Thus $q'$ is non-decreasing. For $0<t<1$, integrating $q'$ on the two subintervals gives

$$
\frac{q(t)-q(0)}t\leq\frac{q(1)-q(t)}{1-t}.
$$

Rearranging, and including the immediate endpoint cases, yields

$$
\boxed{\varphi((1-t)x+ty)\leq(1-t)\varphi(x)+t\varphi(y)\quad(0\leq t\leq1).}
$$

This is precisely the definition of a [convex function](../../../real-analysis.md#convex-function).

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

**Use the intended strong convexity bound** $\gamma^\top D^2\varphi(x)\gamma\geq\lambda|\gamma|^2$. The original PDF omits $|\gamma|^2$ on the right. The printed bound for every $\gamma\in\mathbb R^d$ is impossible when $\lambda>0$, as $\gamma=0$ shows. Equivalently, the intended bound is stated for unit vectors. The norm of $D^2\zeta$ is the [operator norm](../../../continuous-dual-space.md#operator-norm) induced by the [Euclidean norm](../../../functional-analysis.md#euclidean-norm), or any matrix [norm](../../../functional-analysis.md#norm) that bounds it.

Set

$$
\boxed{\varphi_\varepsilon=\varphi+\varepsilon\zeta,\qquad T_\varepsilon=\nabla\varphi_\varepsilon.}
$$

This function is $C^2$, and its [Hessian matrix](../../../calculus.md#hessian-matrix) satisfies

$$
\begin{aligned}
\gamma^\top D^2\varphi_\varepsilon(x)\gamma
&=\gamma^\top D^2\varphi(x)\gamma+\varepsilon\gamma^\top D^2\zeta(x)\gamma\\
&\geq\bigl(\lambda-\varepsilon\|D^2\zeta(x)\|_{\mathrm{op}}\bigr)|\gamma|^2\geq0.
\end{aligned}
$$

Part (i) therefore proves that $\varphi_\varepsilon$ is a [convex function](../../../real-analysis.md#convex-function). The perturbation can use up the entire positive lower bound defining a [strongly convex function](../../../real-analysis.md#strongly-convex-function); only [convexity](../../../real-analysis.md#convex-function), rather than strict positivity of the [Hessian matrix](../../../calculus.md#hessian-matrix), is asserted.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For every admissible [transport map](../../../mathematical-optimization.md#transport-map) $T$, the [pushforward measure](../../../measure-theory.md#pushforward-measure) condition gives $T(x)\in[1,2]$ for $\mu$-almost every $x\in[0,1]$. Hence $|T(x)-x|=T(x)-x$, and

$$
\int_0^1(T(x)-x)\,dx
=\int_1^2 y\,dy-\int_0^1x\,dx=1.
$$

Apply the [Jensen inequality](../../../real-analysis.md#jensen-s-inequality) to the [convex function](../../../real-analysis.md#convex-function) $h$ and the [probability measure](../../../probability-theory.md#probability-measure) $\mu$:

$$
\mathbb M(T)=\int_0^1h(T(x)-x)\,dx\geq h\left(\int_0^1(T(x)-x)\,dx\right)=h(1).
$$

Translation by one sends the source [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) to the target [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution), so $T^\dagger(x)=x+1$ is admissible. Its displacement is constantly one, giving

$$
\boxed{T^\dagger(x)=x+1,\qquad\min_{T_\#\mu=\nu}\mathbb M(T)=h(1).}
$$

No monotonicity assumption on $h$ is needed, because all displacements have the same sign. The same argument with a [transport plan](../../../mathematical-optimization.md#transport-plan) also gives the identical minimum for the [Kantorovich optimal transport problem](../../../mathematical-optimization.md#kantorovich-optimal-transport-problem).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

As in part (c), every admissible [transport map](../../../mathematical-optimization.md#transport-map) has nonnegative displacement $D(x)=T(x)-x$ with $\int_0^1D(x)\,dx=1$. The square root is a [strictly concave function](../../../real-analysis.md#strictly-concave-function), so the reversed [Jensen inequality](../../../real-analysis.md#jensen-s-inequality) gives

$$
\mathbb M(T)=\int_0^1\sqrt{D(x)}\,dx\leq\sqrt{\int_0^1D(x)\,dx}=1.
$$

The map $T^\dagger(x)=x+1$ is admissible and attains one. Therefore

$$
\boxed{\max_{T_\#\mu=\nu}\mathbb M(T)=1,\qquad T^\dagger(x)=x+1.}
$$

Thus “worst” means largest cost among admissible [transport maps](../../../mathematical-optimization.md#transport-map). Equality in the [Jensen inequality](../../../real-analysis.md#jensen-s-inequality) for a [strictly concave function](../../../real-analysis.md#strictly-concave-function) forces $D(x)$ to be constant almost everywhere, so this maximizer is unique up to a $\mu$-null set. For comparison, the admissible reflection $T(x)=2-x$ has smaller cost

$$
\int_0^1\sqrt{2-2x}\,dx=\frac{2\sqrt2}{3}<1.
$$

The upper bound also holds for every [transport plan](../../../mathematical-optimization.md#transport-plan).

## 3

↑ **Parent:** [Paper 348](paper-348.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The dual of the [Kantorovich optimal transport problem](../../../mathematical-optimization.md#kantorovich-optimal-transport-problem) is

$$
\boxed{\sup_{(u,v)\in\mathcal A_c}\left\{\int_Xu\,d\mu+\int_Yv\,d\nu\right\},}
$$

where the [Kantorovich potentials](../../../mathematical-optimization.md#kantorovich-potential) are measurable representatives satisfying

$$
\mathcal A_c=\{(u,v):u\in L^1(\mu),\ v\in L^1(\nu),\ u(x)+v(y)\leq c(x,y)\ \text{for every }(x,y)\in X\times Y\}.
$$

One standard form of the [Kantorovich duality theorem](../../../mathematical-optimization.md#kantorovich-duality-theorem) assumes that $X,Y$ are [Polish spaces](../../../topological-analysis.md#polish-space), $\mu,\nu$ are [probability measures](../../../probability-theory.md#probability-measure) defined as [Borel measures](../../../measure-theory.md#borel-measure), and $c:X\times Y\to[0,+\infty]$ is [sequentially lower semicontinuous](../../../calculus.md#sequential-lower-semicontinuity). Then

$$
\boxed{\min_{\pi\in\Pi(\mu,\nu)}\int c\,d\pi
=\sup_{(u,v)\in\mathcal A_c}\left(\int u\,d\mu+\int v\,d\nu\right).}
$$

The primal infimum is attained; its value may be $+\infty$. Nonnegativity can be replaced by a constant lower bound by shifting the cost. This duality for lower semicontinuous costs is also discussed in [Beiglboeck, Leonard and Schachermayer's duality paper](https://arxiv.org/abs/0911.4347).

**Equality of values does not by itself assert a dual maximum.** A sufficient stronger setting for attainment on both sides is [compact metric spaces](../../../topological-analysis.md#compact-metric-space) $X,Y$ and a finite [continuous](../../../calculus.md#continuous-function) cost $c$; then [continuous](../../../calculus.md#continuous-function) [Kantorovich potentials](../../../mathematical-optimization.md#kantorovich-potential) attain the dual supremum. The general statement above correctly uses a supremum.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Fix any admissible pair of [Kantorovich potentials](../../../mathematical-optimization.md#kantorovich-potential) $(u,v)$ and any [transport plan](../../../mathematical-optimization.md#transport-plan) $\pi\in\Pi(\mu,\nu)$. Its [marginal distributions](../../../probability-theory.md#marginal-distribution) give

$$
\int_Xu\,d\mu+\int_Yv\,d\nu
=\int_{X\times Y}(u(x)+v(y))\,d\pi(x,y).
$$

The right side is well defined because $u(x)$ and $v(y)$ are [Lebesgue integrable](../../../measure-theory.md#lebesgue-integrable-function) with respect to $\pi$. Integrating their pointwise feasibility inequality gives

$$
\int_Xu\,d\mu+\int_Yv\,d\nu\leq\int_{X\times Y}c(x,y)\,d\pi(x,y).
$$

Since this holds for every feasible pair and every [transport plan](../../../mathematical-optimization.md#transport-plan),

$$
\boxed{\sup_{(u,v)\in\mathcal A_c}\left(\int u\,d\mu+\int v\,d\nu\right)\leq\inf_{\pi\in\Pi(\mu,\nu)}\mathbb K(\pi).}
$$

This proves the required inequality directly from the transport constraints, without any [convex optimization](../../../convex-optimization.md) duality theorem. Whenever the extrema are attained, the supremum and infimum can respectively be written as a maximum and minimum. Even the [Kantorovich duality theorem](../../../mathematical-optimization.md#kantorovich-duality-theorem) is unnecessary for this direction.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The [Kantorovich–Rubinstein theorem](../../../probability-and-statistics.md#kantorovich-rubinstein-theorem) concerns a [Polish space](../../../topological-analysis.md#polish-space) $(X,\rho)$ and [probability measures](../../../probability-theory.md#probability-measure) $\mu,\nu$ with finite first [moments](../../../probability-theory.md#moment), meaning $\int\rho(x,x_0)\,d\mu(x)+\int\rho(x,x_0)\,d\nu(x)<\infty$ for one, hence every, $x_0\in X$. It states

$$
\boxed{W_1(\mu,\nu)=\inf_{\pi\in\Pi(\mu,\nu)}\int\rho(x,y)\,d\pi
=\sup_{\operatorname{Lip}(f)\leq1}\left\{\int f\,d\mu-\int f\,d\nu\right\}.}
$$

Here $\operatorname{Lip}(f)\leq1$ means $|f(x)-f(y)|\leq\rho(x,y)$ for every $x,y$. The [Wasserstein distance](../../../probability-and-statistics.md#wasserstein-distance) with ground cost $\rho$ therefore equals a supremum over functions with [Lipschitz constant](../../../real-analysis.md#lipschitz-constant) at most one. One may normalize $f(x_0)=0$, since adding a constant does not change the difference of integrals. This normalization bounds $|f(x)|$ by $\rho(x,x_0)$, so finite first [moments](../../../probability-theory.md#moment) ensure integrability. The supremum is unchanged if an absolute value is placed around the difference, because $-f$ is admissible whenever $f$ is.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Put $\nu=(T^\dagger)_\#\mu$ and use the two [Kantorovich potentials](../../../mathematical-optimization.md#kantorovich-potential)

$$
u(x)=(1-\lambda)|x|^2,\qquad
v(y)=\left(1-\frac1\lambda\right)|y|^2.
$$

For every $x,y\in\mathbb R^d$,

$$
\begin{aligned}
|x-y|^2-u(x)-v(y)
&=\lambda|x|^2+\lambda^{-1}|y|^2-2x\cdot y\\
&=\lambda^{-1}|y-\lambda x|^2\geq0.
\end{aligned}
$$

Thus the pair is dual feasible, with equality precisely on $y=\lambda x$. Finite second [moments](../../../probability-theory.md#moment) make both potentials integrable; compactness of $X$ is more than sufficient. For any admissible [transport map](../../../mathematical-optimization.md#transport-map) $T$, integrating the inequality and using its [pushforward measure](../../../measure-theory.md#pushforward-measure) gives

$$
\int|x-T(x)|^2\,d\mu\geq\int u\,d\mu+\int v\,d\nu.
$$

The admissible map $T^\dagger(x)=\lambda x$ attains equality. Consequently

$$
\boxed{T^\dagger(x)=\lambda x\ \text{is optimal},\qquad\min\mathbb M=(1-\lambda)^2\int|x|^2\,d\mu.}
$$

The same certificate proves optimality of its graph [transport plan](../../../mathematical-optimization.md#transport-plan) among all [transport plans](../../../mathematical-optimization.md#transport-plan). Notice that $u$ need not be a [convex function](../../../real-analysis.md#convex-function) when $\lambda>1$: it is a cost dual potential. The associated [convex](../../../real-analysis.md#convex-function) gradient potential is instead $\Phi(x)=\lambda|x|^2/2$.

## 4

↑ **Parent:** [Paper 348](paper-348.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For [probability measures](../../../probability-theory.md#probability-measure) $\mu,\nu$ on $\mathbb R^d$ with finite second [moments](../../../probability-theory.md#moment), the [Knott–Smith optimality criterion](../../../mathematical-optimization.md#knott-smith-optimality-criterion) states that a [transport plan](../../../mathematical-optimization.md#transport-plan) $\pi\in\Pi(\mu,\nu)$ minimizes the quadratic cost $|x-y|^2$ if and only if there is a [proper convex function](../../../real-analysis.md#proper-convex-function) $\Phi:\mathbb R^d\to\mathbb R\cup\{+\infty\}$ that is [sequentially lower semicontinuous](../../../calculus.md#sequential-lower-semicontinuity) and satisfies

$$
\boxed{y\in\partial\Phi(x)\quad\text{for }\pi\text{-almost every }(x,y).}
$$

The [subdifferential](../../../convex-optimization.md#subdifferential) is characterized by

$$
y\in\partial\Phi(x)\quad\Longleftrightarrow\quad
\Phi(z)\geq\Phi(x)+y\cdot(z-x)\quad\text{for every }z\in\mathbb R^d,
$$

with $\Phi(x)<\infty$. Thus the [transport plan](../../../mathematical-optimization.md#transport-plan) is concentrated on the graph of the [subdifferential](../../../convex-optimization.md#subdifferential). No [absolute continuity of measures](../../../measure-theory.md#absolute-continuity-of-measures) assumption on $\mu$ is needed. Multiplying the cost by $1/2$ leaves the criterion unchanged. The original quadratic optimal mapping result is [Knott and Smith, On the optimal mapping of distributions](https://link.springer.com/article/10.1007/BF00934745).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

A standard sufficient form of [Brenier theorem](../../../mathematical-optimization.md#brenier-theorem) assumes $\mu,\nu\in\mathcal P(\mathbb R^d)$ have finite second [moments](../../../probability-theory.md#moment) and $\mu\ll\mathcal L^d$, that is, [absolute continuity of measures](../../../measure-theory.md#absolute-continuity-of-measures) with respect to [Lebesgue measure](../../../measure-theory.md#lebesgue-measure). For the cost $|x-y|^2$, there exists a unique optimal [transport plan](../../../mathematical-optimization.md#transport-plan), and it is induced by a [transport map](../../../mathematical-optimization.md#transport-map):

$$
\boxed{\pi^\dagger=(\operatorname{Id},\nabla\Phi)_\#\mu,\qquad T^\dagger=\nabla\Phi,\qquad(\nabla\Phi)_\#\mu=\nu.}
$$

Here $\Phi$ is a [proper convex function](../../../real-analysis.md#proper-convex-function), which may be chosen [sequentially lower semicontinuous](../../../calculus.md#sequential-lower-semicontinuity), and its [gradient](../../../calculus.md#gradient) exists $\mu$-almost everywhere. The map $\nabla\Phi$ is unique $\mu$-almost everywhere and is the unique minimizer of the [Monge optimal transport problem](../../../mathematical-optimization.md#monge-optimal-transport-problem); its cost equals the [Kantorovich optimal transport problem](../../../mathematical-optimization.md#kantorovich-optimal-transport-problem) minimum. Equivalently, it is the unique [gradient](../../../calculus.md#gradient) of a [convex function](../../../real-analysis.md#convex-function) transporting $\mu$ to $\nu$.

The uniqueness claim concerns the map and the [transport plan](../../../mathematical-optimization.md#transport-plan), not a globally unique potential. The potential may be shifted by a constant, and additional nonuniqueness away from the source can occur. No density assumption is required on $\nu$. A primary reference is [Brenier's Polar factorization and monotone rearrangement of vector-valued functions](https://www.ceremade.dauphine.fr/~carlier/Brenier91.pdf).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Let $\Phi=\varphi_\varepsilon$ and let $\Phi^*$ denote its [convex conjugate](../../../convex-optimization.md#convex-conjugate). Its [Fenchel–Young gap](../../../convex-optimization.md#fenchel-young-gap)

$$
H(x,y)=\Phi(x)+\Phi^*(y)-x\cdot y
$$

is nonnegative by the [Fenchel–Young inequality](../../../convex-optimization.md#fenchel-young-inequality), and the hypothesis says $\int H\,d\pi_\varepsilon\leq\varepsilon$.

First justify the integrability needed for the certificate. Finite second [moments](../../../probability-theory.md#moment) and the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) imply, for every [transport plan](../../../mathematical-optimization.md#transport-plan) $\pi$,

$$
\int|x\cdot y|\,d\pi\leq
\left(\int|x|^2\,d\mu\right)^{1/2}
\left(\int|y|^2\,d\nu\right)^{1/2}<\infty.
$$

Since $\Phi\in L^1(\mu)$ and $H\in L^1(\pi_\varepsilon)$, the identity $\Phi^*(y)=H(x,y)-\Phi(x)+x\cdot y$ proves $\Phi^*\in L^1(\nu)$ by the [marginal distribution](../../../probability-theory.md#marginal-distribution) property. In particular, no subtraction of infinite integrals is being used.

Set

$$
u(x)=\tfrac12|x|^2-\Phi(x),\qquad
v(y)=\tfrac12|y|^2-\Phi^*(y),\qquad
D=\int u\,d\mu+\int v\,d\nu.
$$

These are integrable [Kantorovich potentials](../../../mathematical-optimization.md#kantorovich-potential). The [Fenchel–Young inequality](../../../convex-optimization.md#fenchel-young-inequality) gives $u(x)+v(y)\leq\tfrac12|x-y|^2$. More precisely, for every [transport plan](../../../mathematical-optimization.md#transport-plan) $\pi$,

$$
\mathbb K(\pi)=D+\int H\,d\pi\geq D,
\qquad\mathbb K(\pi_\varepsilon)=D+\int H\,d\pi_\varepsilon\leq D+\varepsilon.
$$

Taking the infimum in the first inequality therefore proves

$$
\boxed{\mathbb K(\pi_\varepsilon)\leq\inf_{\pi\in\Pi(\mu,\nu)}\mathbb K(\pi)+\varepsilon.}
$$

The factor $1/2$ in the quadratic cost is essential for this exact gap identity.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Define $T^\dagger(0)=0$; the printed quotient is undefined at the origin, but this continuous extension changes no transport cost because $\mu(\{0\})=0$. In [polar coordinates](../../../calculus.md#polar-coordinates), the two [probability density functions](../../../continuous-probability-distribution.md#probability-density-function) give

$$
\mu\{|x|\leq r\}=r^2,\qquad
\nu\{|y|\leq s\}=s^4\quad(0\leq r,s\leq1).
$$

Both angular distributions are uniform, with [independence](../../../random-variable.md#independent-random-variables) of angle and radius. The proposed [transport map](../../../mathematical-optimization.md#transport-map) preserves the angle and sends $r$ to $s=\sqrt r$. Therefore

$$
\mu\{|T^\dagger(x)|\leq s\}=\mu\{|x|\leq s^2\}=s^4,
$$

and preservation of the angle proves $(T^\dagger)_\#\mu=\nu$. As a local check using the [Jacobian determinant](../../../calculus.md#jacobian-determinant), its radial and tangential derivatives for $r>0$ are $1/(2\sqrt r)$ and $1/\sqrt r$, respectively, so $\det DT^\dagger=1/(2r)$ and $g(T^\dagger(x))\det DT^\dagger(x)=(2r/\pi)/(2r)=f(x)$.

Now use the [convex function](../../../real-analysis.md#convex-function)

$$
\Phi(x)=\frac23|x|^{3/2}\quad(x\in\mathbb R^2).
$$

It is [convex](../../../real-analysis.md#convex-function) because the [Euclidean norm](../../../functional-analysis.md#euclidean-norm) is [convex](../../../real-analysis.md#convex-function) and $s\mapsto(2/3)s^{3/2}$ is increasing and [convex](../../../real-analysis.md#convex-function) on $[0,\infty)$. It is [differentiable](../../../analysis.md#differentiable-function), including at zero, and

$$
\boxed{\nabla\Phi(x)=T^\dagger(x)=\frac{x}{\sqrt{|x|}}\ (x\ne0),\qquad\nabla\Phi(0)=0.}
$$

Its graph [transport plan](../../../mathematical-optimization.md#transport-plan) lies in the graph of $\partial\Phi$, so the [Knott–Smith optimality criterion](../../../mathematical-optimization.md#knott-smith-optimality-criterion) proves quadratic optimality. Since that plan is induced by a map, part 1(b) proves optimality for the [Monge optimal transport problem](../../../mathematical-optimization.md#monge-optimal-transport-problem) as well. The minimum provides a useful independent check:

$$
\boxed{\min\mathbb M=\int_0^1(r-\sqrt r)^2\,2r\,dr
=\frac12-\frac87+\frac23=\frac1{42}.}
$$

## 5

↑ **Parent:** [Paper 348](paper-348.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

For $1\leq p<\infty$, define the [probability measures](../../../probability-theory.md#probability-measure) with finite $p$th [absolute moment](../../../probability-theory.md#absolute-moment) by

$$
\mathcal P_p(X)=\left\{\mu\in\mathcal P(X):\int_X|x-x_0|^p\,d\mu(x)<\infty\right\},
$$

where $x_0\in X$ is any fixed reference point. The condition is independent of the choice of $x_0$. The [p-Wasserstein distance](../../../probability-and-statistics.md#p-wasserstein-distance) is

$$
\boxed{d_{W_p}(\mu,\nu)=W_p(\mu,\nu)
=\left(\inf_{\pi\in\Pi(\mu,\nu)}\int_{X\times X}|x-y|^p\,d\pi(x,y)\right)^{1/p}.}
$$

The infimum is over all [transport plans](../../../mathematical-optimization.md#transport-plan), rather than only [transport maps](../../../mathematical-optimization.md#transport-map). The [product measure](../../../probability-theory.md#product-measure) gives a finite upper bound using

$$
|x-y|^p\leq2^{p-1}\bigl(|x-x_0|^p+|y-x_0|^p\bigr).
$$

For $p=1$ this is the [Wasserstein distance](../../../probability-and-statistics.md#wasserstein-distance) with the metric of [Euclidean space](../../../functional-analysis.md#euclidean-norm); for $p=2$ it is the [second Wasserstein distance](../../../probability-and-statistics.md#second-wasserstein-distance). “Bounded moment” here means a finite integral, and does not require $X$ to be bounded.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Let $D=\operatorname{diam}(X)<\infty$, and first suppose $1\leq p\leq q<\infty$. On any [transport plan](../../../mathematical-optimization.md#transport-plan) $\pi$, which has total mass one, the [Holder inequality](../../../functional-analysis.md#holder-inequality) gives

$$
\left(\int|x-y|^p\,d\pi\right)^{1/p}
\leq\left(\int|x-y|^q\,d\pi\right)^{1/q}.
$$

Also, $|x-y|\leq D$ gives

$$
\int|x-y|^q\,d\pi\leq D^{q-p}\int|x-y|^p\,d\pi.
$$

Taking infima, or using arbitrarily close competitors if an infimum is not attained, yields

$$
\boxed{W_p(\mu,\nu)\leq W_q(\mu,\nu)
\leq D^{1-p/q}W_p(\mu,\nu)^{p/q}.}
$$

For $p=q$ the two distances coincide, and if $D=0$ there is only one [probability measure](../../../probability-theory.md#probability-measure), so the conclusion is immediate. For $D>0$ and $p<q$, the displayed bounds imply both directions of

$$
\boxed{W_p(\mu_n,\mu)\to0\quad\Longleftrightarrow\quad W_q(\mu_n,\mu)\to0.}
$$

For $q<p$, exchange the exponents. Thus all finite-order [p-Wasserstein distances](../../../probability-and-statistics.md#p-wasserstein-distance) induce the same convergence on a bounded subset of $\mathbb R^d$. Closedness of $X$ is not required for these estimates.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Write $L=W_p(\mu,\nu)$. The assumed equality of the [Monge optimal transport problem](../../../mathematical-optimization.md#monge-optimal-transport-problem) and [Kantorovich optimal transport problem](../../../mathematical-optimization.md#kantorovich-optimal-transport-problem) values gives

$$
\int|T^\dagger(x)-x|^p\,d\mu(x)=L^p.
$$

Each interpolated [pushforward measure](../../../measure-theory.md#pushforward-measure) $\mu_t=(P_t)_\#\mu$ has a finite $p$th [absolute moment](../../../probability-theory.md#absolute-moment), since $|P_t(x)|^p\leq2^{p-1}(|x|^p+|T^\dagger(x)|^p)$ and $(T^\dagger)_\#\mu=\nu$.

For any $s,t\in[0,1]$, the common-source [transport plan](../../../mathematical-optimization.md#transport-plan)

$$
\pi_{s,t}=(P_s,P_t)_\#\mu\in\Pi(\mu_s,\mu_t)
$$

provides the upper bound

$$
W_p(\mu_s,\mu_t)^p\leq\int|P_t(x)-P_s(x)|^p\,d\mu
=|t-s|^p L^p.
$$

For the reverse bound assume $0\leq s\leq t\leq1$. Since $\mu_0=\mu$ and $\mu_1=\nu$, the [triangle inequality](../../../topological-analysis.md#triangle-inequality) for the [p-Wasserstein distance](../../../probability-and-statistics.md#p-wasserstein-distance) and the upper bounds already established give

$$
\begin{aligned}
L&\leq W_p(\mu_0,\mu_s)+W_p(\mu_s,\mu_t)+W_p(\mu_t,\mu_1)\\
&\leq sL+W_p(\mu_s,\mu_t)+(1-t)L.
\end{aligned}
$$

Hence $W_p(\mu_s,\mu_t)\geq(t-s)L$. Combining the bounds and using symmetry proves

$$
\boxed{W_p(\mu_t,\mu_s)=|t-s|W_p(\mu,\nu).}
$$

This is the constant speed property of [displacement interpolation](../../../probability-and-statistics.md#displacement-interpolation). The given invertibility of $P_s$ also lets one realize the competitor as the map $P_t\circ P_s^{-1}$, assuming its inverse is measurable, but the [transport plan](../../../mathematical-optimization.md#transport-plan) argument proves the result without invertibility.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

Let $\Delta=\{(x,y):x=y\}$. For any [transport plan](../../../mathematical-optimization.md#transport-plan) $\pi$ and any [Borel set](../../../measure-theory.md#borel-set) $A$,

$$
\mu(A)-\nu(A)=\pi(A\times A^c)-\pi(A^c\times A).
$$

Both rectangles are contained in $\Delta^c$, so

$$
|\mu(A)-\nu(A)|\leq\pi(\Delta^c)=\mathbb K(\pi).
$$

Thus $\inf\mathbb K\geq\sup_A|\mu(A)-\nu(A)|$.

To attain this bound, use the [dominating measure](../../../measure-theory.md#dominating-measure) $\rho=\mu+\nu$ and [Radon-Nikodym derivatives](../../../measure-theory.md#radon-nikodym-derivative) $f=d\mu/d\rho$, $g=d\nu/d\rho$. Define the common measure and residual mass by

$$
d\alpha=\min(f,g)\,d\rho,\qquad r=1-\alpha(\mathbb R^d).
$$

Since $\int(f-g)\,d\rho=0$, the positive and negative parts have equal mass. Taking $A=\{f>g\}$ gives

$$
r=\int(f-g)_+\,d\rho=\frac12\int|f-g|\,d\rho
=\sup_A|\mu(A)-\nu(A)|.
$$

If $r=0$, then $\mu=\nu$ and the diagonal [transport plan](../../../mathematical-optimization.md#transport-plan) has zero cost. If $r>0$, put $\beta=\mu-\alpha$, $\gamma=\nu-\alpha$ and define

$$
\pi^\dagger=(\operatorname{Id},\operatorname{Id})_\#\alpha+\frac1r\,\beta\otimes\gamma.
$$

The residual measures each have mass $r$, so the [marginal distributions](../../../probability-theory.md#marginal-distribution) of $\pi^\dagger$ are $\alpha+\beta=\mu$ and $\alpha+\gamma=\nu$, and its total mass is $1-r+r=1$. They are [mutually singular measures](../../../measure-theory.md#mutually-singular-measures), concentrated respectively on $\{f>g\}$ and $\{g>f\}$. Their [product measure](../../../probability-theory.md#product-measure) therefore gives no mass to $\Delta$, and $\mathbb K(\pi^\dagger)=r$. This is a [maximal coupling](../../../probability-and-statistics.md#maximal-coupling).

In the paper's convention for the zero-mass signed measure $\mu-\nu$, the answer is

$$
\boxed{\inf_{\pi\in\Pi(\mu,\nu)}\mathbb K(\pi)
=\sup_A|\mu(A)-\nu(A)|=\frac12\|\mu-\nu\|_{\mathrm{TV}}.}
$$

The repository's [total variation distance](../../../probability-and-statistics.md#total-variation-distance) uses the supremum itself. The paper's formula $2\sup_A|\sigma(A)|$ agrees with the usual total variation norm when $\sigma$ has total mass zero, as here; it is not the usual norm for an arbitrary positive measure. All suprema above are over [Borel sets](../../../measure-theory.md#borel-set).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
