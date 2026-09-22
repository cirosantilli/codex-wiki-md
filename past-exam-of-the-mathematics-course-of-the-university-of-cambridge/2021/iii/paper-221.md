# Paper 221

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_221.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_221.pdf)

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
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)
    - [iii](#4/b/iii)
      - [Solution](#4/b/iii/solution)
  - [c](#4/c)
    - [i](#4/c/i)
      - [Solution](#4/c/i/solution)
    - [ii](#4/c/ii)
      - [Solution](#4/c/ii/solution)
    - [iii](#4/c/iii)
      - [Solution](#4/c/iii/solution)

## 1

↑ **Parent:** [Paper 221](paper-221.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

[Causal identification](../../../causal-inference.md#causal-identification) means that $\mathbb E[Y(a_1,a_2)]$ is uniquely determined by the observed joint distribution of $(A_1,X,A_2,Y)$ under the causal assumptions. Equivalently, it admits an identifying formula containing only observed-data probabilities and conditional expectations.

The [G-computation](../../../causal-inference.md#g-computation) formula for this two-stage treatment is

$$
\boxed{
\mathbb E[Y(a_1,a_2)]
=\sum_x \mathbb E[Y\mid A_1=a_1,X=x,A_2=a_2]
\mathbb P(X=x\mid A_1=a_1)}.
$$

The first factor is the observed mean outcome after the specified treatment history and intermediate value; the second averages over the intermediate-variable distribution generated after the first treatment.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

In the second [causal directed acyclic graph](../../../causal-inference.md#causal-directed-acyclic-graph), $Y(a_1,a_2)$ depends on $U_2$ but not on $U_1$, whereas $A_1$ depends on $U_1$ and the two latent roots are independent. Hence

$$
Y(a_1,a_2)\mathrel\perp A_1.
$$

Although conditioning on $X$ conveys information about $U_2$, the assignment $A_2$ uses only $(A_1,X)$ and fresh randomization, so

$$
Y(a_1,a_2)\mathrel\perp A_2\mid A_1,X.
$$

These are the two [sequential exchangeability](../../../causal-inference.md#sequential-exchangeability) conditions. Using them successively, together with [consistency of potential outcomes](../../../causal-inference.md#consistency-in-causal-inference), gives

$$
\begin{aligned}
\mathbb E[Y(a_1,a_2)]
&=\sum_x\mathbb E[Y(a_1,a_2)\mid A_1=a_1,X=x]
\mathbb P(X=x\mid A_1=a_1)\\
&=\sum_x\mathbb E[Y\mid A_1=a_1,X=x,A_2=a_2]
\mathbb P(X=x\mid A_1=a_1),
\end{aligned}
$$

which is the formula from part a.

Adding $X\to Y$ invalidates the argument in general. The latent variable $U_1$ confounds $A_1$ and $X$, so $\mathbb P(X\mid A_1=a_1)$ need not equal the distribution of $X(a_1)$. When $X$ directly affects $Y$, that discrepancy no longer cancels after summing over $x$. The same observed distribution can then correspond to different intervention means, so the displayed formula need not identify the effect.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Write

$$
H_t=(A_1,X_1,\ldots,A_{t-1},X_{t-1})
$$

for the observed history just before $A_t$. A sufficient condition is [sequential exchangeability](../../../causal-inference.md#sequential-exchangeability)

$$
Y(a_1,\ldots,a_T)\mathrel\perp A_t\mid H_t,
\qquad t=1,\ldots,T,
$$

for every treatment regime, together with [consistency of potential outcomes](../../../causal-inference.md#consistency-in-causal-inference) and [positivity in causal inference](../../../causal-inference.md#positivity-assumption). Repeated conditioning then gives the longitudinal [G-formula](../../../causal-inference.md#g-computation)

$$
\boxed{
\mathbb E[Y(\bar a_T)]
=\sum_{x_1,\ldots,x_{T-1}}
\mathbb E[X_T\mid \bar A_T=\bar a_T,\bar X_{T-1}=\bar x_{T-1}]
\prod_{t=1}^{T-1}
\mathbb P(X_t=x_t\mid\bar A_t=\bar a_t,\bar X_{t-1}=\bar x_{t-1})}.
$$

Graphically, it is enough that each $A_t$ be [D-separated](../../../combinatorics.md#d-separation) from the final counterfactual under the specified regime after conditioning on its observed past. The two independences used in part b are precisely the $T=2$ instance.

## 2

↑ **Parent:** [Paper 221](paper-221.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Conditionally on $X$, a valid [instrumental variable](../../../causal-inference.md#instrumental-variable) $Z$ must satisfy three core conditions.

- [Instrument relevance](../../../causal-inference.md#instrument-relevance): $Z$ changes the conditional distribution of $A$, for example $\operatorname{Cov}(Z,A\mid X)\ne0$ on a set of positive probability.
- [Instrumental-variable independence](../../../causal-inference.md#instrumental-variable-independence): $Z$ is independent of latent outcome causes and the relevant [potential outcomes](../../../causal-inference.md#potential-outcome), for example $Z\mathrel\perp\{Y(a):a\}\mid X$.
- The [exclusion restriction](../../../causal-inference.md#exclusion-restriction): $Z$ affects $Y$ only through $A$, written $Y(a,z)=Y(a)$.

Together with [consistency of potential outcomes](../../../causal-inference.md#consistency-in-causal-inference) and [positivity in causal inference](../../../causal-inference.md#positivity-assumption), these assumptions make variation in $A$ induced by $Z$ causally interpretable. In the displayed graph, relevance is the edge $Z\to A$, independence is the absence of a path from $Z$ to $U$ after conditioning on $X$, and exclusion is the absence of a direct $Z\to Y$ edge.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Retaining the estimator exactly as printed, define the probability limit

$$
c=\frac{\mathbb E[ZX]}{\mathbb E[Z^2]},
\qquad W=Z-cX.
$$

The empirical equations are linear in $(\beta,\alpha)$. Their coefficient matrix converges to

$$
M=
\begin{pmatrix}
\mathbb E[AW]&\mathbb E[XW]\\
\mathbb E[AX]&\mathbb E[X^2]
\end{pmatrix}.
$$

Therefore a sufficient condition, requiring neither parametric assumption, is

$$
0<\mathbb E[Z^2]<\infty,
\qquad
\det M
=\mathbb E[AW]\mathbb E[X^2]
-\mathbb E[XW]\mathbb E[AX]\ne0,
$$

with finite moments sufficient for the [weak law of large numbers](../../../convergence-of-random-variables.md#weak-law-of-large-numbers). The empirical determinant then converges to a nonzero number, so the two linear equations have a unique solution with probability tending to one.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The [homogeneous treatment effect](../../../causal-inference.md#homogeneous-treatment-effect) and consistency imply

$$
Y-\beta_0A=Y(0)=:R.
$$

Instrument validity gives $Z\mathrel\perp R\mid X$.

If Assumption 1 holds, put $V=R-\alpha_0X$. Then $\mathbb E[V\mid X]=0$, so conditional instrument independence gives

$$
\mathbb E[VZ]=0,
\qquad
\mathbb E[VX]=0.
$$

Consequently both population estimating equations vanish at $(\beta_0,\alpha_0)$ for any probability limit of $\widehat\gamma$.

If Assumption 2 holds, choose the linear-projection coefficient

$$
\alpha_*=\frac{\mathbb E[RX]}{\mathbb E[X^2]}.
$$

Then $\mathbb E[(R-\alpha_*X)X]=0$, while

$$
\begin{aligned}
\mathbb E[(R-\alpha_*X)(Z-cX)]
&=\mathbb E[(R-\alpha_*X)\{Z-\mathbb E[Z\mid X]\}]\\
&\quad+(\gamma_0-c)\mathbb E[(R-\alpha_*X)X]=0.
\end{aligned}
$$

The first term is zero by conditional instrument independence and the second by the definition of $\alpha_*$. Thus $(\beta_0,\alpha_*)$ solves the population equations. Under the nonsingularity condition from part b, the root is unique, so standard [estimating equation](../../../statistical-inference.md#estimating-equation) consistency proves

$$
\widehat\beta\xrightarrow{p}\beta_0
$$

whenever either Assumption 1 or Assumption 2 holds. This is [double robustness](../../../probability-and-statistics.md#double-robustness).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Let

$$
d=\mathbb E[X^2],\qquad q=\mathbb E[XZ],\qquad
R_0=Z-\gamma_0X.
$$

Assumption 2 implies $\gamma_0=q/d$. Although the printed $\widehat\gamma$ need not converge to $\gamma_0$, its first-order effect vanishes because $\mathbb E[VX]=0$. Inverting the $2\times2$ Jacobian of the remaining [estimating equations](../../../statistical-inference.md#estimating-equation) gives the influence function

$$
\operatorname{IF}_\beta
=\frac{V\{dW-\mathbb E[XW]X\}}
{d\mathbb E[AW]-\mathbb E[XW]\mathbb E[AX]}
=\frac{VR_0}{\mathbb E[AR_0]}.
$$

The first-stage condition yields

$$
\mathbb E[AR_0]
=\mathbb E[\mathbb E[A\mid X,Z]R_0]
=\lambda\mathbb E[R_0^2].
$$

Hence the asymptotic variance of $\sqrt n(\widehat\beta-\beta_0)$ is the [sandwich](../../../statistical-inference.md#sandwich-covariance-matrix) expression

$$
\boxed{
\mathcal V_\beta
=\frac{\mathbb E[V^2R_0^2]}
{\lambda^2\{\mathbb E[R_0^2]\}^2}}.
$$

There is a defect in the printed assumptions: $\operatorname{Var}(V\mid A,X)=\sigma^2$ alone does not determine $\mathbb E[V^2R_0^2]$, because $R_0$ depends on $Z$ and $V$ can have a nonzero conditional mean given $(A,X)$ under unmeasured confounding. Under the standard intended strengthening $\mathbb E[V^2\mid X,Z]=\sigma^2$, the formula simplifies to

$$
\boxed{
\mathcal V_\beta=\frac{\sigma^2}{\lambda^2\mathbb E[(Z-\gamma_0X)^2]}}.
$$

The asymptotic variance of $\widehat\beta$ itself is $\mathcal V_\beta/n$.

## 3

↑ **Parent:** [Paper 221](paper-221.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A distribution is [faithful](../../../causal-inference.md#faithfulness-of-a-directed-acyclic-graph) to a [Directed acyclic graph](../../../combinatorics.md#directed-acyclic-graph) $G$ when every [conditional independence](../../../random-variable.md#conditional-independence) in the distribution is implied by [D-separation](../../../combinatorics.md#d-separation) in $G$. Together with the graphical Markov property, faithfulness makes conditional independence equivalent to D-separation and rules out independences caused only by exact parameter cancellation.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

A [backdoor path](../../../causal-inference.md#backdoor-path) from $A$ to $Y$ is a path whose first edge has an arrowhead at $A$. The set $X_I$ satisfies the [backdoor criterion](../../../causal-inference.md#backdoor-adjustment-set) when it contains no descendant of $A$ and blocks every backdoor path from $A$ to $Y$. Under this criterion, consistency, and positivity,

$$
Y(a)\mathrel\perp A\mid X_I,
$$

so adjustment for $X_I$ identifies the intervention mean.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Definition 1 satisfies Property 1 but not Property 2. Let $S_1$ contain every non-descendant that blocks some backdoor path. Every backdoor path begins $A\leftarrow P$ for a parent $P$ of $A$; whenever that path can transmit confounding, $P\in S_1$. Conditioning on $S_1$ therefore blocks every such path at its first nonendpoint vertex, so $S_1$ is sufficient.

For failure of Property 2, consider the faithful graph with arrows

$$
C\to A,qquad C\to Y,qquad C\to X_i\to Y.
$$

The variable $X_i$ blocks the backdoor path $A\leftarrow C\to X_i\to Y$, so Definition 1 calls it a confounder. Every sufficient set containing $X_i$ must nevertheless contain $C$ to block $A\leftarrow C\to Y$. Once $C$ is included, deleting $X_i$ leaves a sufficient set. Thus $X_i$ can never be essential as Property 2 demands.

Definition 2 satisfies Property 2 but not Property 1. If $X_i$ belongs to every [minimal sufficient adjustment set](../../../causal-inference.md#minimal-sufficient-adjustment-set), choose one such set $I$ and put $J=I\setminus\{i\}$. By minimality, $J\cup\{i\}$ is sufficient and $J$ is not, proving Property 2.

For failure of Property 1, use the faithful chain-shaped backdoor path

$$
A\leftarrow C_1\to C_2\to Y.
$$

Both $\{C_1\}$ and $\{C_2\}$ are minimal sufficient adjustment sets. No variable belongs to every minimal sufficient set, so Definition 2 labels no variable a confounder, but the empty set is not sufficient.

Definition 3 satisfies Property 1 but not Property 2. Under faithfulness, its associational criterion contains enough non-descendants to block every open backdoor path. Indeed, if such a path remained open, its first unconditioned parent of $A$ would be D-connected to $A$ and, after a suitable conditioning set, to $Y$ given $A$; faithfulness would place that parent in the Definition 3 set, a contradiction. Thus adjusting for all variables selected by Definition 3 is sufficient.

For failure of Property 2, consider

$$
Z\to A\leftarrow U\to Y,qquad A\to Y,
$$

with both $Z$ and $U$ observed and a faithful distribution. The [instrumental variable](../../../causal-inference.md#instrumental-variable) $Z$ is associated with $A$. Conditioning on the [collider](../../../combinatorics.md#collider) $A$ opens $Z\to A\leftarrow U\to Y$, so $Z$ is associated with $Y$ given $A$ and Definition 3 calls it a confounder. Any sufficient set containing $Z$ must also contain $U$ to block $A\leftarrow U\to Y$, but $\{U\}$ is already sufficient. Hence removing $Z$ never destroys sufficiency, violating Property 2.

## 4

↑ **Parent:** [Paper 221](paper-221.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Restricting to pupils who already attended a Catholic middle school improves [covariate balance](../../../causal-inference.md#covariate-balance): the treatment-group differences in family income, urban residence, and prior mathematics score are all much smaller. This makes severe extrapolation and measured [confounding](../../../causal-inference.md#confounding) less prominent.

The restriction reduces the sample from $11{,}839$ to $1{,}006$, so estimates are less precise. It also changes the target population to Catholic-middle-school pupils, reducing [external validity](../../../causal-inference.md#external-validity) for all United States pupils.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

In the full sample, covariate adjustment moves the estimated coefficient from $0.73$ to $0.32$, a large change consistent with substantial measured [confounding](../../../causal-inference.md#confounding). In the Catholic-middle-school subsample the estimates remain between $0.48$ and $0.60$, supporting the claim that restriction has already improved comparability. The cost is visible in the standard errors, which rise from about $0.08$--$0.09$ to $0.13$--$0.15$ despite similar coefficient magnitudes.

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

A sufficient causal condition is [conditional exchangeability](../../../causal-inference.md#conditional-exchangeability)

$$
\{Y(0),Y(1)\}\mathrel\perp A\mid X,
$$

together with [consistency of potential outcomes](../../../causal-inference.md#consistency-in-causal-inference) and [positivity in causal inference](../../../causal-inference.md#positivity-assumption). For the ordinary-least-squares coefficient itself to equal one common causal effect, also require the correctly specified additive conditional-mean model

$$
\mathbb E[Y(a)\mid X]=\theta_0+\theta^TX+\beta a.
$$

Then $\beta$ is the [homogeneous treatment effect](../../../causal-inference.md#homogeneous-treatment-effect), and the adjusted coefficient consistently estimates both conditional effects and the [average treatment effect](../../../causal-inference.md#average-treatment-effect) in the analyzed population.

<h4 id="4/b/iii">iii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/b/iii)

Let $e(x)=\mathbb P(A=1\mid X=x)$ and let $\widehat e$ be a consistent estimate. The [inverse-probability-weighted estimator of the average treatment effect](../../../causal-inference.md#inverse-probability-weighted-estimator-of-the-average-treatment-effect) is

$$
\boxed{
\widehat\tau_{\rm IPW}
=\frac1n\sum_{i=1}^n\left\{
\frac{A_iY_i}{\widehat e(X_i)}-
\frac{(1-A_i)Y_i}{1-\widehat e(X_i)}
\right\}}.
$$

Under the exchangeability, consistency, and positivity conditions in part ii, and consistent estimation of the [propensity score](../../../causal-inference.md#propensity-score), its probability limit is

$$
\mathbb E[Y(1)]-\mathbb E[Y(0)],
$$

so it consistently estimates the [average treatment effect](../../../causal-inference.md#average-treatment-effect). It does not require the additive outcome-regression model used to interpret the ordinary-least-squares coefficient.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/i">i</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#4/c/i)

In the [bivariate probit model for endogenous treatment](../../../causal-inference.md#bivariate-probit-model-for-endogenous-treatment), $U$ affects treatment through its threshold equation and $V$ affects the outcome through its threshold equation. When $\rho\ne0$, the two disturbances are dependent, so treatment status carries information about the latent outcome disturbance even after conditioning on $X$. Consequently

$$
Y(a)\not\!\perp A\mid X
$$

in general, and the [no unmeasured confounding assumption](../../../causal-inference.md#conditional-exchangeability) fails.

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/c/ii)

Fix $\rho$. For an observation with covariates $x$, put

$$
u=-x^T\alpha,
\qquad
v_a=-a\beta-x^T\gamma,
$$

and let $\Phi$ be the standard-normal distribution function. The four conditional cell probabilities are

$$
\begin{aligned}
p_{00}(x)&=F_\rho(u,v_0),\\
p_{01}(x)&=\Phi(u)-F_\rho(u,v_0),\\
p_{10}(x)&=\Phi(v_1)-F_\rho(u,v_1),\\
p_{11}(x)&=1-\Phi(u)-\Phi(v_1)+F_\rho(u,v_1),
\end{aligned}
$$

where the first index is $A$ and the second is $Y$.

Define $(\widehat\alpha_\rho,\widehat\beta_\rho,\widehat\gamma_\rho)$ as any maximizer of the [log likelihood](../../../statistical-modelling.md#maximum-likelihood-estimation)

$$
\sum_{i=1}^n\sum_{a,y\in\{0,1\}}
\mathbf1_{\{A_i=a,Y_i=y\}}\log p_{ay}(X_i).
$$

Then $\widehat\beta_\rho$ is the requested estimator for the fixed sensitivity value $\rho$.

<h4 id="4/c/iii">iii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/c/iii)

The correlation $\rho$ measures dependence between two normalized latent disturbances; it is not a scale-free measure of the strength of one physical [confounder](../../../causal-inference.md#confounder). Different latent-variable constructions can induce the same $\rho$ while producing different treatment-outcome confounding, and the same omitted cause can produce different $\rho$ after changing thresholds or disturbance scales. Moreover, re-estimating $(\alpha,\beta,\gamma)$ at each value of $\rho$ changes the entire latent model, so the fitted models do not represent one fixed data-generating mechanism with only its confounder strength varied. At $\rho=\pm1$ the [bivariate normal distribution](../../../probability-and-statistics.md#bivariate-normal-distribution) is singular as well. Varying $\rho$ is a model-based sensitivity analysis, but interpreting the interval $[-1,1]$ as an ordered range of strengths of a single unmeasured confounder is therefore logically unjustified.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
