# Paper 221

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_221.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_221.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
    - [iv](#1/b/iv)
      - [Solution](#1/b/iv/solution)
    - [v](#1/b/v)
      - [Solution](#1/b/v/solution)
    - [vi](#1/b/vi)
      - [Solution](#1/b/vi/solution)
    - [vii](#1/b/vii)
      - [Solution](#1/b/vii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
    - [iii](#3/b/iii)
      - [Solution](#3/b/iii/solution)
    - [iv](#3/b/iv)
      - [Solution](#3/b/iv/solution)
  - [c](#3/c)
    - [i](#3/c/i)
      - [Solution](#3/c/i/solution)
    - [ii](#3/c/ii)
      - [Solution](#3/c/ii/solution)
    - [iii](#3/c/iii)
      - [Solution](#3/c/iii/solution)
    - [iv](#3/c/iv)
      - [Solution](#3/c/iv/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
  - [b](#4/b)
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)

## 1

↑ **Parent:** [Paper 221](paper-221.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

In a standardized [linear structural equation model](../../../causal-inference.md#linear-structural-equation-model), attach to every directed edge its path coefficient. [Wright path tracing rule](../../../causal-inference.md#wright-path-tracing-rule) says that a covariance is the sum, over admissible unblocked paths between the two variables, of the product of the coefficients along each path; an admissible path does not pass through a collider and does not enter and later leave the same variable in a way that reverses direction twice. The total causal effect of $X$ on $Y$ is the sum of the products of edge coefficients over all directed paths from $X$ to $Y$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

The $X_1$ coefficient is the total causal effect of $X_1$ on $Y$. The node $X_1$ has no parents, so there is no [backdoor path](../../../causal-inference.md#backdoor-path) into it, and the unadjusted regression sums all directed paths from $X_1$ to $Y$.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

The $X_2$ coefficient has no causal interpretation. The open backdoor path $X_2\leftarrow X_1\to Y$, together with paths through $X_3$, confounds the unadjusted association.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

The $X_3$ coefficient has no causal interpretation. In particular, $X_3\leftarrow U\to Y$ is an open backdoor path, and $X_1$ and $X_2$ supply further confounding paths.

<h4 id="1/b/iv">iv</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/b/iv)

After adjusting for $X_1$, the $X_2$ coefficient is the total causal effect of $X_2$ on $Y$, consisting of $X_2\to Y$ and $X_2\to X_3\to Y$. The $X_1$ coefficient is the causal effect of $X_1$ with $X_2$ held fixed: it retains paths not passing through $X_2$, namely the direct path and $X_1\to X_3\to Y$.

<h4 id="1/b/v">v</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/v/solution">Solution</h5>

↑ **Parent:** [V](#1/b/v)

Neither coefficient has a causal interpretation. Conditioning on $X_3$ opens the [collider bias](../../../causal-inference.md#collider-bias) path $X_1\to X_3\leftarrow U\to Y$ for the $X_1$ coefficient, while the $X_3$ coefficient remains confounded by $U$ and by omitted $X_2$.

<h4 id="1/b/vi">vi</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/vi/solution">Solution</h5>

↑ **Parent:** [Vi](#1/b/vi)

Neither coefficient has a causal interpretation. The $X_2$ coefficient is confounded by omitted $X_1$, and conditioning on the collider $X_3$ also opens $X_2\to X_3\leftarrow U\to Y$. The $X_3$ coefficient retains the open path through $U$.

<h4 id="1/b/vii">vii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/vii/solution">Solution</h5>

↑ **Parent:** [Vii](#1/b/vii)

None of the three coefficients has a causal interpretation. The $X_3$ coefficient is unavoidably confounded by unmeasured $U$. Conditioning on the collider $X_3$ opens paths through $U$ for both $X_1$ and $X_2$, so adding all measured regressors does not repair the bias.

## 2

↑ **Parent:** [Paper 221](paper-221.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Write $p=p^*$, $\mu_z=\mathbb E(Y\mid Z=z)$, and $\tau^*=\mu_1-\mu_0$. The summand has finite variance, so the [central limit theorem](../../../convergence-of-random-variables.md#central-limit-theorem) gives

$$
\sqrt n(\widetilde\tau-\tau^*)
\xrightarrow{d}N(0,V_{\mathrm{known}}),
$$

where

$$
V_{\mathrm{known}}
=\frac{\mathbb E(Y^2\mid Z=1)}p
+\frac{\mathbb E(Y^2\mid Z=0)}{1-p}
-(\mu_1-\mu_0)^2.
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For $\vartheta=(q,t)$ use the [estimating equation](../../../statistical-inference.md#estimating-equation)

$$
\psi(Y,Z;\vartheta)=
\binom{Z-q}{ZY/q-(1-Z)Y/(1-q)-t}.
$$

Its empirical mean vanishes exactly at $(\widehat p,\widehat\tau)$. The population equation has the unique root $(p,\tau^*)$, so the [Z-estimator](../../../statistical-inference.md#z-estimator) is consistent. Linearizing the equation, or simplifying the corresponding sandwich covariance, gives the influence function

$$
\phi(Y,Z)
=\frac Zp(Y-\mu_1)-\frac{1-Z}{1-p}(Y-\mu_0).
$$

Hence

$$
\boxed{\sqrt n(\widehat\tau-\tau^*)
\xrightarrow{d}N(0,V_{\mathrm{estimated}}),
\qquad
V_{\mathrm{estimated}}
=\frac{\operatorname{Var}(Y\mid Z=1)}p
+\frac{\operatorname{Var}(Y\mid Z=0)}{1-p}.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Subtracting the two asymptotic variances and expanding the conditional second moments gives

$$
V_{\mathrm{known}}-V_{\mathrm{estimated}}
=\frac{\bigl((1-p)\mu_1+p\mu_0\bigr)^2}{p(1-p)}\geq0.
$$

Estimating the randomized treatment probability therefore projects out the component of the known-probability influence function proportional to $Z-p$, weakly improving asymptotic efficiency.

## 3

↑ **Parent:** [Paper 221](paper-221.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A minimal [causal directed acyclic graph](../../../causal-inference.md#causal-directed-acyclic-graph) has edges

$$
A\to Y,quad A\to M,quad M\to Y,quad M\to S,quad
Z\to A,quad D\to A,quad D\to C,quad C\to M,quad
G\to A,quad G\to Y,quad W\to Y.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

**Yes.** Every path from $D$ to $G$ is blocked by a collider, such as $D\to A\leftarrow G$ or $D\to C\to M\leftarrow A\leftarrow G$. Thus [D-separation](../../../combinatorics.md#d-separation) gives $D\mathbin\perp G$.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

**No.** Conditioning on the collider $A$ opens $D\to A\leftarrow Z$, so $D$ and $Z$ are not conditionally independent given $A$.

<h4 id="3/b/iii">iii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/b/iii)

**Yes.** Conditioning on $A$ blocks the directed paths from $Z$ to $Y$. Although conditioning on $A$ opens $Z\to A\leftarrow G\to Y$ and $Z\to A\leftarrow D\to C\to M\to Y$, conditioning additionally on $G$ and $D$ blocks those paths. Hence $Z\mathbin\perp Y\mid(A,G,D)$.

<h4 id="3/b/iv">iv</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#3/b/iv)

**Yes.** Conditioning on $D$ blocks $C\leftarrow D\to A$, while $C\to M\leftarrow A$ is blocked at the collider $M$. Therefore $C\mathbin\perp A\mid D$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/i">i</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/i/solution">Solution</h5>

↑ **Parent:** [I](#3/c/i)

The independence fails after conditioning on $S=1$. Since $S$ is a descendant of collider $M$, selection opens $D\to C\to M\leftarrow A\leftarrow G$.

<h4 id="3/c/ii">ii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/c/ii)

The independence already failed, and it still fails because conditioning on $A$ opens $D\to A\leftarrow Z$.

<h4 id="3/c/iii">iii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/c/iii)

The independence still holds. Every path from $Z$ starts through $A$; paths on which $A$ is a noncollider are blocked by conditioning on $A$, while paths opened at collider $A$ are blocked by the conditioned variables $G$ or $D$. Conditioning on $S$ creates no route avoiding these blocks.

<h4 id="3/c/iv">iv</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#3/c/iv)

The independence fails. Conditioning on $S$, a descendant of $M$, opens the collider path $C\to M\leftarrow A$ even after conditioning on $D$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Each factor $f_{j\mid\operatorname{pa}(j)}$ depends only on node $j$ and its parents. Those vertices form a clique in the [moral graph](../../../combinatorics.md#moral-graph), because moralization joins every pair of parents and removes arrow directions. The positive joint density therefore factors into clique potentials of the moral graph. The [Hammersley-Clifford theorem](../../../combinatorics.md#hammersley-clifford-theorem) then implies the global Markov property for that undirected graph.

## 4

↑ **Parent:** [Paper 221](paper-221.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

By [consistency of potential outcomes](../../../causal-inference.md#consistency-in-causal-inference) and [conditional exchangeability](../../../causal-inference.md#conditional-exchangeability),

$$
\mathbb E[Y(z)\mid X]
=\mathbb E[Y(z)\mid Z=z,X]
=\mathbb E[Y\mid Z=z,X].
$$

Taking conditional expectations given $X_1=x_1$ and subtracting the cases $z=1$ and $z=0$ proves the outcome-regression identification formula.

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

Conditional on $X$,

$$
\mathbb E\!\left[\frac{ZY}{e(X)}\middle|X\right]
=\mathbb E[Y\mid Z=1,X],
\qquad
\mathbb E\!\left[\frac{(1-Z)Y}{1-e(X)}\middle|X\right]
=\mathbb E[Y\mid Z=0,X].
$$

Multiplying by $\mathbf1\{X_1=x_1\}$, taking expectations, dividing by $\mathbb P(X_1=x_1)$, and using part (i) proves the [inverse probability weighting](../../../causal-inference.md#inverse-probability-weighting) formula.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

Write $m_z(X)=\mu_z(X,\beta_z)$ and $\widetilde e(X)=e(X;\alpha)$. Conditional on $X$,

$$
\widetilde\mu_1^{\mathrm{dr}}(X)
=m_1(X)+\frac{e(X)}{\widetilde e(X)}\bigl(\mu_1(X)-m_1(X)\bigr),
$$

with the analogous control expression

$$
\widetilde\mu_0^{\mathrm{dr}}(X)
=m_0(X)+\frac{1-e(X)}{1-\widetilde e(X)}\bigl(\mu_0(X)-m_0(X)\bigr).
$$

If the propensity model is correct, both ratios are one and these equal $\mu_1(X)$ and $\mu_0(X)$, so their difference is the [conditional average treatment effect](../../../causal-inference.md#conditional-average-treatment-effect).

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

If both outcome models are correct, each residual term in the preceding conditional expectations has mean zero regardless of the working propensity model. Thus $\widetilde\mu_z^{\mathrm{dr}}(X)=\mu_z(X)$ for $z=0,1$, and their difference is again $\tau(X)$. This proves [double robustness](../../../probability-and-statistics.md#double-robustness).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
