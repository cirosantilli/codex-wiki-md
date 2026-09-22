<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

Write $s=\sqrt{1-\rho^2}>0$. The inverse change of variables is $y=\rho x+sz$, whose [Jacobian determinant](../../../../../jacobian-determinant.md) has absolute value $s$. Completing the square gives

$$
\frac{x^2-2\rho xy+y^2}{1-\rho^2}=x^2+z^2.
$$

The [change of variables formula](../../../../../change-of-variables-formula.md) therefore transforms the joint [probability density function](../../../../../probability-density-function.md) to

$$
g(x,z)=s f(x,\rho x+sz)
=\frac1{2\pi}e^{-(x^2+z^2)/2}
=\left(\frac{e^{-x^2/2}}{\sqrt{2\pi}}\right)
 \left(\frac{e^{-z^2/2}}{\sqrt{2\pi}}\right).
$$

It factors into two normalized [standard normal distribution](../../../../../standard-normal-distribution.md) densities. Thus **$X$ and $Z$ are [independent](../../../../../independent-random-variables.md) $N(0,1)$ variables**; factorization proves the requested [independence](../../../../../independent-random-variables.md), rather than simply zero [covariance](../../../../../covariance.md).

The [standard Gaussian random vector](../../../../../standard-gaussian-random-vector.md) $(X,Z)$ has a rotation-invariant density. In [polar coordinates](../../../../../polar-coordinates.md), $X=r\cos\theta$, $Z=r\sin\theta$, its density with the area factor is $(2\pi)^{-1}re^{-r^2/2}$, so the angular coordinate is uniform on an interval of length $2\pi$.

Put $\alpha=\arcsin\rho\in(-\pi/2,\pi/2)$, so $s=\cos\alpha$ and

$$
Y=\rho X+sZ=r\sin(\theta+\alpha).
$$

In the right half-plane, choose $-\pi/2<\theta<\pi/2$. The additional condition $Y>0$ then requires $-\alpha<\theta<\pi/2$. This wedge has angle $\pi/2+\alpha$; its boundary has [probability](../../../../../probability.md) zero. Consequently

$$
\boxed{\mathbb P(X>0,Y>0)=\frac14+\frac{\arcsin\rho}{2\pi}.}
$$

At $\rho=0$ this is $1/4$, as required by [independence](../../../../../independent-random-variables.md). The limits as $\rho\to1$ and $\rho\to-1$ are $1/2$ and zero, respectively. The angular calculation is also the geometric [basis](../../../../../basis.md) of the [Gaussian sign-correlation identity](../../../../../gaussian-sign-correlation-identity.md).

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
