<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put $L=\sup_x\|\nabla f(x)\|_\infty$, the uniform bound on the [supremum norm](../../../../../supremum-norm.md) of the [gradient](../../../../../gradient.md). The [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) on a line segment, together with the [inner product](../../../../../inner-product.md) inequality $|\langle a,b\rangle|\leq\|a\|_\infty\|b\|_1$, gives

$$
|f(x)-f(y)|\leq L\|x-y\|_1,\qquad |f(x)|\leq|f(0)|+L\|x\|_1.
$$

Thus $f$ is [Lipschitz continuous](../../../../../lipschitz-continuity.md) with respect to the [L1 norm](../../../../../l1-norm.md). The [Gaussian random variables](../../../../../gaussian-random-variable.md) comprising $X$ and $Y$ have finite exponential moments of their absolute values. More explicitly, for $c\geq0$, [Hölder's inequality](../../../../../holder-s-inequality.md) gives $\mathbb E e^{c\|X\|_1}\leq\prod_{j=1}^n(\mathbb E e^{nc|X_j|})^{1/n}<\infty$. Consequently $\mathbb Ef(X)$ and every exponential expression below are finite, including when the [covariance matrix](../../../../../covariance-matrix.md) is singular.

Use the [convex function](../../../../../convex-function.md) $\Psi(v)=e^{\lambda|v|}$. Since $Y$ is an [independent](../../../../../independent-random-variables.md) copy of $X$, [Jensen inequality](../../../../../jensen-s-inequality.md) for the [conditional expectation](../../../../../conditional-expectation.md) gives

$$
\mathbb E\Psi(f(X)-\mathbb Ef(X))\leq\mathbb E\Psi(f(X)-f(Y)).
$$

For $0\leq\theta\leq\pi/2$, define the [Gaussian rotation of independent copies](../../../../../gaussian-rotation-of-independent-copies.md)

$$
U_\theta=X\sin\theta+Y\cos\theta,\qquad V_\theta=X\cos\theta-Y\sin\theta.
$$

Writing $\Sigma=\operatorname{Cov}(X)$, both rotated [covariance matrices](../../../../../covariance-matrix.md) are $\Sigma$ and their cross-[covariance](../../../../../covariance.md) is zero. The pair has a centered [multivariate normal distribution](../../../../../multivariate-normal-distribution.md), so its components are [independent](../../../../../independent-random-variables.md) and $(U_\theta,V_\theta)$ has the same [probability law](../../../../../probability-distribution.md) as $(X,Y)$. This calculation uses no inverse of $\Sigma$ and therefore also proves the assertion for degenerate [multivariate normal distributions](../../../../../multivariate-normal-distribution.md).

The path $\theta\mapsto U_\theta$ runs from $Y$ to $X$. The [chain rule](../../../../../chain-rule.md) and the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) give the pathwise identity

$$
f(X)-f(Y)=\int_0^{\pi/2}\langle\nabla f(U_\theta),V_\theta\rangle\,d\theta.
$$

Apply [Jensen inequality](../../../../../jensen-s-inequality.md) to the uniform [probability measure](../../../../../probability-measure.md) on $[0,\pi/2]$. Then use [Tonelli theorem](../../../../../tonelli-theorem.md) and the [Gaussian rotation of independent copies](../../../../../gaussian-rotation-of-independent-copies.md) to obtain

$$
\begin{aligned}
\mathbb E\Psi(f(X)-f(Y))&\leq\frac2\pi\int_0^{\pi/2}\mathbb E\Psi\!\left(\frac\pi2\langle\nabla f(U_\theta),V_\theta\rangle\right)\,d\theta\\
&=\mathbb E\Psi\!\left(\frac\pi2\langle\nabla f(X),Y\rangle\right).
\end{aligned}
$$

This proves the [Gaussian rotation interpolation inequality](../../../../../gaussian-rotation-interpolation-inequality.md) in the required form:

$$
\boxed{\mathbb E e^{\lambda|f(X)-\mathbb Ef(X)|}\leq\mathbb E e^{(\lambda\pi/2)|\langle\nabla f(X),Y\rangle|}.}
$$

The stated almost-sure domination now gives an [exponential moment of an absolute standard normal variable](../../../../../exponential-moment-of-an-absolute-standard-normal-variable.md) bound. If $a=\lambda\pi/2$, completing the square in the [standard normal density](../../../../../standard-normal-density.md) yields

$$
\mathbb E e^{a|Z|}=\frac2{\sqrt{2\pi}}\int_0^\infty e^{az-z^2/2}\,dz=2e^{a^2/2}\Phi(a)\leq2e^{a^2/2},
$$

where $\Phi$ is the [standard normal distribution function](../../../../../standard-normal-distribution-function.md). Hence [Markov inequality](../../../../../markov-inequality.md) gives, for every $\lambda>0$,

$$
\mathbb P(|f(X)-\mathbb Ef(X)|>u)\leq2\exp\!\left(-\lambda u+\frac{\pi^2\lambda^2}{8}\right).
$$

The exponent is minimized at $\lambda=4u/\pi^2>0$. Therefore the resulting [Gaussian tail bound](../../../../../gaussian-tail-bound.md) is

$$
\boxed{\mathbb P(|f(X)-\mathbb Ef(X)|>u)\leq2e^{-2u^2/\pi^2}\qquad(u>0).}
$$

No [independence](../../../../../independent-random-variables.md) of $Z$ from $X$ or $Y$ is needed: only the given almost-sure domination is used.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 217](../../paper-217-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
