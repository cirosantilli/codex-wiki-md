# Paper 218

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_218.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_218.pdf)

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
  - [e](#1/e)
    - [i](#1/e/i)
      - [Solution](#1/e/i/solution)
    - [ii](#1/e/ii)
      - [Solution](#1/e/ii/solution)
  - [f](#1/f)
    - [Solution](#1/f/solution)
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
  - [e](#4/e)
    - [Solution](#4/e/solution)
  - [f](#4/f)
    - [Solution](#4/f/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [i](#5/d/i)
      - [Solution](#5/d/i/solution)
    - [ii](#5/d/ii)
      - [Solution](#5/d/ii/solution)
  - [e](#5/e)
    - [Solution](#5/e/solution)

## 1

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The first fit is a [Poisson regression](../../../statistical-modelling.md#poisson-regression) with independent responses

$$
Y_i\sim\operatorname{Poisson}(\mu_i),
\qquad
\log\mu_i=\beta_0+\beta_1x_{i1}+\beta_2x_{i2}.
$$

The fitted intercept gives $e^{3.8879}$ expected visitors when spending on both services is zero. Holding advert2 fixed, increasing advert1 by one unit, namely one hundred pounds, multiplies the expected visitor count by $e^{0.1923}\simeq1.212$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The second fit is a [Quasi-Poisson regression](../../../statistical-modelling.md#quasi-poisson-regression). It retains the [logarithmic link function](../../../statistical-modelling.md#logarithmic-link-function) and mean model

$$
\log\mu_i=\beta_0+\beta_1x_{i1}+\beta_2x_{i2},
$$

but assumes only $\operatorname{Var}(Y_i)=\phi\mu_i$ for an unknown [dispersion parameter](../../../exponential-family.md#dispersion-parameter) $\phi$, rather than a complete [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The quasi-Poisson standard errors are the Poisson standard errors multiplied by $\sqrt{\widehat\phi}$, and the Pearson estimator divides the [Pearson chi-squared statistic](../../../statistical-modelling.md#pearson-chi-squared-statistic) by the residual degrees of freedom $40-3=37$. Therefore the requested sum of squared Pearson residuals is

$$
37\widehat\phi
=37\left(\frac{0.1305}{0.1020}\right)^2,
$$

up to the rounding in the printed standard errors.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The third fit is a [negative binomial regression](../../../statistical-modelling.md#negative-binomial-regression). The Poisson model is obtained at the boundary where the negative-binomial overdispersion tends to zero, so the [likelihood-ratio test](../../../statistical-modelling.md#likelihood-ratio-test) has the asymptotic null distribution $\tfrac12\chi_0^2+\tfrac12\chi_1^2$. Since model3 has one additional parameter,

$$
D=2(\ell_3-\ell_1)
=\operatorname{AIC}_1-\operatorname{AIC}_3+2.
$$

The supplied output gives $\mathbb P(\chi_1^2\geq D)=0.04608555$, and hence the boundary-corrected p-value is

$$
\boxed{p=\frac12(0.04608555)=0.023042775.}
$$

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/i">i</h4>

↑ **Parent:** [E](#1/e)

<h5 id="1/e/i/solution">Solution</h5>

↑ **Parent:** [I](#1/e/i)

The stated mean and variance identify $\lambda_i$ as a [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution) with shape $\nu_i$ and scale $\alpha_i$. A [Poisson-gamma mixture](../../../discrete-probability-distribution.md#poisson-gamma-mixture) is negative binomial, with

$$
\mathbb E Y_i=\mu_i=\alpha_i\nu_i,
\qquad
\operatorname{Var}(Y_i)=\mu_i+\frac{\mu_i^2}{\nu_i}.
$$

When $\nu_i=\nu$, this is exactly the constant-shape variance model fitted by the negative binomial regression, so the most appropriate printed p-value is $0.0798$ from model3.

<h4 id="1/e/ii">ii</h4>

↑ **Parent:** [E](#1/e)

<h5 id="1/e/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/e/ii)

When $\alpha_i=\alpha$, the [law of total variance](../../../probability-theory.md#law-of-total-variance) gives

$$
\operatorname{Var}(Y_i)=\mu_i+\alpha\mu_i=(1+\alpha)\mu_i.
$$

This is the quasi-Poisson mean-variance relation with constant dispersion, so the most appropriate printed p-value is $0.0982$ from model2.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

Among all depth-one [regression tree](../../../foundations-of-mathematics.md#regression-tree) splits, the best split separates the second observation from the first and third by cutting advert1 between $0.89$ and $1.13$. The test point with advert1 equal to zero reaches the leaf containing responses $60$ and $53$, so the output is their [arithmetic mean](../../../arithmetic.md#arithmetic-mean),

$$
\widehat y=\frac{60+53}{2}=56.5.
$$

This [decision stump](../../../foundations-of-mathematics.md#decision-stump) makes a piecewise-constant prediction far outside the observed predictor range and cannot extrapolate the spending trend towards the origin. Its shallow structure and leaf averaging keep its [variance of an estimator](../../../statistical-modelling.md#variance-of-an-estimator) modest, while that extrapolation failure can produce substantial [bias of an estimator](../../../statistical-modelling.md#bias-of-an-estimator).

## 2

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [ridge regression](../../../linear-regression.md#ridge-regression) estimator is the elastic net at $\alpha=0$, while the [Lasso regression](../../../probability-and-statistics.md#lasso) estimator is the elastic net at $\alpha=1$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Put $z=\widehat\beta_{\mathrm{OLS}}=X^TY/n$. Under $X^TX=nI_p$, the objective separates by coordinates. Completing the square and applying the [soft-thresholding operator](../../../probability-and-statistics.md#soft-thresholding) $S(u,t)=\operatorname{sign}(u)(|u|-t)_+$ gives

$$
(\widehat\beta_{\alpha,\lambda})_j
=\frac{S(z_j,\lambda\alpha)}{1+\lambda(1-\alpha)}.
$$

For a fixed $z_j$, its magnitude lies between the ridge endpoint $|z_j|/(1+\lambda)$ and the lasso endpoint $(|z_j|-\lambda)_+$; this follows directly on the two intervals $\lambda\alpha\geq|z_j|$ and $\lambda\alpha<|z_j|$ by cross-multiplication. Thus the stated endpoint inequality holds.

For $alpha>0$ and $z_j\ne0$, the coordinate first vanishes when the soft threshold reaches $|z_j|$, so

$$
(\lambda_α^*)_j=\frac{|z_j|}{\alpha}.
$$

This is strictly decreasing in $\alpha$, and it diverges to infinity as $\alpha\downarrow0$. This agrees with the fact that pure ridge shrinkage does not set a nonzero coordinate exactly to zero at any finite penalty.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Writing the horizontal coordinate as $u=\log\lambda$, so that $\lambda=e^u$, the two coefficient paths at $\alpha=1/2$ are

$$
\beta_1(u)=\frac{(1.41-e^u/2)_+}{1+e^u/2},
\qquad
\beta_2(u)=-\frac{(0.41-e^u/2)_+}{1+e^u/2}.
$$

Equivalently, as functions of $\lambda$, replace every $e^u$ by $\lambda$. The paths reach zero at $lambda=2.82$ and $lambda=0.82$, respectively.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Let $z=\widehat\beta_{\mathrm{OLS}}$ and $G=X^TX/n=\begin{pmatrix}1&\rho\\\rho&1\end{pmatrix}$. While both lasso coordinates are positive, the [Karush-Kuhn-Tucker conditions](../../../mathematical-optimization.md#karush-kuhn-tucker-conditions) give

$$
G(\widehat\beta-z)+\lambda\binom11=0,
\qquad
\widehat\beta=z-\frac{\lambda}{1+\rho}\binom11.
$$

Hence

$$
\lambda^\dagger=(1+\rho)\min(z_1,z_2).
$$

Assume without loss of generality that $z_1\leq z_2$. After the first coordinate vanishes, the second remains active until $lambda=z_2+\rho z_1$. The zero vector satisfies the KKT conditions exactly when $lambda\geq\lVert Gz\rVert_\infty$; for $z_1\leq z_2$ and $-1<\rho<1$, this norm is $z_2+\rho z_1$. Therefore

$$
\lambda^\ddagger=\max(z_1,z_2)+\rho\min(z_1,z_2),
$$

and

$$
\lambda^\ddagger-\lambda^\dagger
=\max(z_1,z_2)-\min(z_1,z_2)=|z_1-z_2|,
$$

which is independent of $\rho$.

## 3

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [conditional class probability](../../../statistical-learning.md#conditional-class-probability) is $p_k(x)=\mathbb P(Y=k\mid X=x)$. A [Bayes classifier](../../../statistical-inference.md#bayes-classifier) chooses

$$
h^*(x)\in\operatorname*{argmax}_{1\leq k\leq K}p_k(x),
$$

and its [Bayes risk](../../../statistical-inference.md#bayes-risk) is

$$
R_{\mathrm{Bayes}}=R(h^*)
=\mathbb E\left[1-\max_kp_k(X)\right].
$$

A sequence of classifiers is [consistent](../../../statistical-learning.md#risk-consistency) when $R(h_n)\to R_{\mathrm{Bayes}}$ as $n\to\infty$, with convergence interpreted in probability or in expectation according to whether the training sample is conditioned upon.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The $L$-nearest-neighbour classifier finds the $L$ training predictors nearest to $x$ and returns the majority class among their labels. Increasing $L$ averages more labels and reduces [variance of an estimator](../../../statistical-modelling.md#variance-of-an-estimator), but uses observations farther from $x$ and therefore increases [bias of an estimator](../../../statistical-modelling.md#bias-of-an-estimator); decreasing $L$ reverses this [bias-variance tradeoff](../../../statistical-modelling.md#bias-variance-tradeoff).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For two classes, write $m(x)=\min\{p_1(x),p_2(x)\}$, the conditional Bayes error. The nearest-neighbour label and the test label become conditionally independent draws from the same local class distribution, so the limiting conditional error of [one-nearest-neighbour classification](../../../statistical-learning.md#one-nearest-neighbour-classification) is

$$
2p_1(x)p_2(x)=2m(x)(1-m(x)).
$$

The assumption gives $c\leq m(x)\leq1/2-c$. Its excess over the conditional Bayes error is

$$
2m(1-m)-m=m(1-2m)\geq2c^2>0.
$$

After taking expectations, the limiting risk remains at least $2c^2$ above the Bayes risk, so one-nearest-neighbour classification is not consistent.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The limiting conditional error of one-nearest-neighbour classification is $1-\sum_kp_k(x)^2$. Put $M=\max_kp_k(x)$ and $r=1-M$. By the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality), the other $K-1$ probabilities satisfy

$$
\sum_{k:p_k\ne M}p_k^2\geq\frac{r^2}{K-1}.
$$

Consequently

$$
1-\sum_kp_k^2
\leq1-(1-r)^2-\frac{r^2}{K-1}
=2r-\frac K{K-1}r^2.
$$

Now $\mathbb Er=R_{\mathrm{Bayes}}$, and [Jensen inequality](../../../real-analysis.md#jensen-s-inequality) gives $\mathbb Er^2\geq(\mathbb Er)^2$. Taking expectations proves

$$
\boxed{\lim_{n\to\infty}R(h_n^{\mathrm{1NN}})
\leq2R_{\mathrm{Bayes}}-\frac K{K-1}R_{\mathrm{Bayes}}^2.}
$$

## 4

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Encode the two classes by the standard basis vectors of $\mathbb R^2$. With [rectified linear unit](../../../statistical-learning.md#rectified-linear-unit) $r(t)=\max(t,0)$ applied coordinatewise and [softmax function](../../../statistical-learning.md#softmax-function) $s_j(z)=e^{z_j}/\sum_ke^{z_k}$, the fitted [feedforward neural network](../../../statistical-learning.md#feedforward-neural-network) is

$$
\widehat p(x)=s\!\left(W_3r\!\left(W_2r(W_1x+b_1)+b_2\right)+b_3\right),
$$

where $W_1\in\mathbb R^{40\times40}$, $b_1\in\mathbb R^{40}$, $W_2\in\mathbb R^{20\times40}$, $b_2\in\mathbb R^{20}$, $W_3\in\mathbb R^{2\times20}$, and $b_3\in\mathbb R^2$. The number of trainable parameters is

$$
\boxed{40\cdot40+40+20\cdot40+20+2\cdot20+2=2502.}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Training minimizes the empirical [categorical cross-entropy loss](../../../statistical-learning.md#categorical-cross-entropy-loss)

$$
L(\theta)=-\frac1{10000}\sum_{i=1}^{10000}\sum_{k=1}^2y_{ik}\log\widehat p_k(x_i;\theta)
$$

by [stochastic gradient descent](../../../numerical-analysis.md#stochastic-gradient-descent). The independent validation set monitors generalization, while the small fixed number of epochs limits how long the network can fit training noise; using validation loss for [early stopping](../../../statistical-learning.md#early-stopping) would make this safeguard explicit. A forward pass computes all layer activations, class probabilities, and the mini-batch loss. There are $10000/2=5000$ training mini-batches per epoch and hence $5\cdot5000=25000$ training forward passes, in addition to validation evaluation after each epoch.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The usual [Akaike information criterion](../../../statistical-modelling.md#akaike-information-criterion) correction assumes a regular maximum-likelihood fit with a meaningful fixed parameter dimension. Here stochastic optimization stopped after five epochs need not attain the maximum likelihood estimator, and neural-network symmetries, inactive units, and heavy overparameterization make the raw count $2502$ a poor effective dimension. Either failure invalidates a direct AIC comparison with an ordinary [logistic regression](../../../statistical-modelling.md#logistic-regression).

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The proposed function $g(\eta)=\eta\Phi(\eta)$ is the [Gaussian error linear unit](../../../statistical-learning.md#gaussian-error-linear-unit). Unlike ReLU, it is smooth at zero and has a nonzero gradient on much of the negative half-line, reducing dead hidden units and making gradient optimization smoother. It is less computationally convenient because evaluating the [standard normal cumulative distribution function](../../../probability-theory.md#standard-normal-distribution-function) is costlier than taking a maximum, and it does not produce ReLU's exact sparse zero activations.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

The intended quantity is the [Leave-one-out cross-validation](../../../statistical-learning.md#leave-one-out-cross-validation) error

$$
\operatorname{LOOCV}
=\frac1n\sum_{i=1}^n
\ell\!\left(\widehat h^{(-i)}(X_i),Y_i\right),
$$

where $\widehat h^{(-i)}$ is trained without observation $i$ and the loss is the zero-one misclassification loss. Computing it literally requires fitting $10000$ neural networks, which is prohibitively expensive.

<h3 id="4/f">f</h3>

↑ **Parent:** [4](#4)

<h4 id="4/f/solution">Solution</h4>

↑ **Parent:** [F](#4/f)

The assignment `nn.model.i <- nn.model` does not construct a fresh untrained Keras model: it aliases an object whose weights were already fitted using every training observation, including the nominally held-out one, and repeated fits continue mutating those weights. This [data leakage](../../../statistical-learning.md#data-leakage) makes metric2 severely optimistic. Moreover, random leave-one-out validation among reviews from 2012--2025 does not reproduce the [dataset shift](../../../statistical-learning.md#dataset-shift) to new recent reviews that metric1 measures.

## 5

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Model1 is the [simple linear regression](../../../linear-regression.md#simple-linear-regression)

$$
Y_{ij}=\alpha+\beta X_{ij}+\varepsilon_{ij},
\qquad
\varepsilon_{ij}\stackrel{\mathrm{iid}}\sim N(0,\tau^2).
$$

Model2 is a [random-intercept linear mixed model](../../../statistical-modelling.md#random-intercept-linear-mixed-model)

$$
Y_{ij}=\alpha+\beta X_{ij}+b_i+\varepsilon_{ij},
\qquad
b_i\stackrel{\mathrm{iid}}\sim N(0,\sigma^2),
\quad
\varepsilon_{ij}\stackrel{\mathrm{iid}}\sim N(0,\tau^2),
$$

with the random intercepts and errors mutually independent.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Repeated measurements from one person can share persistent unobserved spending tendencies, violating model1's independent-error assumption and shifting that person's baseline. Model2 represents this [clustered data](../../../statistical-modelling.md#clustered-data) through a common random intercept $b_i$, which induces within-person covariance $\operatorname{Cov}(Y_{ij},Y_{ik}\mid X)=\sigma^2$ for $j\ne k$.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

The residual deviance of a Gaussian GLM is its [residual sum of squares](../../../linear-regression.md#residual-sum-of-squares), $154.30$. Thus the empirical training error for squared-error loss is

$$
\frac1{100}\sum_{i,j}(Y_{ij}-\widehat Y_{ij})^2
=\frac{154.30}{100}=1.543.
$$

If training error is defined as the unnormalized total loss, its value is $154.30$.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/i">i</h4>

↑ **Parent:** [D](#5/d)

<h5 id="5/d/i/solution">Solution</h5>

↑ **Parent:** [I](#5/d/i)

The first column of the model matrix is the all-ones intercept column. Hence $A_{11}=\sum_{i,j}1=100$.

<h4 id="5/d/ii">ii</h4>

↑ **Parent:** [D](#5/d)

<h5 id="5/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/d/ii)

The second cross-product entry is $A_{12}=\sum_{i,j}X_{ij}$. Regressing earned on the ten person indicators without an intercept makes $(g_x)_i$ the mean of that person's ten earned values. Therefore

$$
\boxed{\sum_i(g_x)_i=\frac1{10}\sum_{i,j}X_{ij}=0.1A_{12}.}
$$

<h3 id="5/e">e</h3>

↑ **Parent:** [5](#5)

<h4 id="5/e/solution">Solution</h4>

↑ **Parent:** [E](#5/e)

Let $q=(\alpha,\beta)^T$, let

$$
A=\begin{pmatrix}100&562.600\\562.600&3331.778\end{pmatrix},
\qquad
\widehat q_0=\binom{1.68782}{0.54218},
$$

and recover the sufficient cross-products from the model1 normal equations by setting $c=A\widehat q_0$ and $s=154.30+\widehat q_0^TA\widehat q_0$. Then

$$
S(q)=s-2q^Tc+q^TAq
$$

is the total squared residual about the fixed line. The squared sum of the ten residuals within each person, summed across people, is

$$
B(q)=100\left(244.1738-2\alpha(47.381)-2\beta(274.898)
+10\alpha^2+2\alpha\beta(56.26)+\beta^2(332.2809)\right).
$$

For one person's ten observations, the marginal covariance matrix is $\tau^2I_{10}+\sigma^2\mathbf1\mathbf1^T$. The [matrix determinant lemma](../../../linear-algebra.md#matrix-determinant-lemma) and [Sherman–Morrison formula](../../../linear-algebra.md#sherman-morrison-formula) therefore give, up to an additive constant, twice the negative marginal log-likelihood

$$
\omega(\alpha,\beta,\sigma,\tau)
=10\left(9\log\tau^2+\log(\tau^2+10\sigma^2)\right)
+\frac{S(q)}{\tau^2}
-\frac{\sigma^2B(q)}{\tau^2(\tau^2+10\sigma^2)}.
$$

Because the model was fitted with `REML = FALSE`, it minimizes this ordinary marginal maximum-likelihood objective. Thus $(V1,V2,V3,V4)$ belongs to the stated argmin over $alpha,\beta\in\mathbb R$ and $sigma,\tau>0$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
