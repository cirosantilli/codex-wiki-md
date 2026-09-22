# Paper 36

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_36.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_36.pdf)

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
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
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
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [statistical path](../../../statistical-model.md#statistical-path) through $P$ is a family $t\mapsto P_t\in\mathcal P$, defined on an open interval containing zero, with $P_0=P$. Write $p_t=dP_t/d\mu$ and $p=p_0$. Its [differentiability in quadratic mean](../../../statistical-model.md#differentiability-in-quadratic-mean) at zero means that there is a [square-integrable function](../../../measure-theory.md#square-integrable-function) $g\in L^2(P)$ such that

$$
\boxed{\int\left(\sqrt{p_t}-\sqrt p-\frac t2g\sqrt p\right)^2\,d\mu=o(t^2).}
$$

The [function](../../../function.md) $g$ is the [score function](../../../statistical-modelling.md#informant-function) of the [statistical path](../../../statistical-model.md#statistical-path). Thus it is the [derivative](../../../calculus.md#derivative) of the square-root [probability density function](../../../continuous-probability-distribution.md#probability-density-function), multiplied by two and divided by $\sqrt p$ where $p>0$. The [score function](../../../statistical-modelling.md#informant-function) is determined only $P$-almost everywhere. The displayed definition also controls any probability mass entering a region where $p=0$; a pointwise [derivative](../../../calculus.md#derivative) of the log [probability density function](../../../continuous-probability-distribution.md#probability-density-function) alone would not do that. **The required [derivative](../../../calculus.md#derivative) is in the square-root-density $L^2$ [norm](../../../functional-analysis.md#norm).**

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Put $r_t=\sqrt{p_t}-\sqrt p-(t/2)g\sqrt p$. By [differentiability in quadratic mean](../../../statistical-model.md#differentiability-in-quadratic-mean), $\|r_t\|_{L^2(\mu)}=o(|t|)$ and

$$
\frac{\sqrt{p_t}-\sqrt p}{t}\longrightarrow\frac12g\sqrt p,
\qquad
\sqrt{p_t}+\sqrt p\longrightarrow2\sqrt p
$$

in [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space). The second limit follows because the first gives $\|\sqrt{p_t}-\sqrt p\|_2=O(|t|)$.

Both [probability density functions](../../../continuous-probability-distribution.md#probability-density-function) integrate to one. Consequently the [L2 inner product](../../../measure-theory.md#l2-inner-product) satisfies

$$
0=\frac1t\int(p_t-p)\,d\mu
=\left\langle\frac{\sqrt{p_t}-\sqrt p}{t},\sqrt{p_t}+\sqrt p\right\rangle_{L^2(\mu)}.
$$

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) permits passage to the limit in this [inner product](../../../linear-algebra.md#inner-product), giving

$$
\boxed{Pg=\int g\,dP=0.}
$$

Thus every [score function](../../../statistical-modelling.md#informant-function) is a [mean-zero function](../../../probability-theory.md#mean-zero-function). This proof uses square-root [differentiability in quadratic mean](../../../statistical-model.md#differentiability-in-quadratic-mean), without requiring differentiation under the density [integral](../../../calculus.md#integral).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Fix $P=P_{\theta,\eta}$. Let $\mathcal N$ be the [nuisance tangent space](../../../statistical-inference.md#nuisance-tangent-space): the closed linear span in $L^2(P)$ of [score functions](../../../statistical-modelling.md#informant-function) of [statistical paths](../../../statistical-model.md#statistical-path) that vary only the [nuisance parameter](../../../statistical-model.md#nuisance-parameter) $\eta$. By the preceding argument, $\mathcal N$ is contained in the [mean-zero L2 space](../../../measure-theory.md#mean-zero-l2-space) $L^2_0(P)$.

Let $\Pi_{\mathcal N}$ denote [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) onto this [closed subspace of a Hilbert space](../../../hilbert-space.md#closed-subspace-of-a-hilbert-space). The [efficient score](../../../statistical-inference.md#efficient-score) and scalar [efficient information](../../../statistical-inference.md#efficient-information) are

$$
\boxed{\widetilde\ell_{\theta,\eta}=\dot\ell_{\theta,\eta}-\Pi_{\mathcal N}\dot\ell_{\theta,\eta},
\qquad
\widetilde I_{\theta,\eta}=P_{\theta,\eta}\widetilde\ell_{\theta,\eta}^{\,2}.}
$$

The [efficient score](../../../statistical-inference.md#efficient-score) is the component of the parametric [score function](../../../statistical-modelling.md#informant-function) that cannot be reproduced by changing the [nuisance parameter](../../../statistical-model.md#nuisance-parameter). The [efficient information](../../../statistical-inference.md#efficient-information) is its squared [L2 norm](../../../real-analysis.md#l2-norm); it can be zero, so positivity must not be assumed in the definition.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The map $h\mapsto Ph$ is a [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional) on [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space), since $|Ph|\leq\|h\|_2$ by the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality). Its kernel, the [mean-zero L2 space](../../../measure-theory.md#mean-zero-l2-space), is therefore closed. Every nuisance [score function](../../../statistical-modelling.md#informant-function) and the parametric [score function](../../../statistical-modelling.md#informant-function) $\dot\ell$ are centered, so both $\Pi_{\mathcal N}\dot\ell$ and $\widetilde\ell$ are centered. Hence

$$
\boxed{P\widetilde\ell=0.}
$$

Moreover, the [efficient score](../../../statistical-inference.md#efficient-score) belongs to the [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) of the [nuisance tangent space](../../../statistical-inference.md#nuisance-tangent-space). Writing $\dot\ell=\widetilde\ell+\Pi_{\mathcal N}\dot\ell$ gives

$$
P(\dot\ell\widetilde\ell)
=P\widetilde\ell^2+P\bigl((\Pi_{\mathcal N}\dot\ell)\widetilde\ell\bigr)
=\boxed{\widetilde I}.
$$

This is the [efficient-score projection identity](../../../statistical-inference.md#efficient-score-projection-identity); it remains valid when the [efficient information](../../../statistical-inference.md#efficient-information) is zero.

## 2

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Choose a collection of [statistical paths](../../../statistical-model.md#statistical-path) through $P_f$ that are [differentiable in quadratic mean](../../../statistical-model.md#differentiability-in-quadratic-mean). A [statistical tangent set](../../../statistical-model.md#statistical-tangent-set) at $P_f$ is the set of their [score functions](../../../statistical-modelling.md#informant-function). In particular each member belongs to $L^2_0(P_f)$, by the [mean-zero score identity under quadratic-mean differentiability](../../../statistical-model.md#mean-zero-score-identity-under-quadratic-mean-differentiability).

A [statistical tangent set](../../../statistical-model.md#statistical-tangent-set) records which first-order directions the chosen [statistical paths](../../../statistical-model.md#statistical-path) can realize. Its closed linear span in [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space) is the [statistical tangent space](../../../statistical-model.md#statistical-tangent-space). **The tangent set consists of attainable scores; the tangent space also includes their [linear combinations](../../../vector-space.md#linear-combination) and $L^2(P_f)$ limits.**

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $g$ be a [bounded function](../../../function.md#bounded-function) with $P_fg=0$. A [bounded density tilt](../../../statistical-model.md#bounded-density-tilt) realizes this direction:

$$
f_t(u)=f(u)(1+tg(u)),\qquad |t|\|g\|_\infty<1.
$$

These are nonnegative [probability density functions](../../../continuous-probability-distribution.md#probability-density-function), since $\int f_t=1+tP_fg=1$. The uniform [Taylor expansion](../../../calculus.md#taylor-expansion) of the square root gives

$$
\sqrt{f_t}-\sqrt f-\frac t2g\sqrt f
=\sqrt f\,O(t^2g^2).
$$

The squared [L2 norm](../../../real-analysis.md#l2-norm) of this remainder is $O(t^4P_fg^4)=o(t^2)$, since $g$ is bounded. Thus the [statistical path](../../../statistical-model.md#statistical-path) is [differentiable in quadratic mean](../../../statistical-model.md#differentiability-in-quadratic-mean) with [score function](../../../statistical-modelling.md#informant-function) $g$.

Conversely every [score function](../../../statistical-modelling.md#informant-function) is centered by the [mean-zero score identity under quadratic-mean differentiability](../../../statistical-model.md#mean-zero-score-identity-under-quadratic-mean-differentiability). Choosing all these [bounded density tilts](../../../statistical-model.md#bounded-density-tilt) therefore gives the [statistical tangent set](../../../statistical-model.md#statistical-tangent-set)

$$
\boxed{\dot{\mathcal P}_f=\{g:\ g\text{ is bounded and measurable},\ P_fg=0\}.}
$$

This is a valid choice of [statistical tangent set](../../../statistical-model.md#statistical-tangent-set); it does not assert that every possible [score function](../../../statistical-modelling.md#informant-function) in the unrestricted density model is bounded.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Consider any [differentiable-in-quadratic-mean path](../../../statistical-model.md#differentiability-in-quadratic-mean) with [score function](../../../statistical-modelling.md#informant-function) $g$. Put $\delta_t=\sqrt{f_t}-\sqrt f=(t/2)g\sqrt f+r_t$, where $\|r_t\|_2=o(|t|)$. The [quadratic-mean to L1 density derivative](../../../statistical-model.md#quadratic-mean-to-l1-density-derivative) follows from

$$
f_t-f=2\sqrt f\,\delta_t+\delta_t^2
=tfg+2\sqrt f\,r_t+\delta_t^2.
$$

By the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality),

$$
\|f_t-f-tfg\|_{L^1}
\leq2\|r_t\|_2+\|\delta_t\|_2^2=o(|t|).
$$

Since $a$ is a [bounded function](../../../function.md#bounded-function), multiplying this [L1 norm](../../../functional-analysis.md#l1-norm) bound by $\|a\|_\infty$ proves

$$
\frac{\psi(P_{f_t})-\psi(P_f)}t\longrightarrow P_f(ag)
=P_f\bigl((a-P_fa)g\bigr).
$$

The last equality uses $P_fg=0$. The [derivative](../../../calculus.md#derivative) is a [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional) of $g\in L^2(P_f)$, so the required [pathwise differentiability of a statistical functional](../../../statistical-inference.md#pathwise-differentiability-of-a-statistical-functional) holds, in particular relative to the [statistical tangent set](../../../statistical-model.md#statistical-tangent-set) from part (b). **Its [derivative](../../../calculus.md#derivative) is**

$$
\boxed{D\psi_f(g)=P_f[(a-P_fa)g].}
$$

For the explicit [bounded density tilts](../../../statistical-model.md#bounded-density-tilt) in part (b), this [derivative](../../../calculus.md#derivative) is also obtained by direct integration, with no remainder term.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

For a [pathwise differentiable statistical functional](../../../statistical-inference.md#pathwise-differentiability-of-a-statistical-functional), an [influence-function representer](../../../statistical-inference.md#influence-function-representer) is a [mean-zero function](../../../probability-theory.md#mean-zero-function) $\varphi\in L^2(P)$ such that every admissible [score function](../../../statistical-modelling.md#informant-function) $g$ satisfies $D\psi_P(g)=P(\varphi g)$. The [efficient influence function](../../../statistical-inference.md#canonical-gradient), also called the [canonical gradient](../../../statistical-inference.md#canonical-gradient), is the unique such representer in the [statistical tangent space](../../../statistical-model.md#statistical-tangent-space). Equivalently, it is the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) of any representer onto that [statistical tangent space](../../../statistical-model.md#statistical-tangent-space). The [Pythagorean theorem in an inner-product space](../../../linear-algebra.md#pythagorean-theorem-in-an-inner-product-space) shows that it has the smallest squared [L2 norm](../../../real-analysis.md#l2-norm) among all representers.

Here the [statistical tangent space](../../../statistical-model.md#statistical-tangent-space) is all of $L^2_0(P_f)$. To verify the closure explicitly, take $h\in L^2_0(P_f)$, truncate it to $h_m=\max(-m,\min(h,m))$, and set $g_m=h_m-P_fh_m$. Then $g_m$ is bounded and centered, and $g_m\to h$ in $L^2(P_f)$, by [dominated convergence](../../../measure-theory.md#dominated-convergence-theorem) and the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality). Part (c) supplies a representer already in this space. Hence

$$
\boxed{\varphi_f(u)=a(u)-\int_0^1 a(v)f(v)\,dv.}
$$

Its [variance](../../../variance.md) is $P_fa^2-(P_fa)^2$.

**The closure must be taken in the density-weighted space $L^2(P_f)$.** An unweighted reading of $L^2[0,1]$ in the printed hint is false. For example, when $f(u)=2u$, the [function](../../../function.md) $h(u)=u^{-3/4}-8/5$ has $P_fh=0$ and $P_fh^2=36/25$, so bounded centered truncations converge to it in $L^2(P_f)$; nevertheless $h\notin L^2([0,1],du)$. This illustrates [density of bounded centered scores](../../../statistical-model.md#density-of-bounded-centered-scores) and fixes the measure in the closure statement.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

For the [bounded density tilt](../../../statistical-model.md#bounded-density-tilt) $f_t=f(1+tg)$, differentiate the polynomial in $t$:

$$
\left.\frac{d}{dt}\int_0^1 f_t(u)^4\,du\right|_{t=0}
=4\int_0^1 f(u)^4g(u)\,du=P_f(4f^3g).
$$

Since every [score function](../../../statistical-modelling.md#informant-function) is centered, the centered representer is

$$
\boxed{\varphi_f(u)=4\left(f(u)^3-\int_0^1 f(v)^4\,dv\right).}
$$

A bounded baseline $f$ makes this a bounded [mean-zero function](../../../probability-theory.md#mean-zero-function), hence an element of $L^2_0(P_f)$. Thus it is the [efficient influence function](../../../statistical-inference.md#canonical-gradient) for the [density fourth-power functional](../../../statistical-inference.md#density-fourth-power-functional) relative to the regular [bounded density tilts](../../../statistical-model.md#bounded-density-tilt). Its squared [L2 norm](../../../real-analysis.md#l2-norm) is $16\{\int f^7-(\int f^4)^2\}$.

**A bounded baseline alone does not make this functional differentiable along every quadratic-mean differentiable path.** The [derivative](../../../calculus.md#derivative) above is the intended regular-path answer. To see the need for the qualification, let $f_0=1$ and put $b(s)=6s(1-s)$ on $[0,1]$, extended by zero outside. For $0<|t|<1$, define

$$
f_t(u)=1-t^4+t^{-2}b(u/t^6),\qquad 0\leq u\leq1.
$$

Each $f_t$ is a nonnegative continuous [probability density function](../../../continuous-probability-distribution.md#probability-density-function), because its narrow bump has mass $t^4$. Moreover,

$$
\int(\sqrt{f_t}-1)^2\,du\leq\int|f_t-1|\,du\leq2t^4=o(t^2).
$$

It is therefore a [differentiable-in-quadratic-mean path](../../../statistical-model.md#differentiability-in-quadratic-mean) with zero [score function](../../../statistical-modelling.md#informant-function). Yet

$$
\int f_t^4\,du\geq t^{-2}\int_0^1b(s)^4\,ds=\frac{72}{35t^2}\longrightarrow\infty.
$$

The [density fourth-power functional](../../../statistical-inference.md#density-fourth-power-functional) is not even continuous along this [statistical path](../../../statistical-model.md#statistical-path), although every $f_t$ is individually bounded. Consequently no [efficient influence function](../../../statistical-inference.md#canonical-gradient) represents [derivatives](../../../calculus.md#derivative) over the unrestricted class of all such paths.

One sufficient additional condition is a common bound $f_t,f\leq M$ for all small $t$. [Taylor expansion](../../../calculus.md#taylor-expansion) then bounds the fourth-power remainder by $6M^2(f_t-f)^2$, while

$$
\|f_t-f\|_2\leq2\sqrt M\,\|\sqrt{f_t}-\sqrt f\|_2=O(|t|).
$$

Together with the [quadratic-mean to L1 density derivative](../../../statistical-model.md#quadratic-mean-to-l1-density-derivative), this gives $\psi(P_{f_t})-\psi(P_f)=tP_f(\varphi_fg)+o(|t|)$. Under this local bound, or when the chosen [statistical paths](../../../statistical-model.md#statistical-path) are the [bounded density tilts](../../../statistical-model.md#bounded-density-tilt), the boxed [canonical gradient](../../../statistical-inference.md#canonical-gradient) is fully justified. The counterexample is a [spike obstruction to density-power differentiability](../../../statistical-inference.md#spike-obstruction-to-density-power-differentiability).

## 3

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Fix any [estimator](../../../statistical-modelling.md#estimator) $\widehat\eta$ and put $A(x)=d(\widehat\eta(x),f)$, $B(x)=d(\widehat\eta(x),g)$ and $D=d(f,g)$. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) for the [metric](../../../topological-analysis.md#metric) gives $A+B\geq D$. Hence

$$
A^2+B^2\geq\frac{(A+B)^2}{2}\geq\frac{D^2}{2}.
$$

The larger of the two [risk functions](../../../statistical-modelling.md#risk-function) dominates their average. Using nonnegativity to replace both [probability density functions](../../../continuous-probability-distribution.md#probability-density-function) by their minimum,

$$
\begin{aligned}
\sup_{\eta\in\mathcal F}P_\eta d(\widehat\eta,\eta)^2
&\geq\frac12\{P_fA^2+P_gB^2\}\\
&\geq\frac12\int\min(p_f,p_g)(A^2+B^2)\,d\mu\\
&\geq\frac{D^2}{4}\int\min(p_f,p_g)\,d\mu.
\end{aligned}
$$

The right side is independent of the [estimator](../../../statistical-modelling.md#estimator), so taking the infimum proves

$$
\boxed{\inf_{\widehat\eta}\sup_{\eta\in\mathcal F}P_\eta d(\widehat\eta,\eta)^2\geq\frac{d(f,g)^2}{4}\int\min(p_f,p_g)\,d\mu.}
$$

This [metric squared-loss two-point bound](../../../statistical-inference.md#metric-squared-loss-two-point-bound) uses overlap of the observation laws to quantify how hard it is to distinguish the two separated parameters.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Apply the preceding argument to the two product observation laws and the real-valued [estimator](../../../statistical-modelling.md#estimator) $T=\widehat\psi_n$. Alternatively, directly use

$$
(T-\theta)^2+(T-\tau)^2
=2\left(T-\frac{\theta+\tau}{2}\right)^2+\frac{(\theta-\tau)^2}{2}
\geq\frac{(\theta-\tau)^2}{2}.
$$

The average of the two [mean squared errors](../../../statistical-modelling.md#mean-squared-error) is at least $(\theta-\tau)^2/4$ times the overlap of the two joint [probability density functions](../../../continuous-probability-distribution.md#probability-density-function). Their overlap equals

$$
\int\min(p_f^{(n)},p_g^{(n)})\,d\mu^{(n)}
=\frac12\int(p_f^{(n)}+p_g^{(n)}-|p_f^{(n)}-p_g^{(n)}|)\,d\mu^{(n)}
=1-\frac12\|P_f^{(n)}-P_g^{(n)}\|_1.
$$

Taking the infimum over [estimators](../../../statistical-modelling.md#estimator) therefore yields

$$
\boxed{R_n^*\geq\frac{(\theta-\tau)^2}{4}\left(1-\frac12\|P_f^{(n)}-P_g^{(n)}\|_1\right).}
$$

Here $R_n^*$ is the [minimax risk](../../../statistical-modelling.md#minimax-risk) for this functional. The factor $\frac12\|P_f^{(n)}-P_g^{(n)}\|_1$ is the [total variation distance](../../../probability-and-statistics.md#total-variation-distance), so the same [metric squared-loss two-point bound](../../../statistical-inference.md#metric-squared-loss-two-point-bound) applies to a functional even when distinct density parameters have the same functional value.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For each $n\geq1$, choose the continuous [probability density functions](../../../continuous-probability-distribution.md#probability-density-function)

$$
f(u)=1,\qquad g_n(u)=1+\frac{u-1/2}{\sqrt n}.
$$

The second is at least $1/2$ and integrates to one. Their [expected values](../../../probability-theory.md#expected-value) differ by

$$
\psi(g_n)-\psi(f)=\frac1{\sqrt n}\int_0^1u(u-1/2)\,du=\frac1{12\sqrt n}.
$$

Writing $g_n/f=1+\Delta_n$ gives

$$
P_f\Delta_n^2=\frac1n\int_0^1(u-1/2)^2\,du=\frac1{12n}.
$$

The supplied product bound, also obtained from the [chi-squared divergence of product measures](../../../probability-and-statistics.md#chi-squared-divergence-of-product-measures), implies

$$
\|P_f^{(n)}-P_{g_n}^{(n)}\|_1^2
\leq\left(1+\frac1{12n}\right)^n-1
\leq e^{1/12}-1\leq\frac1{11}<1.
$$

For the final elementary estimate, compare the exponential series with the geometric series: $e^x\leq(1-x)^{-1}$ for $0\leq x<1$. Thus the overlap of the product laws is at least $1/2$. Part (b) now gives the explicit [mean-estimation minimax lower bound for continuous densities](../../../statistical-inference.md#mean-estimation-minimax-lower-bound-for-continuous-densities)

$$
\boxed{R_n^*\geq\frac14\cdot\frac1{144n}\cdot\frac12=\frac1{1152n}.}
$$

So **one may take $C=1/1152$, uniformly for all $n\geq1$**. The alternatives are allowed to depend on $n$, because the [minimax risk](../../../statistical-modelling.md#minimax-risk) takes a supremum over all continuous [probability density functions](../../../continuous-probability-distribution.md#probability-density-function) separately at each sample size.

## 4

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Write $e=y-g_\theta(x)$ and $h_\theta(x)=\partial g_\theta(x)/\partial\theta$. Holding the [nuisance parameter](../../../statistical-model.md#nuisance-parameter) $\eta$ fixed, the parametric [score function](../../../statistical-modelling.md#informant-function) is the [derivative](../../../calculus.md#derivative) with respect to $\theta$ of the one-observation [log-likelihood](../../../statistical-modelling.md#log-likelihood). The joint [probability density function](../../../continuous-probability-distribution.md#probability-density-function) is

$$
p_{\theta,\eta}(x,y)=\eta(x)\frac1{\sqrt{2\pi\sigma^2}}\exp\left(-\frac{(y-g_\theta(x))^2}{2\sigma^2}\right).
$$

Because $\partial e/\partial\theta=-h_\theta(x)$, differentiating gives

$$
\boxed{\dot\ell_{\theta,\eta}(x,y)=\frac{h_\theta(x)(y-g_\theta(x))}{\sigma^2}=\frac{h_\theta(x)e}{\sigma^2}.}
$$

For instance $E_\eta h_\theta(X)^2<\infty$ ensures a [square-integrable](../../../measure-theory.md#square-integrable-function) [score function](../../../statistical-modelling.md#informant-function). Its [expected value](../../../probability-theory.md#expected-value) is zero by [independence](../../../random-variable.md#independent-random-variables) and the centered [normal distribution](../../../probability-theory.md#normal-distribution) of the error. This is the [Gaussian regression score](../../../statistical-modelling.md#gaussian-regression-score).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Vary only the [probability density function](../../../continuous-probability-distribution.md#probability-density-function) of $X$, using $\eta_t=\eta(1+tb)$ with bounded $b$ and $E_\eta b(X)=0$. The nuisance [score function](../../../statistical-modelling.md#informant-function) is $b(X)$, giving the [statistical tangent set](../../../statistical-model.md#statistical-tangent-set)

$$
\{b(X):\ b\text{ bounded and measurable},\ E_\eta b(X)=0\}.
$$

Its closed linear span is the [nuisance tangent space](../../../statistical-inference.md#nuisance-tangent-space) of all centered $L^2(\eta)$ [functions](../../../function.md) of $X$, by [density of bounded centered scores](../../../statistical-model.md#density-of-bounded-centered-scores).

The [conditional expectation](../../../measure-theory.md#conditional-expectation) of the parametric [score function](../../../statistical-modelling.md#informant-function) given $X$ is zero:

$$
E\left[\frac{h_\theta(X)\varepsilon}{\sigma^2}\,\middle|\,X\right]=0.
$$

It is therefore orthogonal to this [nuisance tangent space](../../../statistical-inference.md#nuisance-tangent-space). Its [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) onto that space vanishes, so the [efficient score](../../../statistical-inference.md#efficient-score) is unchanged. By [independence](../../../random-variable.md#independent-random-variables) and $E\varepsilon^2=\sigma^2$,

$$
\boxed{\widetilde\ell_{\theta,\eta}=\frac{h_\theta(X)\varepsilon}{\sigma^2},\qquad
\widetilde I_{\theta,\eta}=\frac{E_\eta h_\theta(X)^2}{\sigma^2}.}
$$

These equal the parametric [score function](../../../statistical-modelling.md#informant-function) and [Fisher information](../../../statistical-modelling.md#fisher-information-matrix) when $\eta$ is known. **There is no loss of information from the unknown covariate density.** This is [adaptivity to an unknown covariate distribution](../../../statistical-inference.md#adaptivity-to-an-unknown-covariate-distribution); it follows from score orthogonality, without having to estimate the [nuisance parameter](../../../statistical-model.md#nuisance-parameter).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Now $p_{\theta,\eta}(x,y)=v(x)f(y-g_\theta(x))$. With $h_\theta=\partial_\theta g_\theta$ and the [location score](../../../statistical-model.md#location-score) $\rho(e)=-f'(e)/f(e)$, differentiation of the [log-likelihood](../../../statistical-modelling.md#log-likelihood) gives

$$
\boxed{\dot\ell_{\theta,\eta}(x,y)=-h_\theta(x)\frac{f'(e)}{f(e)}=h_\theta(x)\rho(e).}
$$

Take the usual regularity conditions $h_\theta\in L^2(v)$ and $\rho\in L^2(f)$ so that this [score function](../../../statistical-modelling.md#informant-function) belongs to [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space).

For the specified nuisance [statistical path](../../../statistical-model.md#statistical-path), differentiating $\log(1+t\gamma(e))$ at zero gives the [score function](../../../statistical-modelling.md#informant-function) $\gamma(e)$. Normalization requires $E_f\gamma=0$. There is a second constraint: the [statistical path](../../../statistical-model.md#statistical-path) must preserve the model's zero error [expected value](../../../probability-theory.md#expected-value). Thus

$$
0=\int e f(e)(1+t\gamma(e))\,de=t\int e\gamma(e)f(e)\,de,
\qquad\boxed{E_f[\varepsilon\gamma(\varepsilon)]=0.}
$$

This constraint follows from being a path through the model, rather than from normalization alone. For a centered symmetric [logistic distribution](../../../statistical-modelling.md#logistic-distribution), for example, $\gamma(e)=\tanh(e)$ is bounded and has zero [expected value](../../../probability-theory.md#expected-value), but $E[\varepsilon\tanh(\varepsilon)]>0$; it would not preserve the mean.

For any $\psi\in L^2(v)$, [independence](../../../random-variable.md#independent-random-variables) implies

$$
E[\gamma(\varepsilon)\varepsilon\psi(X)]
=E_f[\varepsilon\gamma(\varepsilon)]E_v\psi(X)=\boxed{0}.
$$

All these products are integrable by the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality), since $\varepsilon\psi(X)$ is [square-integrable](../../../measure-theory.md#square-integrable-function). Thus every such error-density [score function](../../../statistical-modelling.md#informant-function) is orthogonal to every $e\psi(x)$. Covariate-density nuisance [score functions](../../../statistical-modelling.md#informant-function) $b(X)$ are also orthogonal to these [functions](../../../function.md), since $E\varepsilon=0$. This is the [mean-preserving error tangent space](../../../statistical-inference.md#mean-preserving-error-tangent-space) orthogonality used in the final calculation.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

First use the additional admitted form of the [efficient score](../../../statistical-inference.md#efficient-score). Write $\widetilde\ell=e\zeta(X)$ and let $\tau^2=E_f\varepsilon^2>0$. The difference $\dot\ell-\widetilde\ell$ is the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) onto the [nuisance tangent space](../../../statistical-inference.md#nuisance-tangent-space). Part (c) makes every $e\psi(X)$ orthogonal to that space. Therefore, for all $\psi\in L^2(v)$,

$$
0=E[(h_\theta(X)\rho(\varepsilon)-\varepsilon\zeta(X))\varepsilon\psi(X)]
=E_v\bigl[\{h_\theta E_f(\varepsilon\rho)-\tau^2\zeta\}\psi\bigr].
$$

The [function](../../../function.md) in braces belongs to [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space); choosing it as $\psi$ shows it vanishes $v$-almost everywhere. Hence the required conditional deduction is

$$
\boxed{\widetilde\ell_{\theta,\eta}(x,e)
=-e\,\frac{\int s f'(s)\,ds}{\int s^2f(s)\,ds}\,h_\theta(x).}
$$

Under the regular tail condition $s f(s)\to0$ at both infinities, [integration by parts](../../../calculus.md#integration-by-parts) gives $\int s f'(s)\,ds=-1$, and the formula becomes $e h_\theta(x)/\tau^2$. This also confirms the sign.

**The admitted product form is an extra restriction; it does not follow for every independent-error regression model.** To locate the restriction precisely, suppose the error-density nuisance [statistical paths](../../../statistical-model.md#statistical-path) preserve both normalization and mean to first order. Their closed [mean-preserving error tangent space](../../../statistical-inference.md#mean-preserving-error-tangent-space) is $\{\gamma:E_f\gamma=E_f(\varepsilon\gamma)=0\}$. The full [nuisance tangent space](../../../statistical-inference.md#nuisance-tangent-space) is the orthogonal sum of this space and the centered [functions](../../../function.md) of $X$.

For completeness, bounded [functions](../../../function.md) satisfying the two constraints are dense in the error space. Truncate an arbitrary element, subtract its [expected value](../../../probability-theory.md#expected-value), and then subtract a multiple of a fixed bounded centered [function](../../../function.md) $q$ with $E_f(\varepsilon q)\ne0$. Such a $q$ exists by truncating $\varepsilon$, since $\tau^2>0$. The correction coefficients tend to zero by the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality), so the corrected truncations converge in [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space).

Let $m=E_vh_\theta(X)$. With $E_f\rho=0$ and $E_f(\varepsilon\rho)=1$, the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) of $h_\theta(X)\rho(\varepsilon)$ onto the error nuisance space is $m\{\rho(\varepsilon)-\varepsilon/\tau^2\}$; its projection onto the covariate nuisance space is zero. Thus the general [efficient score in independent-error regression](../../../statistical-inference.md#efficient-score-in-independent-error-regression) is

$$
\boxed{\widetilde\ell=(h_\theta(X)-m)\rho(\varepsilon)+\frac{m\varepsilon}{\tau^2},
\qquad
\widetilde I=\operatorname{Var}_v(h_\theta)E_f\rho^2+\frac{m^2}{\tau^2}.}
$$

The [orthogonality](../../../linear-algebra.md#orthogonal-vectors) of the two terms gives the displayed [efficient information](../../../statistical-inference.md#efficient-information). For a [normal distribution](../../../probability-theory.md#normal-distribution) of the error, $\rho(e)=e/\tau^2$, so this reduces to the admitted formula. It also does so when $h_\theta$ is constant.

A concrete counterexample to the generality of the admission is $g_\theta(x)=\theta x$, with $X$ uniform on $[-1,1]$ and independent standard [logistic distribution](../../../statistical-modelling.md#logistic-distribution) error. Here $m=0$ and $\rho(e)=\tanh(e/2)$, so the actual [efficient score](../../../statistical-inference.md#efficient-score) is $x\tanh(e/2)$. It cannot equal $e\zeta(x)$ because $\tanh(e/2)/e$ is not constant. This [score function](../../../statistical-modelling.md#informant-function) is already orthogonal to every nuisance [score function](../../../statistical-modelling.md#informant-function): its factor $X$ is centered against error-only directions, and its factor $\rho(\varepsilon)$ is centered against covariate-only directions. **The requested formula is valid under its stated additional admission, with the general independent-error formula above explaining its limits.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
