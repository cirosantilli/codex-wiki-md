<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [comoving observer](../../../../../../comoving-observer.md) measures $E=ap^0$, so $q=aE=a^2p^0$. Write $\mathcal H=a'/a$. The [null geodesic](../../../../../../null-geodesic.md) condition implies

$$
(\delta_{ij}+h_{ij})p^ip^j=(p^0)^2.
$$

The time component of the [geodesic equation](../../../../../../geodesic-equation.md), using $d\tau/d\lambda=p^0$, is therefore

$$
\frac{dp^0}{d\tau}
=-\mathcal Hp^0-\frac{\mathcal H(\delta_{ij}+h_{ij})p^ip^j+\tfrac12h'_{ij}p^ip^j}{p^0}
=-2\mathcal Hp^0-\frac{h'_{ij}p^ip^j}{2p^0}.
$$

Differentiate $q=a^2p^0$. The homogeneous expansion terms cancel:

$$
q'=2\mathcal Ha^2p^0+a^2\frac{dp^0}{d\tau}
=-\frac{a^2}{2p^0}h'_{ij}p^ip^j.
$$

At zeroth order $p^i/p^0=n^i$, with $\delta_{ij}n^in^j=1$. The difference between coordinate [velocity](../../../../../../velocity.md) and physical unit direction is already first order and multiplies $h'$, so it can be discarded in this expression. We obtain the [synchronous photon momentum redshift](../../../../../../synchronous-photon-momentum-redshift.md)

$$
\boxed{\frac{dq}{d\tau}=-\frac12q h'_{ij}n^in^j.}
$$

In the unperturbed universe $q$ is constant and physical [photon](../../../../../../photon.md) energy redshifts as $a^{-1}$; the displayed term is the additional anisotropic first-order redshift.

To check the direction, let $v^i=p^i/p^0$. Combining the spatial and temporal [geodesic equations](../../../../../../geodesic-equation.md) cancels their homogeneous Hubble terms and gives

$$
\frac{dv^i}{d\tau}
=-h'^i{}_jv^j-\Gamma^i{}_{jk}v^jv^k
+\frac12v^i h'_{jk}v^jv^k=O(h).
$$

Every remaining connection or explicit metric-derivative term is first order. A local orthonormal spatial frame defines the physical unit vector by $n^i=v^i+\tfrac12h^i{}_jv^j+O(h^2)$. Its derivative adds only first-order terms, so

$$
\boxed{\frac{dn^i}{d\tau}=O(h).}
$$

Consequently direction deflection multiplied by an already first-order [temperature](../../../../../../temperature.md) anisotropy is second order. The first-order brightness calculation may use a straight unperturbed ray without neglecting the first-order gravitational frequency change.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
