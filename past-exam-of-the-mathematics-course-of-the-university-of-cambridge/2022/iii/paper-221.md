# Paper 221

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_221.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_221.pdf)

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
  - [iv](#4/iv)
    - [Solution](#4/iv/solution)

## 1

↑ **Parent:** [Paper 221](paper-221.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

In [potential outcome](../../../causal-inference.md#potential-outcome) notation, a valid [instrumental variable](../../../causal-inference.md#instrumental-variable) $Z$ must satisfy:

- [Instrument relevance](../../../causal-inference.md#instrument-relevance): the conditional law of $A$ changes with $Z$.
- [Instrumental-variable independence](../../../causal-inference.md#instrumental-variable-independence): $Z$ is independent of the joint collection of potential treatments and outcomes, such as $\{A(z),Y(a):z,a\}$.
- The [exclusion restriction](../../../causal-inference.md#exclusion-restriction): $Y(z,a)=Y(a)$, so $Z$ can affect $Y$ only through $A$.
- [Consistency of potential outcomes](../../../causal-inference.md#consistency-in-causal-inference) and no [interference in causal inference](../../../causal-inference.md#interference-in-causal-inference) connect the potential variables to the observations.

In the graph, $Z_1$ has open noncausal paths to $Y$ that do not pass through $A$, including

$$
Z_1\leftarrow M_1\to C\to Y
\qquad\text{and}\qquad
Z_1\leftarrow S\to Z_3\to Y.
$$

Equivalently, these paths remain after deleting the causal edge $A\to Y$. Thus $Z_1$ is associated with potential outcomes through the latent variables $C$ and $S$, violating [instrumental-variable independence](../../../causal-inference.md#instrumental-variable-independence); it is not a valid marginal instrument.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Among observed pretreatment variables, every sufficient set must contain $M_1$ to block

$$
Z_1\leftarrow M_1\to C\to Y
$$

and $Z_3$ to block

$$
Z_1\leftarrow S\to Z_3\to Y.
$$

Conditioning on $Z_3$ opens the [collider](../../../combinatorics.md#collider) on

$$
Z_1\leftarrow S\to Z_3\leftarrow M_3\to C\to Y,
$$

so $M_3$ must also be included. The resulting minimal [sufficient adjustment set](../../../causal-inference.md#sufficient-adjustment-set) is

$$
X_0=\{M_1,M_3,Z_3\}.
$$

It blocks every path from $Z_1$ to $Y$ that remains after removing $A\to Y$, while the open path

$$
Z_1\leftarrow S\to Z_2\to A
$$

preserves [instrument relevance](../../../causal-inference.md#instrument-relevance). Adding $M_2$ blocks no required relevance path, so

$$
X_1=\{M_1,M_2,M_3,Z_3\}
$$

is also sufficient.

There are no others. In particular, adding $Z_2$ blocks the displayed relevance path. Without $M_2$, conditioning on $Z_2$ also opens

$$
Z_1\leftarrow S\to Z_2\leftarrow M_2\to C\to Y,
$$

which violates independence; adding $M_2$ closes that path but leaves no open path from $Z_1$ to $A$. Hence the complete list is $X_0$ and $X_1$.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

For one unit write $M=(M_1,M_2,M_3)$ and $W=(M,Z_1,Z_3)$. Since the graph makes $S$ independent of $M$, the known distributions determine the conditional assignment law

$$
q(z_2\mid w)
=\frac{
\sum_s p(s)p(z_1,z_2,z_3\mid m,s)
}{
\sum_s\sum_{z_2'}p(s)p(z_1,z_2',z_3\mid m,s)
}.
$$

Under the [sharp causal null hypothesis](../../../causal-inference.md#causal-null-hypothesis) that $A$ has no effect on $Y$, delete $A\to Y$. The [D-separation](../../../combinatorics.md#d-separation) criterion then gives

$$
Z_2\mathrel\perp Y\mid W:
$$

$M_2$ blocks the route through $C$, $Z_3$ blocks the route through $S$, $M_1$ and $M_3$ block the collider-opened detours through $Z_1$ and $Z_3$, and $A$ remains a collider on routes through $U$.

For independent units $i=1,\ldots,n$, choose a [test statistic](../../../statistical-modelling.md#test-statistic) $T(Z_{2,1:n},Y_{1:n},W_{1:n})$ that measures residual association between $Z_2$ and $Y$. Hold $(Y_i,W_i)$ fixed and independently draw

$$
Z_{2i}^{(b)}\sim q(\mathord\cdot\mid W_i),
\qquad b=1,\ldots,B.
$$

Recompute $T^{(b)}$ after each draw. A valid Monte Carlo [conditional randomization test](../../../statistical-modelling.md#conditional-randomization-test) uses

$$
p_B=\frac{1+\sum_{b=1}^B\mathbf1_{\{T^{(b)}\geq T^{\rm obs}\}}}{B+1},
$$

with a two-sided statistic or absolute value when appropriate.

Under the null, conditional on $(Y_{1:n},W_{1:n})$, the observed $Z_{2,1:n}$ and its $B$ resamples are exchangeable because they have the same product law $\prod_iq(\mathord\cdot\mid W_i)$. The rank of $T^{\rm obs}$ among the $B+1$ values is therefore uniform after randomized tie breaking and conservative without it. Consequently

$$
\mathbb P_{H_0}(p_B\leq\alpha\mid Y_{1:n},W_{1:n})\leq\alpha.
$$

Taking expectations proves unconditional [Type I error](../../../information-theory.md#type-i-and-type-ii-errors) control.

## 2

↑ **Parent:** [Paper 221](paper-221.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Take all components to be centered and let their marginal variances be $V_A,V_C,V_E$. A [linear structural equation model](../../../causal-inference.md#linear-structural-equation-model) is

$$
C_{i1}=C_{i2}=C_i,
\qquad
Y_{ij}=A_{ij}+C_i+E_{ij},
$$

where $C_i,E_{i1},E_{i2}$ are mutually independent and the $E_{ij}$ are identically distributed. The [causal directed acyclic graph](../../../causal-inference.md#causal-directed-acyclic-graph) has arrows

$$
A_{i1}\to Y_{i1}\leftarrow C_i\to Y_{i2}\leftarrow A_{i2},
\qquad
E_{i1}\to Y_{i1},
\qquad
E_{i2}\to Y_{i2}.
$$

For [monozygotic twins](../../../biology.md#monozygotic-twin), set $A_{i1}=A_{i2}=G_i$ with $\operatorname{Var}(G_i)=V_A$; the genetic cause is completely shared. For [dizygotic twins](../../../biology.md#dizygotic-twin), one explicit construction is

$$
A_{i1}=G_i+G_{i1},
\qquad
A_{i2}=G_i+G_{i2},
$$

where $G_i,G_{i1},G_{i2}$ are independent with variance $V_A/2$. Then both additive genetic terms have variance $V_A$, while their covariance is $V_A/2$ and their [correlation coefficient](../../../variance.md#pearson-correlation-coefficient) is $1/2$. In a fuller graph, the shared $G_i$ points to both genetic components and the unique $G_{ij}$ points only to its own component.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The common marginal trait variance is

$$
V_Y=V_A+V_C+V_E.
$$

For monozygotic pairs, shared genes and shared environment give

$$
\operatorname{Cov}(Y_{i1},Y_{i2})=V_A+V_C,
\qquad
r_{\rm MZ}=\frac{V_A+V_C}{V_Y}.
$$

For dizygotic pairs, the genetic covariance is halved while the common environment is unchanged:

$$
\operatorname{Cov}(Y_{i1},Y_{i2})=\frac12V_A+V_C,
\qquad
r_{\rm DZ}=\frac{V_A/2+V_C}{V_Y}.
$$

Subtracting cancels the common-environment variance and proves [Falconer's formula](../../../biology.md#falconer-s-formula)

$$
2(r_{\rm MZ}-r_{\rm DZ})
=\frac{V_A}{V_Y}=h^2,
$$

the [heritability](../../../biology.md#heritability) under the [ACE model](../../../biology.md#ace-model).

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Suppose [assortative mating](../../../biology.md#assortative-mating) raises the dizygotic genetic correlation from $1/2$ to $\rho>1/2$. Then

$$
r_{\rm DZ}=\frac{\rho V_A+V_C}{V_Y},
$$

so the formula returns

$$
2(r_{\rm MZ}-r_{\rm DZ})
=2(1-\rho)\frac{V_A}{V_Y}
<h^2.
$$

**Thus using the nominal one-half genetic correlation produces downward bias in estimated heritability, assuming the other ACE assumptions remain valid.**

## 3

↑ **Parent:** [Paper 221](paper-221.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

The [no unmeasured confounding assumption](../../../causal-inference.md#conditional-exchangeability), or [conditional exchangeability](../../../causal-inference.md#conditional-exchangeability), is

$$
(Y(0),Y(1))\mathrel\perp A\mid X.
$$

Also assume [consistency of potential outcomes](../../../causal-inference.md#consistency-in-causal-inference), no [interference in causal inference](../../../causal-inference.md#interference-in-causal-inference), [positivity in causal inference](../../../causal-inference.md#positivity-assumption), and finite expectations. For $a\in\{0,1\}$, the [law of total expectation](../../../measure-theory.md#law-of-total-expectation), exchangeability, and consistency give

$$
\begin{aligned}
\mathbb E[Y(a)]
&=\mathbb E\{\mathbb E[Y(a)\mid X]\}\\
&=\mathbb E\{\mathbb E[Y(a)\mid A=a,X]\}\\
&=\mathbb E\{\mathbb E[Y\mid A=a,X]\}.
\end{aligned}
$$

Positivity ensures that the observed conditional means exist on the covariate support being averaged. Subtracting the two cases identifies the [average treatment effect](../../../causal-inference.md#average-treatment-effect) as

$$
\boxed{\beta_1
=\mathbb E\{\mathbb E[Y\mid A=1,X]\}
-\mathbb E\{\mathbb E[Y\mid A=0,X]\}.}
$$

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Under the [partially linear model](../../../statistical-inference.md#partially-linear-model),

$$
\mathbb E[Y\mid A=1,X]-\mathbb E[Y\mid A=0,X]
=\beta_2.
$$

Inserting this constant conditional contrast into the identification formula from part i gives

$$
\boxed{\beta_1=\mathbb E[\beta_2]=\beta_2.}
$$

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

For fixed $\beta$, conditional least squares is minimized by

$$
g_\beta(X)=\mathbb E[Y-\beta A\mid X]
=\mu(X)-\beta e(X).
$$

Therefore the remaining objective is

$$
\mathbb E\left[
\{Y-\mu(X)-\beta(A-e(X))\}^2
\right],
$$

whose [normal equation](../../../statistical-modelling.md#normal-equation) gives

$$
\beta_3
=\frac{\mathbb E[(A-e(X))(Y-\mu(X))]}
{\mathbb E[(A-e(X))^2]}.
$$

Let

$$
\tau(X)=\mathbb E[Y(1)-Y(0)\mid X]
$$

be the [conditional average treatment effect](../../../causal-inference.md#conditional-average-treatment-effect). Since $A$ is binary, conditional exchangeability implies

$$
\operatorname{Cov}(A,Y\mid X)
=e(X)\{1-e(X)\}\tau(X),
$$

and $\operatorname{Var}(A\mid X)=e(X)\{1-e(X)\}$. Hence

$$
\beta_3
=\frac{\mathbb E[e(X)\{1-e(X)\}\tau(X)]}
{\mathbb E[e(X)\{1-e(X)\}]}.
$$

Thus $\beta_3$ is the [overlap-weighted average treatment effect](../../../causal-inference.md#overlap-weighted-average-treatment-effect). It weights covariate strata by the [overlap weight](../../../causal-inference.md#overlap-weight) and generally differs from the ordinary ATE $\beta_1=\mathbb E[\tau(X)]$ when treatment effects are heterogeneous and overlap varies with $X$.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

Differentiating the residualized objective gives

$$
\beta_4
=\frac{\mathbb E[\widetilde A\widetilde Y]}
{\mathbb E[\widetilde A^2]}
=\frac{\mathbb E[(A-e(X))(Y-\mu(X))]}
{\mathbb E[(A-e(X))^2]}
=\beta_3.
$$

This is the population [Frisch–Waugh–Lovell theorem](../../../linear-regression.md#frisch-waugh-lovell-theorem).

For a [semiparametric estimator](../../../statistical-inference.md#semiparametric-estimator), estimate $e(x)=\mathbb E[A\mid X=x]$ and $\mu(x)=\mathbb E[Y\mid X=x]$ flexibly. With [cross-fitting](../../../probability-and-statistics.md#cross-fitting), obtain held-out predictions $\widehat e_i,\widehat\mu_i$ and regress the residualized outcome on the residualized treatment through the origin:

$$
\widehat\beta_3
=\frac{\sum_{i=1}^n(A_i-\widehat e_i)(Y_i-\widehat\mu_i)}
{\sum_{i=1}^n(A_i-\widehat e_i)^2}.
$$

Cross-fitting limits overfitting bias and permits flexible nuisance estimators under the usual convergence and overlap conditions.

## 4

↑ **Parent:** [Paper 221](paper-221.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

The administrative data include only encounters with $M=1$. Conditioning on the stop indicator selects on the [collider](../../../combinatorics.md#collider)

$$
D\to M\leftarrow U,
$$

which opens the noncausal path $D\leftrightarrow U\to Y$ and creates [collider bias](../../../causal-inference.md#collider-bias). The equal entries estimate only the selected risks $\mathbb P(Y=1\mid D=d,M=1)$. They ignore racial differences in the probability of being stopped and therefore do not identify the total [causal effect](../../../causal-inference.md#causal-effect) of race on violence. This is also [selection bias](../../../causal-inference.md#selection-bias), because encounters with $M=0$ never enter the dataset.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Let $Y(d,m)$ be the potential violence outcome if race were set to $d$ and stop status to $m$. The substantive assumption is the [structural zero](../../../causal-inference.md#structural-zero)

$$
Y(d,0)=0
\qquad\text{for every unit and }d\in\{0,1\}.
$$

Equivalently, with the natural stop status $M(d)$, $M(d)=0$ implies $Y(d)=Y(d,M(d))=0$.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

The graph has no cause of $D$, so $D$ is independent of its potential outcomes. By [consistency of potential outcomes](../../../causal-inference.md#consistency-in-causal-inference), the [G-formula](../../../causal-inference.md#g-computation) therefore gives

$$
\mathbb E[Y(d)]=\mathbb E[Y\mid D=d].
$$

Condition on $M$ and use the structural zero from part ii:

$$
\begin{aligned}
\mathbb E[Y(d)]
&=\mathbb E[Y\mid D=d,M=1]\mathbb P(M=1\mid D=d)\\
&\quad+\mathbb E[Y\mid D=d,M=0]\mathbb P(M=0\mid D=d)\\
&=\mathbb E[Y\mid D=d,M=1]\mathbb P(M=1\mid D=d).
\end{aligned}
$$

Consequently the [causal risk ratio](../../../causal-inference.md#causal-risk-ratio) is

$$
\frac{\mathbb E[Y(1)]}{\mathbb E[Y(0)]}
=\frac{\mathbb E[Y\mid D=1,M=1]}{\mathbb E[Y\mid D=0,M=1]}
\frac{\mathbb P(M=1\mid D=1)}{\mathbb P(M=1\mid D=0)}.
$$

Applying [Bayes' theorem](../../../probability-theory.md#bayes-theorem) to the second factor gives

$$
\frac{\mathbb P(M=1\mid D=1)}{\mathbb P(M=1\mid D=0)}
=\frac{\mathbb P(D=1\mid M=1)/\mathbb P(D=0\mid M=1)}
{\mathbb P(D=1)/\mathbb P(D=0)},
$$

which proves the stated formula. The unmeasured common cause $U$ of $M$ and $Y$ does not obstruct this total-effect argument because no mediator effect is being identified.

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#4/iv)

The stop records estimate

$$
\mathbb E[Y\mid D=d,M=1]
\quad\text{and}\quad
\mathbb P(D=d\mid M=1),
$$

but they cannot estimate the population encounter probabilities $\mathbb P(D=1)$ and $\mathbb P(D=0)$ because encounters without a stop are absent. Equivalently, they do not determine the race-specific stop-probability ratio.

The scientist needs a representative denominator for all police-civilian encounters, including those with $M=0$. Suitable sources could include a carefully designed population or travel survey, systematic street and traffic observation, dispatch or body-camera sampling that records non-stop encounters, or an external administrative source measuring exposure to police by race. Combining its estimate of the population race odds with the estimable stop-data terms identifies the displayed causal risk ratio, provided the external sample targets the same city, period, and encounter population.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
