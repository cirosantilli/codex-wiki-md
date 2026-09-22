<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [linearization](../../../../../../linearization.md) at the zero solution is the [self-adjoint differential operator](../../../../../../self-adjoint-differential-operator.md) $L=\mu-(\partial_x^2+K)^2$, with domain satisfying both endpoint conditions. The [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) for $-\partial_x^2$ on $(-1,1)$ gives the orthogonal [eigenfunctions](../../../../../../eigenfunction.md) $\cos((n+\tfrac12)\pi x)$ and $\sin((n+1)\pi x)$. Their second derivatives are multiples of themselves, so the additional condition $\psi_{xx}(\pm1)=0$ is automatic. Completeness of the Dirichlet [eigenfunctions](../../../../../../eigenfunction.md) also shows that these exhaust the spectrum of the polynomial operator $L$. Set $q_j=(j+1)\pi/2$; each [eigenfunction](../../../../../../eigenfunction.md) has growth rate $\sigma_j=\mu-(K-q_j^2)^2$. Hence the stationary [bifurcation](../../../../../../bifurcation.md) thresholds are

$$
\boxed{\mu_j(K)=\left(K-\frac{(j+1)^2\pi^2}{4}\right)^2.}
$$

Equality of the first two thresholds requires $K$ to be the midpoint of $\pi^2/4$ and $\pi^2$, since these numbers are distinct. Therefore

$$
\boxed{K^*=\frac{5\pi^2}{8},\qquad \mu^*=\frac{9\pi^4}{64}.}
$$

At this point the even and odd lowest [eigenfunctions](../../../../../../eigenfunction.md) become neutral simultaneously.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
