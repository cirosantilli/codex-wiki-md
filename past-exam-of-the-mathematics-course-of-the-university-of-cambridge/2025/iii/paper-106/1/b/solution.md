<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [holomorphic functional calculus](../../../../../../holomorphic-functional-calculus.md) assigns to every function $f$ holomorphic on a neighbourhood of $\sigma_A(x)$ the element

$$
f(x)=\frac1{2\pi i}\int_\Gamma f(z)(z1-x)^{-1}\,dz,
$$

where the oriented contour $\Gamma$ surrounds the spectrum inside that neighbourhood. The value is independent of the admissible contour, and $f\mapsto f(x)$ is a continuous unital algebra homomorphism sending the coordinate function $z$ to $x$.

Every $\varphi\in\Phi_A$ commutes with the contour integral, so the [Cauchy integral formula](../../../../../../cauchy-integral-formula.md) gives

$$
\varphi(f(x))
=\frac1{2\pi i}\int_\Gamma f(z)(z-\varphi(x))^{-1}\,dz
=f(\varphi(x)).
$$

Part a applied to $f(x)$ now proves the [spectral mapping theorem](../../../../../../spectral-mapping-theorem.md):

$$
\sigma_A(f(x))
=\{\varphi(f(x)): \varphi\in\Phi_A\}
=f(\sigma_A(x)).
$$

Let $\Omega$ be the unbounded component of $\mathbb C\setminus\sigma_A(x)$. On the spectrum, spectral mapping gives

$$
|f(z)|\leq r(f(x))\leq\|f(x)\|.
$$

Every remaining point of $\mathbb C\setminus\Omega$ lies in a bounded complementary component $D$. Its boundary is contained in $\sigma_A(x)$, and $f$ is holomorphic near $\overline D$. The [maximum modulus principle](../../../../../../maximum-modulus-principle.md) therefore extends the same estimate from $\partial D$ to $D$. Hence

$$
\boxed{|f(z)|\leq\|f(x)\|
\qquad(z\in\mathbb C\setminus\Omega).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
