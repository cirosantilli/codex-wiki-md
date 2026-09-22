<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A general [exponential family](../../../../../../exponential-family-split.md) of order $p$ has the representation

$$
f(x;\alpha)=h(x)\exp\{\eta(\alpha)^TT(x)-\kappa(\eta(\alpha))\},\qquad T(x)=(T_1(x),\ldots,T_p(x))^T.
$$

The canonical [sufficient statistics](../../../../../../sufficient-statistic.md) $T_j$ are independent of the parameter, the support is fixed, and the [cumulant function](../../../../../../cumulant-function-of-an-exponential-family.md) normalizes the [probability density function](../../../../../../probability-density-function.md). Minimality rules out a redundant affine relation among the [sufficient statistics](../../../../../../sufficient-statistic.md). If $\alpha$ ranges over an [open subset](../../../../../../open-set.md) of $\mathbb R^q$, $q<p$, and $\eta$ is a [smooth embedding](../../../../../../smooth-embedding.md) with derivative of rank $q$, its image is a $q$-dimensional parameter surface in the $p$-dimensional [natural parameter space](../../../../../../natural-parameter-space.md): this is a $(p,q)$ [curved exponential family](../../../../../../curved-exponential-family.md). In a genuinely curved example the surface is nonaffine.

Take the [normal distribution](../../../../../../normal-distribution.md) $N(\mu,\mu^2)$ with $\mu>0$. Its log density expands as

$$
\log f(y;\mu)=-\tfrac12\log(2\pi\mu^2)-\tfrac12+\frac y\mu-\frac{y^2}{2\mu^2}.
$$

It is a $(2,1)$ [curved exponential family](../../../../../../curved-exponential-family.md) with [sufficient statistics](../../../../../../sufficient-statistic.md) $(y,y^2)$ and [natural parameters](../../../../../../natural-parameter-of-an-exponential-family.md) $\eta_1=1/\mu$, $\eta_2=-1/(2\mu^2)$. The ambient full [normal distribution](../../../../../../normal-distribution.md) family has $\eta_1\in\mathbb R$, $\eta_2<0$ and

$$
\kappa(\eta)=-\frac{\eta_1^2}{4\eta_2}+\frac12\log\frac\pi{-\eta_2}.
$$

The curve is $\eta_2=-\eta_1^2/2$ with $\eta_1>0$, and its derivative with respect to $\mu$ has rank one. Thus **the mean and [variance](../../../../../../variance-split.md) are constrained by $\operatorname{Var}(Y)=(\mathbb EY)^2$**; the two canonical parameters cannot vary independently. [Concavity](../../../../../../concave-function.md) of an ambient canonical log [likelihood](../../../../../../likelihood-function.md) need not persist along a curved parameter surface.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
