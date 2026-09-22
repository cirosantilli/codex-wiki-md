# Paper 218

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20218.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20218.pdf)

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
    - [Solution](#1/e/solution)
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
  - [f](#2/f)
    - [Solution](#2/f/solution)
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
    - [Solution](#3/e/solution)
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
  - [g](#4/g)
    - [Solution](#4/g/solution)
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

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Expanding the exponent of the [Inverse Gaussian distribution](../../../exponential-family.md#inverse-gaussian-distribution) gives

$$
-\frac{\lambda(y-\mu)^2}{2\mu^2y}
=\lambda\left(-\frac{y}{2\mu^2}+\frac1\mu-\frac1{2y}\right).
$$

Thus the [exponential dispersion family](../../../exponential-family.md#exponential-dispersion-model) representation

$$
f(y;\theta,\phi)=a(y,\phi)
\exp\left\{\frac{y\theta-K(\theta)}\phi\right\}
$$

has

$$
\theta=-\frac1{2\mu^2},\qquad
K(\theta)=-\sqrt{-2\theta},\qquad
\phi=\frac1\lambda,
$$

and

$$
a(y,\phi)=\frac1{\sqrt{2\pi\phi y^3}}
\exp\left(-\frac1{2\phi y}\right).
$$

The standard cumulant identities yield

$$
\mathbb EY=K'(\theta)=\mu,qquad
\operatorname{Var}(Y)=\phi K''(\theta)=\frac{\mu^3}{\lambda}.
$$

**Hence the [variance function](../../../exponential-family.md#variance-function) is $V(\mu)=\mu^3$, and the [canonical link function](../../../statistical-modelling.md#canonical-link-function) is $g(\mu)=\theta(\mu)=-1/(2\mu^2)$.**

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Writing $d_i$ for difficulty, model1 assumes independent responses

$$
Y_i\sim\operatorname{IG}(\mu_i,\lambda),
\qquad
\frac1{\mu_i^2}=\beta_0+\beta_1d_i,
$$

with common dispersion. The estimates are $\widehat\beta_0=9.0827$ and $\widehat\beta_1=-1.4323$.

One extra difficulty level decreases the fitted inverse squared mean response time by $1.4323$. Since $\mu=(\beta_0+\beta_1d)^{-1/2}$, this means that fitted mean response time increases with difficulty. The negative coefficient is therefore unsurprising; its sign looks counterintuitive only if the inverse-squared [link function](../../../statistical-modelling.md#link-function) is ignored. The independence assumption is questionable because every subject contributes eight repeated responses.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The [Pearson residual](../../../statistical-modelling.md#pearson-residual) is

$$
r_i^{P}=\frac{Y_i-\widehat\mu_i}
{\sqrt{\widehat\phi V(\widehat\mu_i)}}
=\frac{Y_i-\widehat\mu_i}{\sqrt{\widehat\phi\widehat\mu_i^3}},
$$

where the moment estimate of dispersion is

$$
\widehat\phi
=\frac1{n-p}\sum_{i=1}^n
\frac{(Y_i-\widehat\mu_i)^2}{\widehat\mu_i^3}.
$$

If the fitted model is adequate and the deviance residual sum is close to the Pearson statistic, then

$$
\boxed{\widehat\phi\approx\frac{245.00}{238}=1.029.}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For response $j$ from subject $s$, model2 is the [generalized linear mixed model](../../../statistical-modelling.md#generalized-linear-mixed-model)

$$
Y_{sj}\mid b_s\sim\operatorname{IG}(\mu_{sj},\lambda),
\qquad
\frac1{\mu_{sj}^2}=\beta_0+\beta_1d_{sj}+b_s,
\qquad
b_s\overset{\mathrm{iid}}\sim N(0,\tau^2),
$$

with conditional independence given the [random intercepts](../../../statistical-modelling.md#random-intercept). The fitted values are $\widehat\beta_0=8.9966$, $\widehat\beta_1=-1.2317$, $\widehat\tau^2=1.7533$, and fitted residual dispersion $0.7591$.

The random intercept models persistent between-subject differences and the resulting within-subject dependence among repeated measurements. That is the main feature absent from model1.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Test

$$
H_0:\tau^2=0
\qquad\text{against}\qquad
H_1:\tau^2>0
$$

with a [likelihood-ratio test](../../../statistical-modelling.md#likelihood-ratio-test). Model1 has three likelihood parameters and model2 has four, so their AIC values give

$$
-2\ell_1=-42.874-2(3)=-48.874,
\qquad
-2\ell_2=-45.366-2(4)=-53.366.
$$

The statistic is

$$
2(\ell_2-\ell_1)=4.492.
$$

Using a naive $\chi_1^2$ reference gives $p=0.0341$. Because the null variance lies on the boundary, the standard asymptotic reference is the mixture $\tfrac12\chi_0^2+\tfrac12\chi_1^2$, giving $p=0.0170$. Either calibration rejects at the five-percent level and supports a subject random effect.

## 2

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Order the observations so that

$$
\lVert X_{(1)}-x\rVert_\infty\leq\cdots\leq
\lVert X_{(n)}-x\rVert_\infty,
$$

using a fixed or randomized rule for ties. The [L-nearest-neighbour classifier](../../../statistical-learning.md#l-nearest-neighbour-classifier) estimates

$$
\widehat p_k(x)=\frac1L\sum_{\ell=1}^L
\mathbf1_{\{Y_{(\ell)}=k\}},
\qquad k=1,2,
$$

and predicts a class maximizing $\widehat p_k(x)$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Conditional on $X_1,\ldots,X_n$, the $L$ selected class indicators are independent Bernoulli variables. Therefore

$$
e_1(x)=\frac1L\sum_{\ell=1}^Lp_1(X_{(\ell)})
$$

and

$$
\mathbb E\left[(\widehat p_1(x)-e_1(x))^2\mid X_1,\ldots,X_n\right]
=\frac1{L^2}\sum_{\ell=1}^Lp_1(X_{(\ell)})(1-p_1(X_{(\ell)}))
\leq\frac1{4L}\leq\frac1L.
$$

Taking expectations proves the claim.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $N_\delta$ count sample points in the intersection of $[0,1]^d$ with the $\ell^\infty$ ball of radius $\delta$ around $x$. That intersection has volume at least $\delta^d$, so $N_\delta\sim\operatorname{Bin}(n,q)$ with $q\geq M\delta^d$. The event $\lVert X_{(L)}-x\rVert_\infty>\delta$ implies $N_\delta<L$. Since $\operatorname{Var}(N_\delta)\leq nq$ and $nq\geq nM\delta^d\geq L$, [Chebyshev inequality](../../../probability-inequality.md#chebyshev-inequality) gives

$$
\mathbb P(N_\delta<L)
\leq\frac{nq}{(nq-L)^2}
\leq\frac{nM\delta^d}{(nM\delta^d-L)^2}.
$$

Taking the minimum with the trivial bound one proves the result.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Put $R=\lVert X_{(L)}-x\rVert_\infty$ and $\delta_0=(2L/(nM))^{1/d}$. If $\delta_0\geq1$, the claim follows from $R\leq1$. Otherwise, for $\delta\geq\delta_0$, part (c) gives

$$
\mathbb P(R>\delta)
\leq\frac4{nM\delta^d}leq\frac2L.
$$

The [tail-sum formula](../../../probability-theory.md#tail-sum-formula) then yields

$$
\boxed{\mathbb ER
\leq\delta_0+\int_{\delta_0}^1\mathbb P(R>\delta)\,d\delta
\leq\left(\frac{2L}{nM}\right)^{1/d}+\frac2L.}
$$

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

The [Lipschitz continuity](../../../real-analysis.md#lipschitz-continuity) of $p_1$ gives

$$
|e_1(x)-p_1(x)|
\leq\frac CL\sum_{\ell=1}^L
\lVert X_{(\ell)}-x\rVert_\infty
\leq C\lVert X_{(L)}-x\rVert_\infty.
$$

Part (d) therefore implies

$$
\boxed{\mathbb E|e_1(x)-p_1(x)|
\leq C\left\{
\left(\frac{2L}{nM}\right)^{1/d}+\frac2L
\right\}.}
$$

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

By the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality), part (b), and part (e),

$$
\mathbb E|\widehat p_1(x)-p_1(x)|
\leq\frac1{\sqrt L}
+C\left\{
\left(\frac{2L}{nM}\right)^{1/d}+\frac2L
\right\}.
$$

This bound tends uniformly to zero if

$$
L\longrightarrow\infty,
\qquad \frac Ln\longrightarrow0.
$$

The [plug-in classifier excess-risk bound](../../../statistical-learning.md#plug-in-classifier-excess-risk-bound) then shows that the misclassification risk of the nearest-neighbour classifier converges to the [Bayes risk](../../../statistical-inference.md#bayes-risk).

## 3

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The $\xi_i$ are [slack variables of a support vector machine](../../../statistical-learning.md#slack-variables-of-a-support-vector-machine). The solid line is the [support-vector-machine decision boundary](../../../statistical-learning.md#support-vector-machine-decision-boundary)

$$
\widehat\alpha+x^\top\widehat\beta=0.
$$

The dashed lines are the two [support-vector-machine margin boundaries](../../../statistical-learning.md#support-vector-machine-margin-boundaries)

$$
\widehat\alpha+x^\top\widehat\beta=1,
\qquad
\widehat\alpha+x^\top\widehat\beta=-1.
$$

Each is at perpendicular distance $1/\lVert\widehat\beta\rVert_2$ from the decision boundary, so the full margin width is $2/\lVert\widehat\beta\rVert_2$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For a monarch point, $\widehat\xi_i=\max\{0,1-(\widehat\alpha+X_i^\top\widehat\beta)\}$. Point P2 lies well beyond the monarch-side dashed margin, so a plausible value is $0$. P1 lies between the decision boundary and that margin, so a plausible value is about $0.4$. P3 lies on the wrong side of the decision boundary, so its slack exceeds one; about $1.3$ is plausible. Points P1 and P3 are [support vectors](../../../statistical-learning.md#support-vector), while P2 is not.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Increasing $C$ raises the cost of [slack variables of a support vector machine](../../../statistical-learning.md#slack-variables-of-a-support-vector-machine). The fit therefore generally accepts fewer margin violations and misclassifications, at the price of a larger $\lVert\widehat\beta\rVert_2$ and hence a narrower [support-vector-machine margin](../../../statistical-learning.md#support-vector-machine-margin). Fewer observations will generally lie on or inside the narrower margin, so the number of [support vectors](../../../statistical-learning.md#support-vector) tends to decrease. These are qualitative tendencies; individual counts need not vary monotonically for every data set.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

A training observation is misclassified only if

$$
Y_i(\widehat\alpha+X_i^\top\widehat\beta)\leq0.
$$

The SVM constraint then forces $\widehat\xi_i\geq1$. Hence

$$
\mathbf1_{\{Y_i(\widehat\alpha+X_i^\top\widehat\beta)\leq0\}}
\leq\widehat\xi_i.
$$

Summing and dividing by $n$ proves $\widehat{\operatorname{Err}}_{\mathrm{tr}}\leq n^{-1}\sum_i\widehat\xi_i$.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

The code computes [Leave-one-out cross-validation](../../../statistical-learning.md#leave-one-out-cross-validation). If

$$
Y_i(\widehat\alpha+X_i^\top\widehat\beta)>1,
$$

then observation $i$ is not a support vector. Removing it leaves the optimum unchanged, and the resulting classifier still classifies it correctly. A leave-one-out error can therefore occur only for an observation on or inside the margin, which proves

$$
\widehat{\operatorname{Err}}
\leq\frac1n\sum_{i=1}^n
\mathbf1_{\{Y_i(\widehat\alpha+X_i^\top\widehat\beta)\leq1\}}.
$$

Thus the fraction of training observations on or inside the margin is an upper bound on leave-one-out error. One can refit only after deleting support vectors, reusing the full fit for every other observation. Alternatively, [K-fold cross-validation](../../../statistical-learning.md#k-fold-cross-validation) needs only $K$ fits and is often preferable for larger data sets.

## 4

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A real [positive-semidefinite kernel](../../../probability-and-statistics.md#positive-semidefinite-kernel) is a symmetric function $k:X\times X\to\mathbb R$ such that every finite Gram matrix $(k(x_i,x_j))$ is positive semidefinite. The [Moore-Aronszajn theorem](../../../probability-and-statistics.md#moore-aronszajn-theorem) says that there are a Hilbert space $H$ and a feature map $\phi:X\to H$ such that

$$
k(x,y)=\langle\phi(x),\phi(y)\rangle_H.
$$

Equivalently, $H$ can be chosen as the unique [Reproducing kernel Hilbert space](../../../probability-and-statistics.md#reproducing-kernel-hilbert-space) with reproducing kernel $k$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let $(e_{r,a},e_{r,b})_{r=1}^L$ be the standard orthonormal basis of $\mathbb R^{2L}$ and define

$$
\phi(x)=\sum_{r=1}^Le_{r,x_r}.
$$

Then

$$
\langle\phi(x),\phi(y)\rangle
=\sum_{r=1}^L\mathbf1_{\{x_r=y_r\}}=g(x,y).
$$

**Thus $g$ is a [positive-semidefinite kernel](../../../probability-and-statistics.md#positive-semidefinite-kernel).**

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The empirical [kernel covariance operator](../../../probability-and-statistics.md#kernel-covariance-operator) $\Sigma$ is self-adjoint and positive semidefinite. Maximize $\langle u,\Sigma u\rangle$ subject to $\langle u,u\rangle=1$. The first variation of the [Lagrange multiplier](../../../mathematical-optimization.md#lagrange-multiplier) functional gives

$$
2\Sigma v-2\lambda v=0,
$$

so $\Sigma v=\lambda v$. Taking the inner product with $v$ gives

$$
\boxed{\lambda=\langle v,\Sigma v\rangle
=\frac1n\sum_{i=1}^n|\langle v,\phi(x_i)\rangle|^2\geq0.}
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Positive definiteness of $K$ makes the vectors $\phi(x_1),\ldots,\phi(x_n)$ linearly independent. In particular $\Sigma\ne0$, so the maximum Rayleigh quotient is positive and $\lambda>0$. The eigenvector equation gives

$$
v=\frac1{n\lambda}\sum_{i=1}^n
\langle\phi(x_i),v\rangle\phi(x_i),
$$

which lies in their span. Hence $v=\sum_i\alpha_i\phi(x_i)$ for some $\alpha\in\mathbb R^n$.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Substituting $v=\sum_j\alpha_j\phi(x_j)$ into $\Sigma v=\lambda v$ gives

$$
\frac1n\sum_i(K\alpha)_i\phi(x_i)
=\lambda\sum_i\alpha_i\phi(x_i).
$$

Linear independence yields $K\alpha=n\lambda\alpha$. The unit-norm constraint gives

$$
\boxed{1=\langle v,v\rangle=\alpha^\top K\alpha.}
$$

<h3 id="4/f">f</h3>

↑ **Parent:** [4](#4)

<h4 id="4/f/solution">Solution</h4>

↑ **Parent:** [F](#4/f)

The feature space may be extremely high-dimensional or infinite-dimensional, and $\phi$ may be known only implicitly. Instead, compute the leading eigenvector $\alpha$ of the [kernel matrix](../../../probability-and-statistics.md#kernel-matrix) $K$, normalize it by $\alpha^\top K\alpha=1$, and use the [kernel trick](../../../probability-and-statistics.md#kernel-trick):

$$
s(x)=\langle v,\phi(x)\rangle
=\sum_{i=1}^n\alpha_i k(x_i,x).
$$

This requires only kernel evaluations.

<h3 id="4/g">g</h3>

↑ **Parent:** [4](#4)

<h4 id="4/g/solution">Solution</h4>

↑ **Parent:** [G](#4/g)

[Kernel principal component analysis](../../../probability-and-statistics.md#kernel-principal-component-analysis) can represent nonlinear low-dimensional structure by performing linear PCA in a nonlinear feature space. It can also work directly with structured objects such as strings through a kernel, without assigning them explicit finite-dimensional coordinates. Both capabilities are unavailable to ordinary linear PCA on the original variables.

## 5

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

For standardized $x\in\mathbb R^8$, model1 computes

$$
h_1=\operatorname{ReLU}(W_1x+b_1)\in\mathbb R^{24},
\quad
h_2=\operatorname{ReLU}(W_2h_1+b_2)\in\mathbb R^{16},
$$

followed by logits $z=W_3h_2+b_3\in\mathbb R^2$ and [softmax function](../../../statistical-learning.md#softmax-function) probabilities

$$
p_k(x)=\frac{e^{z_k}}{e^{z_1}+e^{z_2}}.
$$

The parameter count is

$$
(8\cdot24+24)+(24\cdot16+16)+(16\cdot2+2)=650.
$$

For one-hot labels $y_{ik}$, the [categorical cross-entropy loss](../../../statistical-learning.md#categorical-cross-entropy-loss) is

$$
-\sum_i\sum_{k=1}^2y_{ik}\log p_k(x_i).
$$

This is the negative conditional log-likelihood of independent categorical labels, equivalently Bernoulli labels in the two-class case.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

[Stochastic gradient descent](../../../numerical-analysis.md#stochastic-gradient-descent) replaces the full empirical-loss gradient by the gradient on a randomly ordered observation or mini-batch, then updates $\theta\leftarrow\theta-\eta\widehat\nabla L(\theta)$. The training half contains $768/2=384$ observations, so batches of 16 give $384/16=24$ updates per epoch. Over 100 epochs every parameter is updated $2400$ times.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

The neural-network likelihood is nonconvex, so optimization can stop at a local optimum or saddle rather than a global maximum. One hundred epochs may be insufficient for convergence. Mini-batch gradient noise together with a fixed positive learning rate can keep the iterates fluctuating around a stationary point rather than reaching it exactly. Any of these prevents the final parameters from being exact [maximum-likelihood estimators](../../../statistical-modelling.md#maximum-likelihood-estimator).

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

The dashed curve is training accuracy: it continues to rise as optimization adapts to the training observations. The solid curve is testing accuracy: it peaks near 10 epochs and then declines. The widening gap is [overfitting](../../../statistical-learning.md#overfitting).

A sensible choice is about 10 epochs, selected by [early stopping](../../../statistical-learning.md#early-stopping) at the maximum validation accuracy. In a proper analysis, a validation set rather than the final test set should choose this epoch. Early stopping is an implicit [regularization](../../../statistical-learning.md#regularization) method because it limits how far the parameters can adapt to training-specific noise.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
