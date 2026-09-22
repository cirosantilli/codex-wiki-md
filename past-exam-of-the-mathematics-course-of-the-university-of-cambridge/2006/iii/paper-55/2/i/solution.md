<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The comoving observer's [four-velocity](../../../../../../four-velocity.md) has $u_0=-a$, so its measured photon energy is $E=-u_\mu p^\mu=ap^0$, and the comoving momentum is $q=aE=a^2p^0$. Let $P^i=p^i/p^0=dx^i/d\tau$. The [null geodesic](../../../../../../null-geodesic.md) condition is

$$
(\delta_{ij}+h_{ij})p^ip^j=(p^0)^2.
$$

Divide the temporal [geodesic equation](../../../../../../geodesic-equation.md) by $p^0=d\tau/d\lambda$, and use the supplied [Christoffel symbols](../../../../../../christoffel-symbol.md):

$$
\frac{dp^0}{d\tau}
=-\mathcal H p^0-\mathcal H\frac{(\delta_{ij}+h_{ij})p^ip^j}{p^0}
-\frac12h'_{ij}\frac{p^ip^j}{p^0}
=-2\mathcal H p^0-\frac12p^0h'_{ij}P^iP^j.
$$

Differentiating $q=a^2p^0$ cancels the homogeneous redshift terms. In the remaining first-order term, replace $P^i$ by the unperturbed unit propagation direction $n^i$:

$$
\boxed{\frac{dq}{d\tau}=-\frac12q h'_{ij}n^in^j+O(h^2).}
$$

This is the [synchronous photon momentum redshift](../../../../../../synchronous-photon-momentum-redshift.md). Background physical momentum decreases as $a^{-1}$, while the background comoving momentum stays constant.

The spatial [geodesic equation](../../../../../../geodesic-equation.md) gives $dp^i/d\tau=-2\mathcal H p^i$ in the unperturbed universe. Since the temporal equation gives the identical factor for $p^0$, their ratio $P^i$ is constant at zeroth order. More explicitly, at first order,

$$
\frac{dP^i}{d\tau}=-h'^i{}_j n^j-\Gamma^i{}_{jk}n^jn^k
+\frac12n^i h'_{jk}n^jn^k+O(h^2).
$$

Every displayed term contains a [metric perturbation](../../../../../../linearized-gravity.md) or its derivative. The orthonormal-frame unit direction differs from $P^i$ by a first-order metric correction, $n^i=P^i+h^i{}_jP^j/2+O(h^2)$, whose derivative is also first order. Hence **$dn^i/d\tau=O(h)$**, with no background change of direction. Direction corrections multiplied by an already first-order source contribute only at second order.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
