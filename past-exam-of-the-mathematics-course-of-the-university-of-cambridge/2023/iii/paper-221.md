# Paper 221

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_221.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_221.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)

## 1

↑ **Parent:** [Paper 221](paper-221.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

A path in a [causal directed acyclic graph](../../../causal-inference.md#causal-directed-acyclic-graph) is active given a conditioning set $K$ when every noncollider on the path is outside $K$ and every collider has itself or a descendant in $K$. Two vertex sets are [d-separated](../../../combinatorics.md#d-separation) by $K$ when no path between them is active given $K$. The [global Markov property of a directed acyclic graph](../../../combinatorics.md#global-markov-property-of-a-directed-acyclic-graph) then turns d-separation into conditional independence.

In the displayed graph, the edges are

$$
X_1\to X_2,
\quad X_1\to X_3,
\quad X_2\to X_3,
\quad X_3\to X_4,
\quad U\to X_2,
\quad U\to X_4.
$$

Every observed pair except $(X_1,X_4)$ and $(X_2,X_4)$ is joined by a direct edge, which remains active under conditioning on any other observed variables. The pair $(X_2,X_4)$ is always joined by the fork $X_2\leftarrow U\to X_4$, because the unobserved noncollider $U$ cannot be conditioned on.

For $(X_1,X_4)$, if $X_3$ is not conditioned on, $X_1\to X_3\to X_4$ is active. If $X_3$ is conditioned on, the path

$$
X_1\to X_2\leftarrow U\to X_4
$$

becomes active because its collider $X_2$ has conditioned descendant $X_3$; conditioning on $X_2$ itself also opens it. Thus every observed pair is d-connected given every subset of the other observed variables. Any conditional independence between two nonempty observed subvectors would imply one between each selected pair, so the graph entails none.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The [directed acyclic graph factorization](../../../causal-inference.md#directed-acyclic-graph-factorization) is

$$
p(x_1,u,x_2,x_3,x_4)
=p(x_1)p(u)p(x_2\mid x_1,u)
p(x_3\mid x_1,x_2)p(x_4\mid x_3,u).
$$

The graph gives $U\perp X_1$ and $U\perp X_3\mid(X_1,X_2)$. Therefore [Bayes' theorem](../../../probability-theory.md#bayes-theorem) gives

$$
p(u\mid x_1,x_2,x_3)
=p(u\mid x_1,x_2)
=\frac{p(u)p(x_2\mid x_1,u)}{p(x_2\mid x_1)}.
$$

Consequently

$$
\begin{aligned}
&\sum_{x_2}p(x_4\mid x_1,x_2,x_3)p(x_2\mid x_1)\\
&=\sum_{x_2,u}p(x_4\mid x_3,u)p(u)p(x_2\mid x_1,u)\\
&=\sum_up(x_4\mid x_3,u)p(u),
\end{aligned}
$$

which contains no $x_1$. This observed equality is a [Verma constraint](../../../causal-inference.md#verma-constraint): it is implied by the latent-variable causal graph even though it is not a conditional independence.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Write

$$
m(x_1,x_2,x_3)=\mathbb E[X_4\mid x_1,x_2,x_3].
$$

Since $X_1$ has no parents, its total effect has no [backdoor path](../../../causal-inference.md#backdoor-path), and

$$
\tau_1
=\mathbb E[X_4\mid X_1=1]
-\mathbb E[X_4\mid X_1=0].
$$

For $X_2$, $X_3$ intercepts every directed path to $X_4$. Conditional on $X_1$, there is no unblocked backdoor path from $X_2$ to $X_3$, and $(X_1,X_2)$ blocks every backdoor path from $X_3$ to $X_4$. The [conditional front-door adjustment](../../../causal-inference.md#conditional-front-door-adjustment) therefore gives

$$
\mu_2(x)=
\sum_{x_1,x_3}p(x_1)p(x_3\mid x_1,x)
\sum_{x_2'}m(x_1,x_2',x_3)p(x_2'\mid x_1),
$$

and

$$
\tau_2=\mu_2(1)-\mu_2(0).
$$

Part ii shows that the inner sum, after also averaging $X_4$, does not actually depend on $x_1$.

For $X_3$, $(X_1,X_2)$ is a sufficient [backdoor adjustment set](../../../causal-inference.md#backdoor-adjustment-set). Hence

$$
\mu_3(x)=
\sum_{x_1,x_2}m(x_1,x_2,x)
p(x_2\mid x_1)p(x_1),
\qquad
\tau_3=\mu_3(1)-\mu_3(0).
$$

These three formulas identify the requested [average treatment effects](../../../causal-inference.md#average-treatment-effect) from the observed joint distribution.

## 2

↑ **Parent:** [Paper 221](paper-221.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

The [no unmeasured confounding assumption](../../../causal-inference.md#conditional-exchangeability) is the conditional exchangeability statement

$$
(Y(0),Y(1))\perp A\mid X.
$$

Also assume [consistency of potential outcomes](../../../causal-inference.md#consistency-in-causal-inference), no interference between units, and [positivity in causal inference](../../../causal-inference.md#positivity-assumption), in particular $\mathbb P(A=0\mid X)>0$ on the covariate support of treated units. Then

$$
\begin{aligned}
\mathbb E[Y(0)\mid A=1]
&=\mathbb E\{\mathbb E[Y(0)\mid X,A=1]\mid A=1\}\\
&=\mathbb E\{\mathbb E[Y(0)\mid X,A=0]\mid A=1\}\\
&=\mathbb E\{\mu(X)\mid A=1\}.
\end{aligned}
$$

The first treated potential outcome equals the observed treated mean by consistency. Moreover,

$$
\mathbb E\{\mu(X)\mid A=1\}
=\frac{\mathbb E[A\mu(X)]}{\mathbb P(A=1)}
=\frac{\mathbb E[\pi(X)\mu(X)]}{\mathbb E[\pi(X)]}.
$$

Subtracting proves the displayed identification formula for the [average treatment effect on the treated](../../../causal-inference.md#average-treatment-effect-on-the-treated).

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

For discrete $X$,

$$
\beta=\sum_xp(x)\pi(x)\mu(x).
$$

Perturbing the marginal mass $p(x)$ contributes $\pi(X)\mu(X)-\beta$. Perturbing $\pi(x)=\mathbb E[A\mid X=x]$ contributes

$$
\mu(X)\{A-\pi(X)\}.
$$

Their sum is $A\mu(X)-\beta$. Finally, the [influence function](../../../statistical-inference.md#influence-function) of

$$
\mu(x)=\mathbb E[Y\mid A=0,X=x]
$$

is

$$
\frac{\mathbf1_{\{A=0,X=x\}}}{p(x)\{1-\pi(x)\}}
\{Y-\mu(x)\}.
$$

Multiplication by the derivative $p(x)\pi(x)$ of $\beta$ with respect to $\mu(x)$ and summation over $x$ gives

$$
(1-A)\frac{\pi(X)}{1-\pi(X)}\{Y-\mu(X)\}.
$$

Adding the three contributions yields the claimed mean-zero [influence curve](../../../statistical-inference.md#influence-function)

$$
\boxed{(1-A)\frac{\pi(X)}{1-\pi(X)}\{Y-\mu(X)\}
+A\mu(X)-\beta.}
$$

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Estimate the [propensity score](../../../causal-inference.md#propensity-score) $\pi$ and the untreated outcome regression $\mu$, preferably with [cross-fitting](../../../probability-and-statistics.md#cross-fitting) when flexible methods are used, and set

$$
\widehat\beta
=\frac1n\sum_{i=1}^n\left[
(1-A_i)\frac{\widehat\pi(X_i)}{1-\widehat\pi(X_i)}
\{Y_i-\widehat\mu(X_i)\}
+A_i\widehat\mu(X_i)
\right].
$$

With $n_1=\sum_iA_i$, the resulting [one-step estimator](../../../statistical-inference.md#one-step-estimator) of the ATT is

$$
\widehat\tau_{\mathrm{ATT}}
=\frac1{n_1}\sum_iA_iY_i-\frac{\widehat\beta}{n_1/n}.
$$

Equivalently,

$$
\widehat\tau_{\mathrm{ATT}}
=\frac1{n_1}\sum_i\left[
A_i\{Y_i-\widehat\mu(X_i)\}
-(1-A_i)\frac{\widehat\pi(X_i)}{1-\widehat\pi(X_i)}
\{Y_i-\widehat\mu(X_i)\}
\right].
$$

This is an [augmented inverse-probability-weighted estimator](../../../probability-and-statistics.md#augmented-inverse-probability-weighted-estimator); it is consistent when either the propensity model or the untreated outcome model is correct, subject to the usual regularity and positivity conditions.

## 3

↑ **Parent:** [Paper 221](paper-221.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

The graph factorizes as

$$
p(x)=p(x_2)p(x_1\mid x_2)p(x_4\mid x_2)
p(x_3\mid x_1,x_4)p(x_5\mid x_2)
p(x_6\mid x_4,x_5).
$$

Conditioning on all variables except $X_1$, terms not involving $x_1$ cancel, leaving

$$
p(x_1\mid x_2,x_3,x_4,x_5,x_6)
\propto p(x_1\mid x_2)p(x_3\mid x_1,x_4).
$$

This depends only on $(x_2,x_3,x_4)$, so

$$
X_1\perp(X_5,X_6)\mid(X_2,X_3,X_4).
$$

**Thus $(X_2,X_3,X_4)$ is a [Markov blanket](../../../statistical-model.md#markov-blanket) of $X_1$.**

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

For a distribution faithful to a [Directed acyclic graph](../../../combinatorics.md#directed-acyclic-graph), the smallest Markov blanket of a vertex consists of

- its parents,
- its children, and
- every other parent of one of its children.

Conditioning on this set blocks every path from the vertex to all remaining vertices. Each listed neighbor is necessary under [faithfulness of a directed acyclic graph](../../../causal-inference.md#faithfulness-of-a-directed-acyclic-graph): omitting a parent or child leaves its direct edge active, while omitting a child's other parent leaves the collider path through that conditioned child active. Faithfulness rules out accidental cancellations that could otherwise make a smaller blanket sufficient.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

[Conditional independence](../../../random-variable.md#conditional-independence) $A\perp B\mid D$ means that, for almost every $d$,

$$
p(a,b\mid d)=p(a\mid d)p(b\mid d),
$$

equivalently $p(a\mid b,d)=p(a\mid d)$ wherever the conditional probabilities are defined.

Now use the chain rule and both assumed independences:

$$
\begin{aligned}
p(a,b,c\mid d)
&=p(a\mid b,c,d)p(b,c\mid d)\\
&=p(a\mid b,d)p(b,c\mid d)\\
&=p(a\mid d)p(b,c\mid d).
\end{aligned}
$$

This is exactly $A\perp(B,C)\mid D$, proving the [contraction axiom for conditional independence](../../../random-variable.md#contraction-axiom-for-conditional-independence).

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

Let $M$ be a Markov blanket of the treatment $A$ inside $(A,X)$, and write the remaining adjustment variables as $N=X\setminus M$. By definition,

$$
A\perp N\mid M.
$$

The sufficiency of $X=(M,N)$ gives

$$
A\perp Y(a)\mid(M,N).
$$

Apply the [contraction axiom for conditional independence](../../../random-variable.md#contraction-axiom-for-conditional-independence) with first variable $A$, second variable $N$, third variable $Y(a)$, and conditioning variable $M$. It gives

$$
A\perp(N,Y(a))\mid M.
$$

The [decomposition axiom for conditional independence](../../../random-variable.md#decomposition-axiom-for-conditional-independence) then yields $A\perp Y(a)\mid M$. Hence every Markov blanket of $A$ in $(A,X)$ is itself a [sufficient adjustment set](../../../causal-inference.md#sufficient-adjustment-set).

## 4

↑ **Parent:** [Paper 221](paper-221.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

The [instrumental variable](../../../causal-inference.md#instrumental-variable) graph is

$$
Z\longrightarrow A\longrightarrow Y,
\qquad
U\longrightarrow A,
\qquad
U\longrightarrow Y,
$$

with no arrow $Z\to Y$ and no common cause of $Z$ with $A$ or $Y$.

In [potential outcome](../../../causal-inference.md#potential-outcome) notation, a valid instrument requires:

- [Instrumental-variable independence](../../../causal-inference.md#instrumental-variable-independence): $Z\perp\{A(0),A(1),Y(0),Y(1)\}$, strengthened to all relevant joint potential outcomes as needed. Coin flipping makes the incentive assignment independent of quitting behavior and blood pressure under either assignment.
- [Exclusion restriction](../../../causal-inference.md#exclusion-restriction): $Y(z,a)=Y(a)$. The incentive can affect blood pressure only by changing whether the subject quits, not through stress, income, or another direct route.
- [Instrument relevance](../../../causal-inference.md#instrument-relevance): $\mathbb P\{A(1)\ne A(0)\}>0$, or at least $\mathbb E[A(1)-A(0)]\ne0$. The monetary incentive must change quitting probability.
- [Consistency of potential outcomes](../../../causal-inference.md#consistency-in-causal-inference) and no interference: observed quitting and blood pressure equal the potential values under the assigned encouragement and received exposure, and one subject's assignment does not affect another's outcome.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

[Instrumental-variable monotonicity](../../../causal-inference.md#instrumental-variable-monotonicity) is

$$
A(1)\geq A(0)\quad\text{for every subject}.
$$

It excludes defiers who would quit without the incentive but continue smoking when offered it. The possible [principal strata](../../../causal-inference.md#principal-stratum) are then never-takers $(0,0)$, compliers $(0,1)$, and always-takers $(1,1)$.

By random assignment, consistency, and exclusion,

$$
\begin{aligned}
\mathbb E[Y\mid Z=1]-\mathbb E[Y\mid Z=0]
&=\mathbb E\{Y(A(1))-Y(A(0))\}\\
&=\mathbb E[(Y(1)-Y(0))(A(1)-A(0))].
\end{aligned}
$$

The second identity follows by checking the two possible binary exposure values. Under monotonicity, $A(1)-A(0)$ is the indicator of being a complier. Therefore the numerator is

$$
\mathbb P(\text{complier})
\mathbb E[Y(1)-Y(0)\mid\text{complier}],
$$

while

$$
\mathbb E[A\mid Z=1]-\mathbb E[A\mid Z=0]
=\mathbb E[A(1)-A(0)]
=\mathbb P(\text{complier}).
$$

Their ratio is the [complier average treatment effect](../../../causal-inference.md#local-average-treatment-effect), also called the [local average treatment effect](../../../causal-inference.md#local-average-treatment-effect).

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Let

$$
\delta(u)=\mathbb E[A\mid Z=1,U=u]
-\mathbb E[A\mid Z=0,U=u]
$$

and

$$
\tau(u)=\mathbb E[Y(1)-Y(0)\mid U=u].
$$

Because $U$ contains all exposure-outcome confounding and $Z$ is independent of $U$, the exclusion restriction and the law of total expectation give

$$
\mathbb E[Y\mid Z=1]-\mathbb E[Y\mid Z=0]
=\mathbb E\{\tau(U)\delta(U)\}.
$$

Likewise,

$$
\mathbb E[A\mid Z=1]-\mathbb E[A\mid Z=0]
=\mathbb E\{\delta(U)\}.
$$

The no [confounder-instrument interaction](../../../causal-inference.md#confounder-instrument-interaction) assumption says $\delta(U)=\delta$ is constant. Relevance gives $\delta\ne0$, so the Wald ratio is

$$
\frac{\delta\,\mathbb E\tau(U)}{\delta}
=\mathbb E[Y(1)-Y(0)],
$$

the overall [average treatment effect](../../../causal-inference.md#average-treatment-effect).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
