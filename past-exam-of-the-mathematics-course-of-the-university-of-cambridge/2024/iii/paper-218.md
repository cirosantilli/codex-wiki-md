# Paper 218

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_218.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_218.pdf)

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
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [i](#3/e/i)
      - [Solution](#3/e/i/solution)
    - [ii](#3/e/ii)
      - [Solution](#3/e/ii/solution)
    - [iii](#3/e/iii)
      - [Solution](#3/e/iii/solution)
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

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Write $Y_i$ for the colony count and $d_i$ for the dose on plate $i$. The first fit is the [Poisson regression](../../../statistical-modelling.md#poisson-regression)

$$
Y_i\mathrel{\perp\!\!\!\perp}Y_j\quad(i\ne j),
\qquad
Y_i\sim\operatorname{Pois}(\mu_i),
\qquad
\log\mu_i=\beta_0+\beta_1d_i.
$$

Thus its [log-likelihood](../../../statistical-modelling.md#log-likelihood) is

$$
\ell(\beta_0,\beta_1)
=\sum_{i=1}^{18}\left[y_i(\beta_0+\beta_1d_i)
-e^{\beta_0+\beta_1d_i}-\log(y_i!)\right].
$$

The [Poisson deviance](../../../statistical-modelling.md#poisson-deviance) relative to the saturated model is

$$
D=2\sum_{i=1}^{18}
\left\{y_i\log\frac{y_i}{\widehat\mu_i}
-(y_i-\widehat\mu_i)\right\},
$$

where a summand with $y_i=0$ uses $0\log0=0$.

At dose zero the fitted [expected value](../../../probability-theory.md#expected-value) is $e^{\widehat\beta_0}=e^{3.321995}\simeq27.72$ eradicated colonies. Increasing dose by one unit multiplies the fitted mean by $e^{\widehat\beta_1}=e^{0.0001901}\simeq1.000190$; for example, an increase of $100$ units multiplies it by about $1.0192$. The positive fitted effect is small and its displayed two-sided $p$-value, $0.105$, gives little evidence against a zero dose coefficient.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For the Poisson [variance function](../../../exponential-family.md#variance-function) $V(\mu)=\mu$, the code computes the [Pearson chi-squared statistic](../../../statistical-modelling.md#pearson-chi-squared-statistic)

$$
X_P^2=\sum_{i=1}^{18}\frac{(Y_i-\widehat\mu_i)^2}{\widehat\mu_i}
$$

and the [Pearson dispersion estimator](../../../statistical-modelling.md#pearson-dispersion-estimator)

$$
\widehat\phi=\frac{X_P^2}{18-2}=\frac{X_P^2}{16}.
$$

The first quantity measures [goodness of fit](../../../statistical-modelling.md#goodness-of-fit); the second estimates the [dispersion parameter](../../../exponential-family.md#dispersion-parameter), which equals one in a correctly specified [Poisson regression](../../../statistical-modelling.md#poisson-regression). A standard rough calculation substitutes the residual deviance for the Pearson statistic and gives

$$
\widehat\phi\simeq\frac{75.806}{16}=4.74.
$$

If the reported upper-tail probability $4.908651\times10^{-11}$ is inverted numerically, the actual Pearson statistic used by the code is about $82.93$, giving $\widehat\phi\simeq5.18$. Either calculation reveals severe [overdispersion](../../../exponential-family.md#overdispersion).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The Pearson [goodness-of-fit test](../../../statistical-modelling.md#goodness-of-fit-test) has null hypothesis that the independent counts follow the fitted [Poisson regression](../../../statistical-modelling.md#poisson-regression), in particular $\operatorname{Var}(Y_i\mid d_i)=\mu_i$, against the alternative that the model does not fit; in this setting the scientifically relevant direction is [overdispersion](../../../exponential-family.md#overdispersion), $\operatorname{Var}(Y_i\mid d_i)>\mu_i$. Under the null, $X_P^2$ is approximately [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) with $16$ degrees of freedom. Its tiny $p$-value decisively rejects the Poisson variance assumption.

The [negative binomial regression](../../../statistical-modelling.md#negative-binomial-regression) keeps the logarithmic mean model but allows $\operatorname{Var}(Y_i\mid d_i)=\mu_i+\mu_i^2/\theta$. It improves the residual deviance from $75.806$ to $18.011$, close to its $16$ residual degrees of freedom, and lowers the [Akaike information criterion](../../../statistical-modelling.md#akaike-information-criterion) from $172.34$ to $141.66$. Both comparisons strongly favour the negative-binomial fit, although its dose coefficient remains statistically insignificant.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The variance $\mu+\mu^2/\theta$ approaches the [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) variance $\mu$ when $\theta\to\infty$. Equivalently, with $\alpha=1/\theta\geq0$, the Poisson model is the boundary value $\alpha=0$. The usual [Wilks theorem](../../../statistical-inference.md#wilks-theorem) for a [likelihood-ratio test](../../../statistical-modelling.md#likelihood-ratio-test) assumes that the null parameter is an interior point of a smooth parameter space, so comparing the statistic with an ordinary $\chi_1^2$ law is invalid here.

A valid [parametric bootstrap](../../../statistical-modelling.md#parametric-bootstrap) proceeds as follows. First fit the null Poisson model and retain its fitted means $\widehat\mu_i$. For each bootstrap repetition $b=1,\ldots,B$, independently simulate

$$
Y_i^{(b)}\sim\operatorname{Pois}(\widehat\mu_i),
$$

using the original doses, refit both the Poisson and negative-binomial models to that simulated data, and calculate

$$
T_b=2\left\{\ell_{NB}^{(b)}-\ell_P^{(b)}\right\}.
$$

For the observations calculate the analogous $T_{obs}$. The bootstrap $p$-value

$$
\widehat p=\frac{1+\sum_{b=1}^B\mathbf1_{\{T_b\geq T_{obs}\}}}{B+1}
$$

uses the null distribution with its boundary and finite-sample fitting behaviour automatically reproduced. A large $B$ controls the [Monte Carlo error](../../../probability-and-statistics.md#monte-carlo-error) of this estimate.

## 2

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Because the columns of the [design matrix](../../../linear-regression.md#design-matrix) are centred, [ridge regression](../../../linear-regression.md#ridge-regression) with an unpenalized intercept solves

$$
(\widehat\alpha_\lambda,\widehat\beta_\lambda)
=\underset{\alpha\in\mathbb R,\,\beta\in\mathbb R^p}{\operatorname{argmin}}
\left\{\|Y-\alpha\mathbf1-X\beta\|_2^2
+\lambda\|\beta\|_2^2\right\}.
$$

The [normal equations](../../../statistical-modelling.md#normal-equation) give, for $\lambda>0$,

$$
\widehat\alpha_\lambda=\overline Y,
\qquad
\widehat\beta_\lambda=(X^TX+\lambda I_p)^{-1}X^T(Y-\overline Y\mathbf1)
=(X^TX+\lambda I_p)^{-1}X^TY.
$$

The [fitted values](../../../linear-regression.md#fitted-values) are consequently

$$
\widehat Y_\lambda
=\overline Y\mathbf1+X(X^TX+\lambda I_p)^{-1}X^TY.
$$

If the objective is normalized by $n$, the same formulas hold after replacing $\lambda$ by $n\lambda$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Choose $\lambda$ to minimize an estimate of out-of-sample [mean squared prediction error](../../../statistical-learning.md#mean-squared-prediction-error), commonly [K-fold cross-validation](../../../statistical-learning.md#k-fold-cross-validation) or a separate [validation set](../../../statistical-learning.md#validation-set). As $\lambda$ increases, the coefficient vector is shrunk toward zero. This generally increases [bias of an estimator](../../../statistical-modelling.md#bias-of-an-estimator) but decreases [variance of an estimator](../../../statistical-modelling.md#variance-of-an-estimator); the minimizing value balances the two contributions in the [bias-variance tradeoff](../../../statistical-modelling.md#bias-variance-tradeoff). The independent test set in the question can assess the final choice, but repeatedly selecting $\lambda$ on that same set would cause [data leakage](../../../statistical-learning.md#data-leakage).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

[Coordinate descent](../../../convex-optimization.md#coordinate-descent) cycles through the intercept and coefficient coordinates, minimizing the convex ridge objective in one coordinate while holding the others fixed. Given current coefficients, update

$$
\alpha\leftarrow\frac1n\sum_{i=1}^n
\left(Y_i-\sum_{k=1}^pX_{ik}\beta_k\right).
$$

For coordinate $j$, form the partial residual

$$
r^{(j)}=Y-\alpha\mathbf1-\sum_{k\ne j}X_k\beta_k
$$

and update it by the exact one-dimensional minimizer

$$
\beta_j\leftarrow
\frac{X_j^Tr^{(j)}}{X_j^TX_j+\lambda}.
$$

Repeated sweeps converge to the unique fitted value because the objective is a [convex function](../../../real-analysis.md#convex-function); with $\lambda>0$ it is strictly convex in $\beta$.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The solid curve is the [test error](../../../statistical-learning.md#test-error)

$$
\frac1n\|Y^*-\widehat Y_\lambda\|_2^2,
$$

and the dashed curve is the [training error](../../../statistical-learning.md#training-error) $n^{-1}\|Y-\widehat Y_\lambda\|_2^2$. As the horizontal coordinate tends to $+\infty$, $\lambda\to\infty$, so every penalized slope tends to zero and $\widehat Y_\lambda\to\overline Y\mathbf1$. The two limits are therefore

$$
\frac1n\|Y^*-\overline Y\mathbf1\|_2^2
\quad\hbox{and}\quad
\frac1n\|Y-\overline Y\mathbf1\|_2^2,
$$

respectively.

As the horizontal coordinate tends to $-\infty$, $\lambda\downarrow0$ and the fit approaches the [ordinary least squares](../../../statistical-modelling.md#ordinary-least-squares) fit $H_0Y$. Hence the solid curve tends to $n^{-1}\|Y^*-H_0Y\|_2^2$, which the plot shows is approximately $0.4$.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Put $f=(f(x_1),\ldots,f(x_n))^T$, so $Y=f+\varepsilon$ and $Y^*=f+\varepsilon^*$ with independent noise vectors having [covariance matrix](../../../variance.md#covariance-matrix) $I_n$. For any deterministic [linear smoother](../../../linear-regression.md#linear-smoother) $H$,

$$
\mathbb E\|Y-HY\|_2^2
=\|(I-H)f\|_2^2
+\operatorname{tr}\!\left((I-H)^T(I-H)\right),
$$

whereas independence gives

$$
\mathbb E\|Y^*-HY\|_2^2
=\|(I-H)f\|_2^2+n+\operatorname{tr}(H^TH).
$$

Expanding the first trace shows that the second expression exceeds the first by $2\operatorname{tr}(H)$, proving the identity.

For ridge regression,

$$
H_\lambda=\frac1n\mathbf1\mathbf1^T
+X(X^TX+\lambda I_p)^{-1}X^T.
$$

Its [effective degrees of freedom](../../../linear-regression.md#effective-degrees-of-freedom) are $\operatorname{tr}(H_\lambda)$. Thus training error is optimistically biased for independent-copy prediction error by $2\operatorname{tr}(H_\lambda)/n$. The graph exhibits exactly this effect: the dashed training curve keeps falling as $\lambda$ decreases, while the solid test curve eventually rises through [overfitting](../../../statistical-learning.md#overfitting).

## 3

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The classification form of [CART](../../../statistical-learning.md#classification-and-regression-tree) starts with the root rectangle $R=[0,1]^2$. For any current region $A$, let $N(A)=\#\{i:X_i\in A\}$ and let

$$
\widehat p(A)=\frac{\#\{i:X_i\in A,\,Y_i=\text{circle}\}}{N(A)},
\qquad
G(A)=\widehat p(A)(1-\widehat p(A))
$$

be its empirical class proportion and [Gini impurity](../../../statistical-learning.md#gini-impurity). A candidate axis-aligned split $X_j\leq s$ partitions $R$ into $U$ and $V$. Its impurity change is

$$
Q=\frac{N(U)}{N(R)}G(U)
+\frac{N(V)}{N(R)}G(V)-G(R).
$$

Among all coordinates and thresholds between consecutive observed coordinates, CART chooses a split minimizing $Q$, then applies the same [recursive partitioning](../../../statistical-learning.md#recursive-partitioning) independently to the children until a stopping rule is met. Each terminal region predicts its majority class. Pruning may then select a smaller subtree by penalizing the number of leaves.

For the resulting classifier $\widehat C$, the [training error](../../../statistical-learning.md#training-error) is

$$
\widehat R_{train}=\frac19\sum_{i=1}^9
\mathbf1_{\{\widehat C(X_i)\ne Y_i\}},
$$

while its [prediction error](../../../statistical-learning.md#prediction-error) is $R(\widehat C)=\mathbb P\{\widehat C(X_{new})\ne Y_{new}\}$ for an independent observation drawn from the target population.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $w=N(U)/N(R)$, so $1-w=N(V)/N(R)$. Since class counts add,

$$
\widehat p(R)=w\widehat p(U)+(1-w)\widehat p(V).
$$

The function $g(p)=p(1-p)$ is [concave function](../../../real-analysis.md#concave-function) on $[0,1]$. [Jensen inequality](../../../real-analysis.md#jensen-s-inequality) therefore gives

$$
G(R)=g(\widehat p(R))
\geq wg(\widehat p(U))+(1-w)g(\widehat p(V)),
$$

which is precisely $Q\leq0$. Thus an axis-aligned split cannot increase the weighted empirical Gini impurity.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

A [random forest](../../../statistical-learning.md#random-forest) fits each of its $500$ classification trees to an independent [bootstrap sample](../../../statistical-modelling.md#bootstrap-sample) of the nine observations. At each node it draws `mtry=2` candidate coordinates; because the data have exactly two coordinates, both are available, and a CART impurity calculation chooses the split. The trees are grown deeply without ordinary cost-complexity pruning, and their [majority vote](../../../statistical-learning.md#majority-vote) is the forest prediction.

R reports an [out-of-bag error estimate](../../../statistical-learning.md#out-of-bag-error): an observation is predicted only by trees whose bootstrap samples omitted it. The [confusion matrix](../../../statistical-learning.md#confusion-matrix) says that class 1 has three correct and three incorrect out-of-bag predictions, while class 2 has one correct and two incorrect predictions. Hence the total out-of-bag error is $5/9$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The loop performs [Leave-one-out cross-validation](../../../statistical-learning.md#leave-one-out-cross-validation): for each $i$ it fits a forest to the other eight observations, tests it on observation $i$, and averages the nine zero-one losses. A random forest's [out-of-bag error estimate](../../../statistical-learning.md#out-of-bag-error) approximates the same held-out prediction error from one fit, because each tree automatically omits roughly a proportion $e^{-1}$ of the observations in its [bootstrap sample](../../../statistical-modelling.md#bootstrap-sample).

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/i">i</h4>

↑ **Parent:** [E](#3/e)

<h5 id="3/e/i/solution">Solution</h5>

↑ **Parent:** [I](#3/e/i)

The [one-nearest-neighbour classification](../../../statistical-learning.md#one-nearest-neighbour-classification) boundary consists of the portions of the [Voronoi diagram](../../../geometry-and-topology.md#voronoi-diagram) separating cells whose observed labels differ. For these nine grid points it forms diagonal and vertical or horizontal perpendicular-bisector segments around the three triangular observations. Every training point is its own nearest neighbour, so, absent a distance tie convention that excludes the query itself, its training error is zero.

<h4 id="3/e/ii">ii</h4>

↑ **Parent:** [E](#3/e)

<h5 id="3/e/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/e/ii)

An unpruned maximal [CART](../../../statistical-learning.md#classification-and-regression-tree) classifier repeatedly cuts with vertical or horizontal lines until every terminal rectangle is pure or contains observations that cannot be separated by an axis-aligned split. Here the distinct grid points can be isolated into pure rectangles, producing a step-shaped, axis-aligned [decision boundary](../../../statistical-learning.md#decision-boundary) and zero training error.

<h4 id="3/e/iii">iii</h4>

↑ **Parent:** [E](#3/e)

<h5 id="3/e/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/e/iii)

The [random forest](../../../statistical-learning.md#random-forest) boundary is the majority vote of many bootstrap-grown axis-aligned trees. It remains piecewise axis-aligned but averages away many unstable individual cuts, so one should sketch a less extreme boundary enclosing regions supported repeatedly by the triangular points. Its resubstitution training error is typically small and can be zero, but bootstrap omission and voting mean that zero is not guaranteed. The relevant built-in estimate is instead the out-of-bag error, which the output gives as $5/9$; this large value reflects the tiny sample and unstable labels near the class boundary.

## 4

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For $X_i^*=(1,X_i^T)^T$ and $\gamma=(\gamma_0,\beta^T)^T$, a linear [support vector machine](../../../statistical-learning.md#support-vector-machine) predicts

$$
\widehat C_\gamma(x)=\operatorname{sign}(\gamma_0+x^T\beta).
$$

One penalized formulation minimizes empirical [hinge loss](../../../foundations-of-mathematics.md#hinge-loss) plus a squared [Euclidean norm](../../../functional-analysis.md#euclidean-norm) penalty:

$$
\widehat\gamma\in\underset{\gamma\in\mathbb R^{p+1}}{\operatorname{argmin}}
\left\{
\sum_{i=1}^n\max(0,1-Y_iX_i^{*T}\gamma)
+\lambda\|\gamma\|_2^2
\right\},
\qquad \lambda>0.
$$

Conventions often leave the intercept unpenalized, replacing $\|\gamma\|_2^2$ by $\|\beta\|_2^2$; this does not change the role of the two terms.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

A [separating hyperplane](../../../statistical-learning.md#separating-hyperplane) for signed data satisfies $Y_i(\gamma_0+X_i^T\beta)>0$ for every $i$; its geometric set is $\{x:\gamma_0+x^T\beta=0\}$. The plot marks three [support vectors](../../../statistical-learning.md#support-vector). At the shown fit they lie on the two [support-vector-machine margin boundaries](../../../statistical-learning.md#support-vector-machine-margin-boundaries), so their signed functional margins satisfy

$$
Y_iX_i^{*T}\widehat\gamma=1.
$$

The solid line is the decision hyperplane $X^{*T}\widehat\gamma=0$, while the dashed parallel lines are $X^{*T}\widehat\gamma=1$ and $X^{*T}\widehat\gamma=-1$.

If $\lambda=0$, every parameter vector with all margins at least one has zero hinge loss. Scaling or changing a separating vector can therefore give another minimizer, so the objective need not select the displayed maximum-margin direction or the same three lines. Positive quadratic regularization selects a finite, minimum-norm compromise.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

This is a normalized [perceptron algorithm](../../../statistical-learning.md#perceptron). Because $\|Z_i\|_2=1$, an update on a misclassified point obeys

$$
\begin{aligned}
\|\gamma^{(m+1)}-\widehat\gamma\|_2^2
&=\|\gamma^{(m)}-\widehat\gamma+Y_iZ_i\|_2^2\\
&=\|\gamma^{(m)}-\widehat\gamma\|_2^2+1
+2Y_iZ_i^T\gamma^{(m)}-2Y_iZ_i^T\widehat\gamma\\
&\leq\|\gamma^{(m)}-\widehat\gamma\|_2^2+1+0-2\\
&=\|\gamma^{(m)}-\widehat\gamma\|_2^2-1.
\end{aligned}
$$

Here the two inequalities use the update condition $Y_iZ_i^T\gamma^{(m)}\leq0$ and the assumed unit margin $Y_iZ_i^T\widehat\gamma\geq1$. A squared distance cannot become negative, so there can be at most $\|\gamma^{(0)}-\widehat\gamma\|_2^2$ updates. The algorithm then returns a vector that correctly separates every training point. The estimate $\widehat\gamma$ is the comparison vector for the proof; without an additional uniqueness condition the returned separator need not equal that particular vector.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

A binary [logistic regression](../../../statistical-modelling.md#logistic-regression) sets

$$
\mathbb P(Y=1\mid X=x)
=\frac{1}{1+e^{-(\gamma_0+x^T\beta)}}
$$

and classifies by the sign of $\gamma_0+x^T\beta$. Its unpenalized [maximum-likelihood estimator](../../../statistical-modelling.md#maximum-likelihood-estimator) minimizes the empirical [logistic loss](../../../statistical-modelling.md#logistic-loss)

$$
L(\gamma)=\sum_{i=1}^n
\log\left(1+e^{-Y_iX_i^{*T}\gamma}\right).
$$

The plotted data are [complete separation](../../../statistical-modelling.md#complete-separation) data: there is a vector $v$ with every signed margin $Y_iX_i^{*T}v>0$. For every finite $c>0$, increasing $c$ strictly decreases each term of $L(cv)$, and $L(cv)\to0$ as $c\to\infty$. No finite parameter attains zero, so the unpenalized optimization has no solution.

Adding an $L^2$ penalty $\lambda\|\gamma\|_2^2$ with $\lambda>0$, constraining $\|\gamma\|_2$, or using a finite stopping rule makes the problem attain a finite approximate solution. The penalized option is preferable because [cross-validation](../../../statistical-learning.md#cross-validation) can select the strength of [regularization](../../../statistical-learning.md#regularization).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
