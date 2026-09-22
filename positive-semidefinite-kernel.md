# Positive-semidefinite kernel

↑ **Parent:** [Probability and statistics](probability-and-statistics.md)

A symmetric function $k$ is a positive-semidefinite kernel when every finite Gram matrix $(k(x_i,x_j))$ is positive semidefinite.

**Table of contents**

- [Mercer kernel](#mercer-kernel)
- [Cauchy-Schwarz inequality for positive-semidefinite kernels](#cauchy-schwarz-inequality-for-positive-semidefinite-kernels)
- [Kernel matrix](#kernel-matrix)
- [Feature map](#feature-map)
  - [Canonical feature space of a positive-semidefinite kernel](#canonical-feature-space-of-a-positive-semidefinite-kernel)
  - [Random feature map](#random-feature-map)
    - [Random Fourier features](#random-fourier-features)
- [Gaussian kernel](#gaussian-kernel)
- [Linear kernel](#linear-kernel)
- [Polynomial kernel](#polynomial-kernel)
- [Closure property of positive-semidefinite kernels](#closure-property-of-positive-semidefinite-kernels)
  - [Integral closure of positive-semidefinite kernels](#integral-closure-of-positive-semidefinite-kernels)
  - [Product of positive-semidefinite kernels](#product-of-positive-semidefinite-kernels)
- [Laplace kernel](#laplace-kernel)
- [Reproducing kernel Hilbert space](#reproducing-kernel-hilbert-space)
  - [Sum of reproducing-kernel Hilbert spaces](#sum-of-reproducing-kernel-hilbert-spaces)
    - [Common representer coefficients for a sum of kernels](#common-representer-coefficients-for-a-sum-of-kernels)
  - [Reproducing property](#reproducing-property)
  - [Representer theorem](#representer-theorem)
  - [Kernel method](#kernel-method)
    - [Kernel ridge regression](#kernel-ridge-regression)
      - [Prediction-risk bound for kernel ridge regression](#prediction-risk-bound-for-kernel-ridge-regression)
      - [Kernel-ridge hat matrix](#kernel-ridge-hat-matrix)
  - [Moore-Aronszajn theorem](#moore-aronszajn-theorem)
  - [Kernel covariance operator](#kernel-covariance-operator)
  - [Kernel trick](#kernel-trick)
    - [XOR separation by a product feature](#xor-separation-by-a-product-feature)
    - [Dual prediction with a kernel](#dual-prediction-with-a-kernel)
    - [Computational tradeoffs of the kernel trick](#computational-tradeoffs-of-the-kernel-trick)
    - [Kernel principal component analysis](#kernel-principal-component-analysis)
  - [Reproducing-kernel Hilbert space of a stationary Gaussian process](#reproducing-kernel-hilbert-space-of-a-stationary-gaussian-process)

## Mercer kernel

↑ **Parent:** [Positive-semidefinite kernel](positive-semidefinite-kernel.md)

In the compact-domain spectral setting, a Mercer kernel is a continuous symmetric [positive-semidefinite kernel](positive-semidefinite-kernel.md) on a compact space equipped with a finite full-support measure. [Mercer's theorem](functional-analysis.md#mercer-s-theorem) yields nonnegative eigenvalues and an expansion $k(x,z)=\sum_j\lambda_j e_j(x)e_j(z)$, giving features $(\sqrt{\lambda_j}e_j(x))_j$ in $\ell^2$. The finite-Gram positivity condition on arbitrary domains is more general than these spectral hypotheses; all such kernels still have a [Reproducing kernel Hilbert space](#reproducing-kernel-hilbert-space) realization.

## Cauchy-Schwarz inequality for positive-semidefinite kernels

↑ **Parent:** [Positive-semidefinite kernel](positive-semidefinite-kernel.md)

A real [positive-semidefinite kernel](positive-semidefinite-kernel.md) satisfies $|k(x,y)|^2\leq k(x,x)k(y,y)$. This follows from positivity of its two-point [kernel matrix](#kernel-matrix). If a diagonal value is zero, the corresponding off-diagonal values must also vanish.

## Kernel matrix

↑ **Parent:** [Positive-semidefinite kernel](positive-semidefinite-kernel.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kernel_matrix)

For points $x_1,\ldots,x_n$, the kernel matrix has entries $K_{ij}=k(x_i,x_j)$ and is positive semidefinite.

## Feature map

↑ **Parent:** [Positive-semidefinite kernel](positive-semidefinite-kernel.md)

A feature map sends $x$ to a vector $\phi(x)$ in a vector space with an [inner product](inner-product.md) so that $k(x,y)=\langle\phi(x),\phi(y)\rangle$.

### Canonical feature space of a positive-semidefinite kernel

↑ **Parent:** [Feature map](#feature-map)

On the finite formal span of symbols $e_x$, define $B(e_x,e_y)=k(x,y)$ and extend bilinearly. For a [positive-semidefinite kernel](positive-semidefinite-kernel.md), the null vectors of this [positive semidefinite bilinear form](quadratic-form.md#positive-semidefinite-bilinear-form) form its [radical of a bilinear form](bilinear-form.md#radical-of-a-bilinear-form). Quotienting by that [linear subspace](vector-space.md#vector-subspace) gives an [inner product space](inner-product.md#inner-product-space) and [feature map](#feature-map) $x\mapsto[e_x]$ with $\langle[e_x],[e_y]\rangle=k(x,y)$. This construction works for degenerate and zero kernels.

### Random feature map

↑ **Parent:** [Feature map](#feature-map)

A random feature map is a random function $\widehat\phi:\mathcal X\to\mathbb R^q$ whose expected inner product represents a kernel:

$$
k(x,y)=\mathbb E\langle\widehat\phi(x),\widehat\phi(y)\rangle.
$$

#### Random Fourier features

↑ **Parent:** [Random feature map](#random-feature-map)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Random_Fourier_features)

Random Fourier features represent a translation-invariant [positive-semidefinite kernel](positive-semidefinite-kernel.md) by sampling frequencies from its spectral distribution and using sine and cosine features. They replace an implicit infinite-dimensional [feature map](#feature-map) by a finite random approximation.

## Gaussian kernel

↑ **Parent:** [Positive-semidefinite kernel](positive-semidefinite-kernel.md)

The Gaussian kernel is a translation-invariant [positive-semidefinite kernel](positive-semidefinite-kernel.md) whose canonical [feature map](#feature-map) takes values in an [infinite-dimensional vector space](vector-space.md#infinite-dimensional-vector-space).

## Linear kernel

↑ **Parent:** [Positive-semidefinite kernel](positive-semidefinite-kernel.md)

The linear kernel is the ordinary [inner product](inner-product.md) on a real vector space.

## Polynomial kernel

↑ **Parent:** [Positive-semidefinite kernel](positive-semidefinite-kernel.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polynomial_kernel)

For $x,z\in\mathbb R^d$, a polynomial kernel is the [positive-semidefinite kernel](positive-semidefinite-kernel.md) $k(x,z)=(x^Tz+c)^r$, where $r$ is a positive integer and $c\geq0$. The case $c=0$ uses [monomials](polynomial.md#monomial) of total degree $r$; $c>0$ also includes lower degrees. The [feature map](#feature-map) weights matter: listing each distinct [monomial](polynomial.md#monomial) once with coefficient one generally gives a different [inner product](inner-product.md).[Section 4.2.2, pp. 89–90, equations (4.23)–(4.24): polynomial kernels and weighted monomial features](mathematics-bibliography.md#gaussian-processes-for-machine-learning-by-carl-edward-rasmussen-and-christopher-k-i-williams)

For the homogeneous quadratic case in two dimensions, take the scaled [quadratic feature map](foundations-of-mathematics.md#quadratic-feature-map)

$$
\phi(x_1,x_2)=\begin{pmatrix}x_1^2\\\sqrt2 x_1x_2\\x_2^2\end{pmatrix},\qquad k(x,z)=(x^Tz)^2.
$$

The [inner product](inner-product.md) identity is explicit:

$$
\phi(x)^T\phi(z)=x_1^2z_1^2+2x_1x_2z_1z_2+x_2^2z_2^2=(x_1z_1+x_2z_2)^2=k(x,z).
$$

The factor $\sqrt2$ accounts for the two equal cross terms in the square. Thus an [inner product](inner-product.md) of three derived coordinates can be obtained from an [inner product](inner-product.md) of the two input coordinates followed by squaring. The [kernel trick](#kernel-trick) uses this equality inside an algorithm; the [feature map](#feature-map) explains which nonlinear [functions](function.md) the algorithm can represent.

## Closure property of positive-semidefinite kernels

↑ **Parent:** [Positive-semidefinite kernel](positive-semidefinite-kernel.md)

Nonnegative scalar multiples, sums, pointwise products, pointwise limits, and pullbacks of positive-semidefinite kernels are positive semidefinite whenever the displayed expressions are defined.

### Integral closure of positive-semidefinite kernels

↑ **Parent:** [Closure property of positive-semidefinite kernels](#closure-property-of-positive-semidefinite-kernels)

Suppose $k_\tau$ is a [positive-semidefinite kernel](positive-semidefinite-kernel.md) for every $\tau$ and its diagonal entries are integrable. Positivity of each $2\times2$ [kernel matrix](#kernel-matrix) gives

$$
|k_\tau(x,y)|\leq\sqrt{k_\tau(x,x)k_\tau(y,y)}.
$$

The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) makes every entry integrable, and integrating each nonnegative finite quadratic form shows that $\int k_\tau\,d\tau$ is again a positive-semidefinite kernel.

### Product of positive-semidefinite kernels

↑ **Parent:** [Closure property of positive-semidefinite kernels](#closure-property-of-positive-semidefinite-kernels)

The pointwise product of two [positive-semidefinite kernels](positive-semidefinite-kernel.md) is positive semidefinite because its finite [kernel matrix](#kernel-matrix) is the entrywise product of two positive-semidefinite matrices, to which the [Schur product theorem](linear-algebra.md#schur-product-theorem) applies.

## Laplace kernel

↑ **Parent:** [Positive-semidefinite kernel](positive-semidefinite-kernel.md)

The Laplace kernel on $\mathbb R^d$ is a translation-invariant [positive-semidefinite kernel](positive-semidefinite-kernel.md). Independent standard [Cauchy random variables](probability-distribution.md#cauchy-random-variable) give its [Random Fourier feature](#random-fourier-features) representation through their characteristic function $e^{-|t|}$.

## Reproducing kernel Hilbert space

↑ **Parent:** [Positive-semidefinite kernel](positive-semidefinite-kernel.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reproducing_kernel_Hilbert_space)

A reproducing-kernel Hilbert space is a Hilbert space of functions in which point evaluation is continuous and satisfies $f(x)=\langle f,k(x,\cdot)\rangle$.

### Sum of reproducing-kernel Hilbert spaces

↑ **Parent:** [Reproducing kernel Hilbert space](#reproducing-kernel-hilbert-space)

For [positive-semidefinite kernels](positive-semidefinite-kernel.md) $k_j$ with [Reproducing kernel Hilbert spaces](#reproducing-kernel-hilbert-space) $\mathcal H_j$, the [Reproducing kernel Hilbert space](#reproducing-kernel-hilbert-space) of $k=\sum_jk_j$ consists of sums $f=\sum_jf_j$, with

$$
\|f\|_{\mathcal H_k}^2=\min_{\sum_jf_j=f}\sum_j\|f_j\|_{\mathcal H_j}^2.
$$

The minimum is attained uniquely. Indeed, in the [Hilbert space](hilbert-space.md) direct sum $E=\bigoplus_j\mathcal H_j$, the tuples summing to zero form a closed subspace $N$: they are the intersection, over inputs $x$, of the kernels of the continuous maps $(f_j)\mapsto\sum_jf_j(x)$. Every affine fibre has a unique representative in $N^\perp$ by [orthogonal decomposition by a closed subspace](hilbert-space.md#orthogonal-decomposition-by-a-closed-subspace). The [vector](vector-space.md#vector) $(k_j(\cdot,x))_j$ lies in $N^\perp$ and represents evaluation in the quotient; its evaluation at $y$ is $\sum_jk_j(y,x)$, identifying the [positive-semidefinite kernel](positive-semidefinite-kernel.md) with $k$.

#### Common representer coefficients for a sum of kernels

↑ **Parent:** [Sum of reproducing-kernel Hilbert spaces](#sum-of-reproducing-kernel-hilbert-spaces)

For a real-valued [loss function](foundations-of-mathematics.md#loss-function) depending only on evaluations at $x_1,\ldots,x_n$, and a positive squared-norm penalty, any minimizing tuple in a [sum of reproducing-kernel Hilbert spaces](#sum-of-reproducing-kernel-hilbert-spaces) has the form

$$
\widehat f_j=\sum_{i=1}^n\widehat\alpha_i k_j(\cdot,x_i)
$$

with the same coefficient [vector](vector-space.md#vector) for every component. The tuple must be the unique minimum-norm decomposition of its sum. Apply the [representer theorem](#representer-theorem) to that sum and note that the displayed tuple has total squared [norm](normed-vector-space.md#norm) $\sum_j\widehat\alpha^TK_j\widehat\alpha=\widehat\alpha^T(\sum_jK_j)\widehat\alpha$, exactly the [norm](normed-vector-space.md#norm) of the sum. This argument is conditional on existence of a [minimizer](analysis.md#global-minimizer); arbitrary [loss functions](foundations-of-mathematics.md#loss-function) need not attain their infimum.

### Reproducing property

↑ **Parent:** [Reproducing kernel Hilbert space](#reproducing-kernel-hilbert-space)

The reproducing property is $f(x)=\langle f,k(x,\cdot)\rangle_{\mathcal H}$; it turns point evaluation into an inner product with a kernel section.

### Representer theorem

↑ **Parent:** [Reproducing kernel Hilbert space](#reproducing-kernel-hilbert-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Representer_theorem)

The representer theorem reduces regularized optimization over a reproducing-kernel Hilbert space to the span of kernel sections at the observed points.

### Kernel method

↑ **Parent:** [Reproducing kernel Hilbert space](#reproducing-kernel-hilbert-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kernel_method)

A kernel method represents data through a [positive-semidefinite kernel](positive-semidefinite-kernel.md), allowing algorithms to use inner products in an implicit [feature map](#feature-map).

#### Kernel ridge regression

↑ **Parent:** [Kernel method](#kernel-method)

Kernel ridge regression minimizes empirical squared error plus the squared norm in a [Reproducing kernel Hilbert space](#reproducing-kernel-hilbert-space). The [representer theorem](#representer-theorem) reduces it to [ridge regression](linear-regression.md#ridge-regression) with the [kernel matrix](#kernel-matrix) as its feature Gram matrix.

##### Prediction-risk bound for kernel ridge regression

↑ **Parent:** [Kernel ridge regression](#kernel-ridge-regression)

For the unscaled objective $\sum_i(Y_i-f(x_i))^2+\lambda\|f\|_{\mathcal H}^2$, the [kernel-ridge hat matrix](#kernel-ridge-hat-matrix) is $H=K(K+\lambda I)^{-1}$. Its prediction variance is $\sigma^2\operatorname{tr}(H^2)/n$. For eigenvalues $d_i\geq0$, use $d_i^2/(d_i+\lambda)^2\leq\min\{d_i/(4\lambda),1\}$ and $\lambda^2d_i/(d_i+\lambda)^2\leq\lambda/4$ to bound the variance and the squared bias. The latter also uses the [reproducing property](#reproducing-property) and [Bessel inequality](hilbert-space.md#bessel-s-inequality), and does not require invertibility of $K$.

> EXISTING BODY EXPANSION, not a new concept: replace the present one-direction definition of Faithfulness of a directed acyclic graph in probability-and-statistics.bigb, under Causal directed acyclic graph, with the following body. Retain its existing header and parent.

##### Kernel-ridge hat matrix

↑ **Parent:** [Kernel ridge regression](#kernel-ridge-regression)

For kernel matrix $K$ and objective normalized as $n^{-1}\lVert Y-f\rVert_2^2+\lambda\lVert f\rVert_{\mathcal H}^2$, the fitted values are $H_\lambda Y$, where

$$
H_\lambda=K(K+n\lambda I)^{-1}.
$$

### Moore-Aronszajn theorem

↑ **Parent:** [Reproducing kernel Hilbert space](#reproducing-kernel-hilbert-space)

Every positive-semidefinite kernel $k$ has a Hilbert-space feature map $\phi$ satisfying $k(x,y)=\langle\phi(x),\phi(y)\rangle$, and determines a unique reproducing-kernel Hilbert space.

### Kernel covariance operator

↑ **Parent:** [Reproducing kernel Hilbert space](#reproducing-kernel-hilbert-space)

For feature vectors $\phi(x_i)$, the empirical uncentered kernel covariance operator is

$$
\Sigma v=\frac1n\sum_i\phi(x_i)\langle\phi(x_i),v\rangle.
$$

### Kernel trick

↑ **Parent:** [Reproducing kernel Hilbert space](#reproducing-kernel-hilbert-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kernel_trick)

The kernel trick evaluates [inner products](inner-product.md) of [feature map](#feature-map) outputs through $k(x,z)=\langle\phi(x),\phi(z)\rangle$ without explicitly constructing those [vectors](vector-space.md#vector). An algorithm expressed entirely through these [inner products](inner-product.md) can therefore operate on nonlinear derived coordinates using only evaluations of a [positive-semidefinite kernel](positive-semidefinite-kernel.md) on the original inputs. A [classifier](foundations-of-mathematics.md#classifier) linear in the derived coordinates can have a nonlinear boundary in the original coordinates.

The [polynomial kernel](#polynomial-kernel) gives a finite, fully visible example: $k(x,z)=(x^Tz)^2$ corresponds to $\phi(x)=(x_1^2,\sqrt2 x_1x_2,x_2^2)^T$. The [XOR separation by a product feature](#xor-separation-by-a-product-feature) below makes the interaction coordinate $x_1x_2$ useful, while [dual prediction with a kernel](#dual-prediction-with-a-kernel) shows how to predict without calculating it explicitly.

An arbitrary score called a similarity need not be a [positive-semidefinite kernel](positive-semidefinite-kernel.md). Symmetry alone, even with nonnegative entries, is insufficient: the symmetric [matrix](vector-space.md#matrix)

$$
S=\begin{pmatrix}1&2\\2&1\end{pmatrix}
$$

has $a^TSa=-2$ for $a=(1,-1)^T$, so it cannot be a [Gram matrix](inner-product.md#gram-matrix) of real [inner products](inner-product.md). A [positive-semidefinite kernel](positive-semidefinite-kernel.md) requires a [positive semidefinite matrix](quadratic-form.md#positive-semidefinite-matrix) for every finite choice of inputs, not just the observed [training data](foundations-of-mathematics.md#training-data).[Section 4.1, p. 80: Gram matrices, quadratic-form definition of positive semidefiniteness, and nonnegative eigenvalues](mathematics-bibliography.md#gaussian-processes-for-machine-learning-by-carl-edward-rasmussen-and-christopher-k-i-williams) The existing [Moore-Aronszajn theorem](#moore-aronszajn-theorem) connects this requirement to a [Reproducing kernel Hilbert space](#reproducing-kernel-hilbert-space); this example needs only finite [linear algebra](linear-algebra.md).

#### XOR separation by a product feature

↑ **Parent:** [Kernel trick](#kernel-trick)

Give the four corners of the square the [exclusive or](theoretical-computer-science.md#exclusive-or) labels: $+1$ when the input signs differ and $-1$ when they agree. In the following order,

$$
p_1=(1,1),\quad p_2=(1,-1),\quad p_3=(-1,1),\quad p_4=(-1,-1),\qquad y=(-1,1,1,-1)^T.
$$

No [affine function](vector-space.md#affine-function) $g(x)=a_1x_1+a_2x_2+b$ has the required strictly positive scores at $p_2,p_3$ and strictly negative scores at $p_1,p_4$: both pairs have midpoint zero, so $g(p_2)+g(p_3)=2b=g(p_1)+g(p_4)$ would have to be both positive and negative. This also rules out perfect classification by a single threshold with a consistent tie rule.

Under the [polynomial kernel](#polynomial-kernel)'s [quadratic feature map](foundations-of-mathematics.md#quadratic-feature-map), the two classes become two distinct [vectors](vector-space.md#vector):

$$
\phi(p_1)=\phi(p_4)=(1,\sqrt2,1)^T,\qquad \phi(p_2)=\phi(p_3)=(1,-\sqrt2,1)^T.
$$

The [hyperplane](vector-space.md#hyperplane) $\phi_2=0$ separates them. With $w=(0,-1/\sqrt2,0)^T$ and $b=0$, the score and [classifier](foundations-of-mathematics.md#classifier) are

$$
f(x)=w^T\phi(x)=-x_1x_2,\qquad h(x)=\operatorname{sgn}f(x).
$$

All four signed scores $y_i f(p_i)$ equal one. In the input plane the boundary is $x_1x_2=0$, the union of the coordinate axes; in the derived coordinates it is a single [hyperplane](vector-space.md#hyperplane). The [feature map](#feature-map) identifies opposite corners, which is harmless for these labels because opposite corners belong to the same class. A fixed [feature map](#feature-map) would not separate labels that disagree at identical mapped [vectors](vector-space.md#vector).

<a id="image-xor-labels-in-the-input-square-and-the-quadratic-feature-slice"></a>
![](kernel-quadratic-xor-feature-separation.png)

**[Figure 1](#image-xor-labels-in-the-input-square-and-the-quadratic-feature-slice). XOR labels in the input square and the quadratic feature slice**. The dashed diagonals join equal-label input pairs and share their midpoint, obstructing affine separation. In the feature panel all mapped points have third coordinate one; the two coincident pairs are separated by the horizontal hyperplane at second coordinate zero.

#### Dual prediction with a kernel

↑ **Parent:** [Kernel trick](#kernel-trick)

If the weight [vector](vector-space.md#vector) lies in the [linear span](vector-space.md#linear-span) of the training [feature map](#feature-map) outputs, write $w=\sum_i\beta_i\phi(p_i)$. Then

$$
f(z)=w^T\phi(z)+b=\sum_i\beta_i k(p_i,z)+b.
$$

This is a dual representation: coefficients weight training examples rather than feature coordinates. They need not be positive, and need not be unique when the [kernel matrix](#kernel-matrix) is singular. Some [kernel methods](#kernel-method) instead write $\beta_i=\alpha_i y_i$ with $\alpha_i\geq0$ under their own optimization constraints.[Kernelizing classification with support vector machines: displayed prediction as a sum of label-weighted kernel evaluations](mathematics-bibliography.md#the-kernel-trick-by-ryan-giordano) The formula is an algebraic conversion for a weight [vector](vector-space.md#vector) in this [linear span](vector-space.md#linear-span), not a claim about every possible weight [vector](vector-space.md#vector). The [representer theorem](#representer-theorem) gives a broader reason this form appears in regularized [kernel methods](#kernel-method).

For the [XOR separation by a product feature](#xor-separation-by-a-product-feature), let $\Phi$ have rows $\phi(p_i)^T$. The [Gram matrix](inner-product.md#gram-matrix) of those rows, equivalently the [kernel matrix](#kernel-matrix), is

$$
\Phi=\begin{pmatrix}1&\sqrt2&1\\1&-\sqrt2&1\\1&-\sqrt2&1\\1&\sqrt2&1\end{pmatrix},\qquad
K=\Phi\Phi^T=\bigl((p_i^Tp_j)^2\bigr)_{ij}=\begin{pmatrix}4&0&0&4\\0&4&4&0\\0&4&4&0\\4&0&0&4\end{pmatrix}.
$$

Its [eigenvalues](linear-operator-theory.md#eigenvalue) are $8,8,0,0$, so it is a [positive semidefinite matrix](quadratic-form.md#positive-semidefinite-matrix) of [rank](quadratic-form.md#rank-one-quadratic-form) two, not an invertible [matrix](vector-space.md#matrix). More generally, for any real coefficient [vector](vector-space.md#vector) $a$ and any finite set of inputs,

$$
a^TKa=\left\|\sum_i a_i\phi(p_i)\right\|_2^2\geq0.
$$

This proves the [positive-semidefinite kernel](positive-semidefinite-kernel.md) condition for the displayed [polynomial kernel](#polynomial-kernel) on all of $\mathbb R^2$, rather than checking only this square.

Here $Ky=8y$, so the explicit choice $\beta=y/8$ gives $K\beta=y$ and $\Phi^T\beta=w$. Consequently

$$
f(z)=\frac{-k(p_1,z)+k(p_2,z)+k(p_3,z)-k(p_4,z)}8=-z_1z_2.
$$

For the new input $z=(1,1/2)$, the four [polynomial kernel](#polynomial-kernel) evaluations are $(9/4,1/4,1/4,9/4)^T$. Their weighted sum is $-1/2$, and the [sign function](foundations-of-mathematics.md#sign-function) predicts $-1$. No explicit [feature map](#feature-map) is needed for this calculation. These coefficients were constructed to reproduce the chosen separator; no fitting algorithm or [generalization](statistical-learning.md#generalization-in-statistical-learning) guarantee is being asserted.

<a id="image-quadratic-kernel-gram-matrix-and-a-dual-prediction-for-a-new-input"></a>
![](kernel-quadratic-gram-dual-evaluation.png)

**[Figure 2](#image-quadratic-kernel-gram-matrix-and-a-dual-prediction-for-a-new-input). Quadratic kernel Gram matrix and a dual prediction for a new input**. Both panels use the same ordered four square corners. The Gram matrix has eigenvalues eight, eight, zero, zero. The new-input column contains four kernel evaluations, whose signed weighted contributions sum to minus one half.

#### Computational tradeoffs of the kernel trick

↑ **Parent:** [Kernel trick](#kernel-trick)

For $d$ input coordinates, the homogeneous quadratic [polynomial kernel](#polynomial-kernel) has a weighted [quadratic feature map](foundations-of-mathematics.md#quadratic-feature-map) with $D=d(d+1)/2$ distinct [monomials](polynomial.md#monomial). Computing an [inner product](inner-product.md) of already stored mapped [vectors](vector-space.md#vector) costs $O(D)$ arithmetic operations, whereas $(x^Tz)^2$ costs $O(d)$ using the input [vectors](vector-space.md#vector). Here $O$ denotes [big O notation](real-analysis.md#big-o-notation). Higher fixed degrees can make the dimension gap much larger.

Sample count still matters. With $n$ training examples, materializing a dense [kernel matrix](#kernel-matrix) stores $n^2$ numbers and requires $n(n+1)/2$ distinct evaluations using symmetry. A dense direct solve for [kernel ridge regression](#kernel-ridge-regression) typically takes $O(n^3)$ operations after constructing the [kernel matrix](#kernel-matrix), while a dual prediction with $m$ nonzero coefficients uses $m$ kernel evaluations. Explicit finite [feature maps](#feature-map) can be preferable when $D$ is small relative to $n$, and a stored primal weight [vector](vector-space.md#vector) can make prediction depend on $D$ rather than on $n$. [The kernel trick by Ryan Giordano](mathematics-bibliography.md#the-kernel-trick-by-ryan-giordano) (sections Ridge regression and The polynomial kernel) explains the change from feature-coordinate equations to training-example equations; neither representation is universally faster.

The [kernel trick](#kernel-trick) saves explicit feature construction when the [positive-semidefinite kernel](positive-semidefinite-kernel.md) is economical to evaluate; it does not remove the cost of optimization, choose a useful [positive-semidefinite kernel](positive-semidefinite-kernel.md), or establish [generalization](statistical-learning.md#generalization-in-statistical-learning). [Random Fourier features](#random-fourier-features) illustrate a different tradeoff: replacing the exact [Gaussian kernel](#gaussian-kernel) with a finite approximate [feature map](#feature-map) can reduce dependence on the sample count while introducing approximation error.

#### Kernel principal component analysis

↑ **Parent:** [Kernel trick](#kernel-trick)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kernel_principal_component_analysis)

Kernel principal component analysis diagonalizes a centered [kernel matrix](#kernel-matrix) to perform principal component analysis in an implicit feature space.

### Reproducing-kernel Hilbert space of a stationary Gaussian process

↑ **Parent:** [Reproducing kernel Hilbert space](#reproducing-kernel-hilbert-space)

If a stationary [Gaussian process](gaussian-process.md) has covariance spectral density $\widehat K$, its reproducing-kernel Hilbert space has norm

$$
\lVert f\rVert_{\mathcal H_K}^2
=c\int\frac{|\widehat f(u)|^2}{\widehat K(u)}\,du
$$

on the functions for which this integral is finite.

## ↑ Ancestors (4)

1. [Probability and statistics](probability-and-statistics.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (34)

- [Canonical feature space of a positive-semidefinite kernel](#canonical-feature-space-of-a-positive-semidefinite-kernel)
- [Cauchy-Schwarz inequality for positive-semidefinite kernels](#cauchy-schwarz-inequality-for-positive-semidefinite-kernels)
- [Computational tradeoffs of the kernel trick](#computational-tradeoffs-of-the-kernel-trick)
- [Covariance function](stochastic-process.md#covariance-function)
- [Dual prediction with a kernel](#dual-prediction-with-a-kernel)
- [Gaussian density kernel](nonparametric-statistics.md#gaussian-density-kernel)
- [Gaussian kernel](#gaussian-kernel)
- [Integral closure of positive-semidefinite kernels](#integral-closure-of-positive-semidefinite-kernels)
- [Kernel method](#kernel-method)
- [Kernel trick](#kernel-trick)
- [Laplace kernel](#laplace-kernel)
- [Mercer kernel](#mercer-kernel)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-205.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-217.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-205.md#3/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-205.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-218.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-205.md#1/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-205.md#1/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-205.md#1/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-205.md#1/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-205.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-218.md#6/c/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-205.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-205.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-205.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-218.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-218.md#4/b/solution)
- [Periodic Gaussian process with zero period average](gaussian-process.md#periodic-gaussian-process-with-zero-period-average)
- [Polynomial kernel](#polynomial-kernel)
- [Product of positive-semidefinite kernels](#product-of-positive-semidefinite-kernels)
- [Random Fourier features](#random-fourier-features)
- [Sum of reproducing-kernel Hilbert spaces](#sum-of-reproducing-kernel-hilbert-spaces)
