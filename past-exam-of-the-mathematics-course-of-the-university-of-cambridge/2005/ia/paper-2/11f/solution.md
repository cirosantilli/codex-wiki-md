<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

All the following [distributions](../../../../../distribution-mathematical-analysis.md) are conditional on the point lying in the unit disk. Initially the [joint probability density](../../../../../joint-probability-density.md) of $(S,T)$ is $1/4$ on the square. The disk has area $\pi$, so the conditioning event has [probability](../../../../../probability.md) $\pi/4$. Dividing by this probability gives the constant conditional [density](../../../../../density.md) $1/\pi$ on the disk, proving its [uniform distribution](../../../../../continuous-uniform-distribution.md) there.

The [polar coordinates](../../../../../polar-coordinates.md) $S=r\cos\theta,T=r\sin\theta$ have [Jacobian determinant](../../../../../jacobian-determinant.md) $r$. Consequently

$$
\boxed{f_{R,\Theta}(r,\theta)=\frac r\pi,\qquad 0<r<1,\quad0\leq\theta<2\pi.}
$$

Integrating the [joint probability density](../../../../../joint-probability-density.md) gives $f_R(r)=2r$ and $f_\Theta(\theta)=1/(2\pi)$. Since the joint density equals the product of these marginal densities on a product support, **$R$ and $\Theta$ are independent**. In particular $U=R^2$ has the [uniform distribution](../../../../../continuous-uniform-distribution.md) on $(0,1)$.

The second [change of variables](../../../../../change-of-variables-formula.md) preserves the angle and changes the radius to

$$
\boxed{Q=\sqrt{-2\log(R^2)}=\sqrt{-2\log U},\qquad\Psi=\Theta.}
$$

The event $R=0$ has probability zero, so arbitrary definitions at that point have no effect on the distribution. For $q\geq0$, monotonicity of the [logarithm](../../../../../logarithm.md) gives

$$
P(Q\leq q)=P(U\geq e^{-q^2/2})=1-e^{-q^2/2},
\qquad f_Q(q)=q e^{-q^2/2}\quad(q>0).
$$

Since $Q$ is a function of $R$, it remains [independent](../../../../../independent-random-variables.md) of the uniform angle. Hence the new [joint probability density](../../../../../joint-probability-density.md) is

$$
\boxed{f_{Q,\Psi}(q,\psi)=\frac{q}{2\pi}e^{-q^2/2},\qquad q>0,\quad0\leq\psi<2\pi.}
$$

Finally, $(X,Y)=(Q\cos\Psi,Q\sin\Psi)$ has polar [Jacobian determinant](../../../../../jacobian-determinant.md) $q$. Dividing the preceding density by $q$ gives the Cartesian [joint probability density](../../../../../joint-probability-density.md)

$$
f_{X,Y}(x,y)=\frac1{2\pi}e^{-(x^2+y^2)/2}
=\left(\frac{e^{-x^2/2}}{\sqrt{2\pi}}\right)
\left(\frac{e^{-y^2/2}}{\sqrt{2\pi}}\right).
$$

This factors into two standard [normal distribution](../../../../../normal-distribution.md) densities on $\mathbb R^2$. Thus **$X$ and $Y$ are independent, each with mean zero and variance one**. This derivation is the radial form of the [Box-Muller transform](../../../../../box-muller-transform.md).

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
