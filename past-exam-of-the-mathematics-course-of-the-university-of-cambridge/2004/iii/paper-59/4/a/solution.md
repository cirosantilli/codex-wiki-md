<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $p^0=d\tau/d\lambda$. A comoving observer measures photon energy $p=a p^0$, so $q=ap=a^2p^0$. The null condition is $(\delta_{ij}+h_{ij})p^ip^j=(p^0)^2$. Using the stated [Christoffel symbols](../../../../../../christoffel-symbol.md) in the time [geodesic](../../../../../../geodesic.md) equation gives

$$
\frac{dp^0}{d\lambda}=-2\mathcal H(p^0)^2-\frac12h'_{ij}p^ip^j.
$$

Divide by $p^0$ to differentiate with respect to [conformal time](../../../../../../conformal-time.md). The background redshift term cancels when differentiating $a^2p^0$:

$$
q'=a^2\left(\frac{dp^0}{d\tau}+2\mathcal Hp^0\right)
=-\frac{a^2}{2p^0}h'_{ij}p^ip^j.
$$

In the perturbation term use the background relation $p^i/p^0=\widehat n^i$, giving

$$
\boxed{q'=-\frac12q h'_{ij}\widehat n^i\widehat n^j.}
$$

Without [metric tensor](../../../../../../metric-tensor.md) perturbations, both $q$ and the propagation direction are constant along an unperturbed ray. Thus $q'$ and $d\widehat n^i/d\tau$ are first order. Multiplying them by [derivatives](../../../../../../derivative.md) of $f_1$, which is also first order, gives second-order terms. The term $q'df_0/dq$ is first order and must be retained. At linear order the [Collisionless Boltzmann equation](../../../../../../collisionless-boltzmann-equation.md) therefore reads

$$
\frac{\partial f_1}{\partial\tau}+\widehat n^i\partial_i f_1
=\frac12q\frac{df_0}{dq}h'_{ij}\widehat n^i\widehat n^j.
$$

Taking the [Fourier transform](../../../../../../fourier-transform.md) in the spatial coordinates proves

$$
\boxed{f_1'+ik\mu f_1=\frac12qf_0'(q)h'_{ij}\widehat n^i\widehat n^j,
\qquad\mu=\widehat{\mathbf k}\cdot\widehat{\mathbf n}.}
$$

A first-order correction to the propagation velocity multiplying a spatial [derivative](../../../../../../derivative.md) of $f_1$ is likewise second order.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
