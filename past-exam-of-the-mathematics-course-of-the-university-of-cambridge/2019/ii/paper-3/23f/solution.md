<h1 id="23f/solution">Solution</h1>

↑ **Parent:** [23F](../23f.md)

Let $\pi:\mathbb C\to\mathbb C/\Lambda$ be the [universal covering map](../../../../../universal-cover.md). Since the [complex plane](../../../../../complex-plane.md) is a [simply connected domain](../../../../../simply-connected-domain.md), the [lifting criterion for a covering space](../../../../../lifting-criterion-for-a-covering-space.md) gives a [holomorphic lift between one-dimensional complex tori](../../../../../affine-lift-of-a-holomorphic-map-between-one-dimensional-complex-tori.md) $F:\mathbb C\to\mathbb C$ such that

$$
\pi\circ F=f\circ\pi.
$$

For every $\lambda\in\Lambda$, the difference $F(z+\lambda)-F(z)$ belongs to the discrete [period lattice](../../../../../period-lattice.md) $\Lambda$. It depends continuously on $z$, so it is constant. Differentiating shows that the [derivative](../../../../../derivative.md) $F'$ is $\Lambda$-periodic. It is bounded on the compact closure of a [fundamental parallelogram](../../../../../fundamental-parallelogram-of-a-period-lattice.md), and periodicity makes it bounded on all of $\mathbb C$. The [Liouville theorem](../../../../../liouville-theorem.md) therefore makes $F'$ constant, and hence

$$
F(z)=az+b.
$$

Thus every holomorphic map has an [affine lift of a holomorphic map between one-dimensional complex tori](../../../../../affine-lift-of-a-holomorphic-map-between-one-dimensional-complex-tori.md). If “map of complex tori” means an identity-preserving map, choose $F(0)=0$; then $b=0$, so $F$ is the required [linear map](../../../../../linear-map.md). Without that convention the statement must say affine, since a nonzero [translation in a group](../../../../../translation-in-a-group.md) of the torus lifts to $z\mapsto z+b$.

The [Weierstrass elliptic function](../../../../../weierstrass-elliptic-function.md) of $\Lambda$ is

$$
\wp_\Lambda(z)=\frac1{z^2}+
\sum_{\omega\in\Lambda\setminus\{0\}}
\left(\frac1{(z-\omega)^2}-\frac1{\omega^2}\right).
$$

The subtracted term gives the [Normal convergence of the Weierstrass elliptic-function series](../../../../../normal-convergence-of-the-weierstrass-elliptic-function-series.md) away from $\Lambda$. Put

$$
G_{2r}=\sum_{\omega\in\Lambda\setminus\{0\}}\omega^{-2r}.
$$

The [Laurent coefficients of the Weierstrass elliptic function](../../../../../laurent-coefficients-of-the-weierstrass-elliptic-function.md) at zero give

$$
\wp(z)=z^{-2}+3G_4z^2+5G_6z^4+O(z^6),
\qquad
\wp'(z)=-2z^{-3}+6G_4z+20G_6z^3+O(z^5).
$$

Set $g_2=60G_4$ and $g_3=140G_6$. Direct substitution shows that the principal part and constant term of

$$
H(z)=\wp'(z)^2-4\wp(z)^3+g_2\wp(z)+g_3
$$

vanish at zero. Since $H$ is an [elliptic function](../../../../../elliptic-function.md), translation gives the same cancellation at every point of the [period lattice](../../../../../period-lattice.md). Every apparent [isolated singularity](../../../../../isolated-singularity-split.md) is therefore a [removable singularity](../../../../../removable-singularity.md), so $H$ is an [entire function](../../../../../entire-function.md). It is periodic and hence bounded on the translates of a compact [fundamental parallelogram](../../../../../fundamental-parallelogram-of-a-period-lattice.md). The [Liouville theorem](../../../../../liouville-theorem.md) gives $H=0$, which proves the [Weierstrass elliptic differential equation](../../../../../weierstrass-elliptic-differential-equation.md)

$$
\boxed{\wp'(z)^2=4\wp(z)^3-g_2\wp(z)-g_3.}
$$

Finally suppose that $f$ is a biholomorphic [group homomorphism](../../../../../group-homomorphism.md). Its identity-preserving lift has the form $F(z)=\zeta z$ by the first part. Since the inverse map also lifts linearly,

$$
\zeta\Lambda=\Lambda.
$$

Choose a $\mathbb Z$-basis of $\Lambda$. Multiplication by $\zeta$ is then represented by a [unimodular matrix](../../../../../unimodular-matrix.md) $A\in\operatorname{GL}_2(\mathbb Z)$. As a real-linear transformation of $\mathbb C$, it has [determinant](../../../../../determinant.md) $|\zeta|^2>0$; hence $\det A=1$ and $|\zeta|=1$. The [characteristic polynomial](../../../../../characteristic-polynomial.md) of $A$ and the [Cayley-Hamilton theorem](../../../../../cayley-hamilton-theorem.md) give

$$
\zeta^2-\operatorname{tr}(A)\zeta+1=0.
$$

This already has the required form with $m=-\operatorname{tr}(A)\in\mathbb Z$ and $n=1$. Moreover $2\operatorname{Re}\zeta=\operatorname{tr}(A)$, so $|\zeta|=1$ forces $\operatorname{tr}(A)\in\{-2,-1,0,1,2\}$. Thus $\zeta$ is a [root of unity](../../../../../root-of-unity.md), of order $1$, $2$, $3$, $4$, or $6$, completing the description of an [automorphism of a one-dimensional complex torus](../../../../../automorphism-of-a-one-dimensional-complex-torus.md).

## ↑ Ancestors (10)

1. [23F](../23f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
