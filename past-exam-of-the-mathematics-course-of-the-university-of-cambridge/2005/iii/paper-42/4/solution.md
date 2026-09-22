<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A scalar [M-estimator](../../../../../m-estimator.md) is a selected root of $n^{-1}\sum_i\psi(Y_i,\widehat\theta)=0$, or equivalently a minimizer of a differentiable empirical objective whose derivative is this estimating equation. Its population [statistical functional](../../../../../statistical-functional.md) $T(F)=\theta_F$ solves $\int\psi(x,\theta_F)dF(x)=0$. Assume local uniqueness, consistency of the sample root, a valid differentiable local expansion, finite $\mathbb E_F\psi^2$, and

$$
A=\int\partial_\theta\psi(x,\theta_F)dF(x)\ne0.
$$

These conditions include domination sufficient to differentiate under the integral and the required local uniform control of the sample derivative.

For $F_\varepsilon=(1-\varepsilon)F+\varepsilon\delta_z$, differentiate the population estimating equation at $\varepsilon=0$. Since its uncontaminated integral is zero,

$$
0=\psi(z,\theta_F)+A\left.\frac{dT(F_\varepsilon)}{d\varepsilon}\right|_{0}.
$$

Thus the [influence function](../../../../../influence-function.md) is **$\operatorname{IF}(z;T,F)=-\psi(z,\theta_F)/A$**, with a proportionality constant [independent](../../../../../independent-random-variables.md) of $z$.

Expanding the sample equation at its population root gives

$$
\sqrt n(\widehat\theta-\theta_F)=-\frac1A\frac1{\sqrt n}\sum_i\psi(Y_i,\theta_F)+o_p(1).
$$

The summands have mean zero. The [central limit theorem](../../../../../central-limit-theorem.md) and [Slutsky's theorem](../../../../../slutsky-theorem.md) therefore yield the scalar [sandwich variance of an M-estimator](../../../../../sandwich-variance-of-an-m-estimator.md)

$$
\boxed{\sqrt n(\widehat\theta-\theta_F)\Rightarrow N(0,V(\psi,F)),\qquad V(\psi,F)=\frac{\int\psi(x,\theta_F)^2dF(x)}{[\int\partial_\theta\psi(x,\theta_F)dF(x)]^2}.}
$$

This $V$ is the limiting [variance](../../../../../variance-split.md) of the $\sqrt n$-scaled error; the estimator's [variance](../../../../../variance-split.md) is approximately $V/n$. In a correctly centred [location family](../../../../../location-family.md) with $\psi(x,\theta)=\psi(x-\theta)$, let $m=\mathbb E_F\psi'(X-\theta)$. Then $A=-m$, so the [influence function](../../../../../influence-function.md) is $\psi(z-\theta)/m$ and $V=\mathbb E\psi^2/m^2$. The minus sign from differentiating $x-\theta$ is essential.

The clipped [Huber score](../../../../../huber-score.md) in the subsequent subparts requires **$0<b<\infty$**. The PDF only displays an upper bound: at $b=0$ the estimating function vanishes identically, and at $b<0$ it is a constant with no root. A positive clipping threshold is the regular interpretation.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
