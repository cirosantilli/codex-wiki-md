# Paper 205

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20205.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20205.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

With the usual objective

$$
\frac1{2n}\lVert Y-\widehat\mu\mathbf1-X\beta\rVert_2^2+\lambda\lVert\beta\rVert_1,
$$

the [Karush-Kuhn-Tucker conditions](../../../mathematical-optimization.md#karush-kuhn-tucker-conditions) for the [Lasso](../../../probability-and-statistics.md#lasso) are

$$
\frac1nX^T(Y-\widehat\mu\mathbf1-X\widehat\beta_\lambda)=\lambda z,
\quad
z_j=\operatorname{sgn}(\widehat\beta_{\lambda j})\text{ if }\widehat\beta_{\lambda j}\ne0,
\quad |z_j|\leq1\text{ otherwise}.
$$

Comparing the objective at $\widehat\beta_\lambda$ and $\beta^0$, expanding the square, and cancelling the noise norm gives exactly

$$
\frac1n\lVert X(\beta^0-\widehat\beta_\lambda)\rVert_2^2
\leq\frac1n\varepsilon^TX(\widehat\beta_\lambda-\beta^0)
+\lambda\lVert\beta^0\rVert_1-\lambda\lVert\widehat\beta_\lambda\rVert_1.
$$

Choose $\lambda=A\sigma\sqrt{\log p/n}$. Since every column has norm $\sqrt n$, each $X_j^T\varepsilon/n$ is [sub-Gaussian](../../../probability-and-statistics.md#sub-gaussian-distribution) with parameter $\sigma/\sqrt n$. A [union bound](../../../probability-inequality.md#boole-s-inequality) gives

$$
\mathbb P\!\left(\left\lVert\frac1nX^T\varepsilon\right\rVert_\infty>\lambda\right)
\leq2p\exp\!\left(-\frac{n\lambda^2}{2\sigma^2}\right)
=2p^{-(A^2/2-1)}.
$$

On the complementary event, [Holder inequality](../../../functional-analysis.md#holder-inequality) and the triangle inequality bound the preceding right-hand side by

$$
\lambda\lVert\widehat\beta_\lambda-\beta^0\rVert_1
+\lambda\lVert\beta^0\rVert_1-\lambda\lVert\widehat\beta_\lambda\rVert_1
\leq2\lambda\lVert\beta^0\rVert_1,
$$

which proves the stated prediction bound.

For the [Dantzig selector](../../../probability-and-statistics.md#dantzig-selector), use the constraint $n^{-1}\lVert X^T(Y-X\beta)\rVert_\infty\leq\lambda$. The Lasso KKT conditions make $\widehat\beta_\lambda$ feasible, so a Dantzig minimizer $\widetilde\beta$ has no larger $\ell^1$ norm. If $\widetilde\beta$ were not the Lasso solution, uniqueness from invertibility of $X^TX$ would imply that some active coordinate $j$ has strict signed KKT slack. For small $\eta>0$, set

$$
\beta_\eta=\widetilde\beta-eta\operatorname{sgn}(\widetilde\beta_j)(X^TX)^{-1}e_j.
$$

Only score coordinate $j$ changes, toward its feasible boundary, so $\beta_\eta$ remains feasible. For small $\eta$, signs on the active coordinates do not change, and

$$
\lVert\beta_\eta\rVert_1-\lVert\widetilde\beta\rVert_1
\leq\eta\left(-[(X^TX)^{-1}]_{jj}+\sum_{k\ne j}|[(X^TX)^{-1}]_{kj}|\right)<0
$$

by strict [diagonal dominance](../../../algebra.md#diagonal-dominance). This contradicts Dantzig optimality, so the two estimators coincide.

## 2

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation) gives

$$
\mathbb E\!\left[\frac{YT}{\pi(X)}\middle|X\right]
=\frac{\mathbb E[YT\mid X]}{\pi(X)}
=\frac{\pi(X)\mu(X)}{\pi(X)}=\mu(X),
$$

and another expectation gives $\theta$.

Use the [augmented inverse-probability-weighted estimator](../../../probability-and-statistics.md#augmented-inverse-probability-weighted-estimator)

$$
\widehat\theta_n=\frac1n\sum_{i=1}^n
\left[\widehat\mu_n(X_i)+\frac{T_i}{\widehat\pi_n(X_i)}
\{Y_i-\widehat\mu_n(X_i)\}\right].
$$

Condition on the independently trained nuisance estimators. Subtracting the oracle influence variable

$$
\phi(X,Y,T)=\mu(X)+\frac{T}{\pi(X)}(Y-\mu(X))
$$

produces a conditional empirical fluctuation with variance $o(1)$ after multiplication by $\sqrt n$, using $\mathcal E_\mu,\mathcal E_\pi\to0$, overlap, and the bounded conditional variance. Its conditional bias is

$$
\mathbb E\left[(\widehat\mu_n(X)-\mu(X))
\left(1-\frac{\pi(X)}{\widehat\pi_n(X)}\right)\right],
$$

whose absolute value is at most $\sqrt{\mathcal E_\mu\mathcal E_\pi}=o(n^{-1/2})$ by [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality). Thus

$$
\sqrt n(\widehat\theta_n-\theta)
=\frac1{\sqrt n}\sum_{i=1}^n(\phi_i-\theta)+o_P(1).
$$

The [central limit theorem](../../../convergence-of-random-variables.md#central-limit-theorem) and [Slutsky theorem](../../../statistical-inference.md#slutsky-theorem) give the claimed $N(0,v)$ limit. Without auxiliary data, use [cross-fitting](../../../probability-and-statistics.md#cross-fitting): split the sample into folds, train both nuisance estimators away from each observation's fold, and average the same score over held-out observations.

## 3

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A real [positive-semidefinite kernel](../../../probability-and-statistics.md#positive-semidefinite-kernel) is a symmetric function $k$ such that every finite Gram matrix $K_{ij}=k(x_i,x_j)$ is positive semidefinite. The [representer theorem](../../../probability-and-statistics.md#representer-theorem) says that any minimizer in a [Reproducing kernel Hilbert space](../../../probability-and-statistics.md#reproducing-kernel-hilbert-space) of an objective depending on $f$ only through $f(x_1),\ldots,f(x_n)$ and a strictly increasing function of $\lVert f\rVert_{\mathcal H}$ lies in

$$
\operatorname{span}\{k(x_1,\mathord\cdot),\ldots,k(x_n,\mathord\cdot)\}.
$$

Indeed, write $f=f_\parallel+f_\perp$ relative to this span. The reproducing property gives $f_\perp(x_i)=0$ for every $i$, while the [Pythagorean theorem in an inner-product space](../../../linear-algebra.md#pythagorean-theorem-in-an-inner-product-space) gives $\lVert f\rVert^2=\lVert f_\parallel\rVert^2+\lVert f_\perp\rVert^2$. Removing a nonzero perpendicular component preserves all data values and strictly decreases the penalty, proving the theorem.

Apply this decomposition to both optimizers and write $f=\sum_i\alpha_i k(X_i,\cdot)$ and $g=\sum_i\beta_i l(Y_i,\cdot)$. If $K$ and $L$ are the two [Gram matrices](../../../linear-algebra.md#gram-matrix), then

$$
\sum_i f(X_i)g(Y_i)=\alpha^TKL\beta,
\qquad \lVert f\rVert_{\mathcal H}^2=\alpha^TK\alpha,
\qquad \lVert g\rVert_{\mathcal G}^2=\beta^TL\beta.
$$

Writing $u=K^{1/2}\alpha$ and $v=L^{1/2}\beta$, with pseudoinverses on the respective ranges, turns the supremum into

$$
\sup_{\lVert u\rVert_2,\lVert v\rVert_2\leq1}u^TK^{1/2}L^{1/2}v
=\sigma_{\max}(K^{1/2}L^{1/2}).
$$

## 4

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The graph has edges $1\to2\leftarrow3$, $1\to4$, $2\to4$, $3\to5$, $4\to5$, $4\to6$, and $6\to5$. Any [D-separating set](../../../combinatorics.md#d-separating-set) for 1 and 6 must contain 4 because of the directed path $1\to4\to6$. Conditioning on 4 activates the collider $1\to4\leftarrow2$ and, through its descendant, the collider $1\to2\leftarrow3$. The remaining route through $3\to5\leftarrow6$ is open exactly when 5 is conditioned on and 3 is not. Hence all separating sets, among the nonendpoint vertices, are

$$
\{4\},\quad\{2,4\},\quad\{3,4\},\quad\{2,3,4\},
\quad\{3,4,5\},\quad\{2,3,4,5\}.
$$

For the second graph, $2\perp\!\!\!\perp5\mid1,6$ forces colliders on the unblocked two-edge paths: $2\to3\leftarrow5$ and $2\to4\leftarrow5$. Acyclicity then forces $1\to4$ and $6\to4$. Thus its edges are

$$
\boxed{1\to2,quad2\to3,quad5\to3,quad1\to4,quad2\to4,
\quad5\to4,quad6\to4,quad6\to5.}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Choose the given [topological ordering](../../../combinatorics.md#topological-ordering). Since $j$ precedes $k$, $j$ is not a descendant of $k$; since they are nonadjacent, it is not a parent of $k$. The [local Markov property of a directed acyclic graph](../../../combinatorics.md#local-markov-property-of-a-directed-acyclic-graph) says that a node is d-separated from all its nondescendants other than its parents by its parent set. Therefore $j$ and $k$ are d-separated by $\operatorname{pa}(k)$.

It follows that adjacency of $Z_1,Z_2$ is certified by rejecting every null hypothesis

$$
Z_1\perp\!\!\!\perp Z_2\mid Z_S,
\qquad S\subseteq\{3,\ldots,p\}.
$$

If the vertices were nonadjacent, the theorem would supply one such separating parent set, whichever vertex comes later.

To certify that $X_1$ is a parent of $Y$, first reject

$$
X_1\perp\!\!\!\perp Y\mid (I,X_S)
$$

for every $S\subseteq\{2,\ldots,d\}$, which forces adjacency. Then reject

$$
I\perp\!\!\!\perp Y\mid X_S
$$

for every such $S$. If the adjacent edge were $Y\to X_1$, then $I\to X_1\leftarrow Y$ would orient $X_1$ as a collider, and the parent-set argument would provide a separator not containing $X_1$, contradicting the second collection of rejections. Hence the edge is $X_1\to Y$.

## 5

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

The [conditional multivariate normal distribution](../../../probability-and-statistics.md#conditional-multivariate-normal-distribution) gives

$$
y\mid z\sim N(z^T\beta,\sigma^2),
\quad
\beta=\Sigma_{-1,-1}^{-1}\Sigma_{-1,1},
\quad
\sigma^2=\Sigma_{11}-\Sigma_{1,-1}\Sigma_{-1,-1}^{-1}\Sigma_{-1,1}>0.
$$

For a jointly Gaussian vector, the residual is independent of the regressor, so $y=z^T\beta+\sigma e$ with $e\sim N(0,1)$ independent of $z$.

The [Square-root Lasso](../../../probability-and-statistics.md#square-root-lasso) minimizes

$$
\frac1{\sqrt n}\lVert X-Z\theta\rVert_2+\gamma\lVert\theta\rVert_1,
\qquad \gamma=\sqrt{\frac{2\log p}{n}}.
$$

At a nonzero residual $R$, its KKT condition is

$$
\frac{Z^TR}{\sqrt n\lVert R\rVert_2}=\gamma u,
\qquad\lVert u\rVert_\infty\leq1,
$$

which proves the required inequality.

Writing the response vector as $Y=f+\sigma e$, the reverse triangle inequality gives

$$
\left|\widehat\sigma-\sigma\frac{\lVert e\rVert_2}{\sqrt n}\right|
\leq\frac{\lVert\widehat f-f\rVert_2}{\sqrt n}=o_P(1).
$$

The [strong law of large numbers](../../../convergence-of-random-variables.md#strong-law-of-large-numbers) gives $\lVert e\rVert_2/\sqrt n\to_P1$, hence $\widehat\sigma\to_P\sigma$.

Under $X\perp\!\!\!\perp Y\mid Z$, Gaussianity makes $e$ independent of $(X,Z)$ and hence of $R$. Conditionally on $R$, $R^Te/\lVert R\rVert_2\sim N(0,1)$. The remaining numerator term obeys

$$
\frac{|R^TZ(\beta-\widehat\beta)|}{\lVert R\rVert_2}
\leq\frac{\lVert Z^TR\rVert_\infty}{\lVert R\rVert_2}
\lVert\widehat\beta-\beta\rVert_1
\leq\sqrt{2\log p}\,\lVert\widehat\beta-\beta\rVert_1=o_P(1).
$$

Combining this with $\widehat\sigma\to_P\sigma$ and [Slutsky theorem](../../../statistical-inference.md#slutsky-theorem) proves the standard-normal limit.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
