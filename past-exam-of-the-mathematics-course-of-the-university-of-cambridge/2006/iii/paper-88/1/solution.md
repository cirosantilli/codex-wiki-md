<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a [period lattice](../../../../../period-lattice.md) $\Lambda$, define the [Weierstrass elliptic function](../../../../../weierstrass-elliptic-function.md) by

$$
\wp(z)=\frac1{z^2}+\sum_{\omega\in\Lambda\setminus\{0\}}\left(\frac1{(z-\omega)^2}-\frac1{\omega^2}\right).
$$

The subtraction is essential: the separate inverse-square lattice sum need not converge. Let $r$ be the distance to the nearest nonzero lattice point. For $|z|<r$, the [power series](../../../../../power-series.md) identity $(1-w)^{-2}=\sum_{m\geq0}(m+1)w^m$ gives

$$
\frac1{(z-\omega)^2}-\frac1{\omega^2}=\sum_{m\geq1}(m+1)\frac{z^m}{\omega^{m+2}}.
$$

The stipulated convergence allows the sums to be interchanged on smaller disks. Pairing $\omega$ with $-\omega$ cancels odd powers. In terms of the [lattice Eisenstein series](../../../../../lattice-eisenstein-sum.md), this proves the [Laurent coefficients of the Weierstrass elliptic function](../../../../../laurent-coefficients-of-the-weierstrass-elliptic-function.md):

$$
\boxed{\wp(z)=z^{-2}+\sum_{k\geq2}(2k-1)G_{2k}z^{2k-2},\qquad G_{2k}=\sum_{\omega\ne0}\omega^{-2k}.}
$$

For completeness, the function is even and is a [periodic function](../../../../../periodic-function.md): differentiating gives $\wp'(z)=-2\sum_{\omega\in\Lambda}(z-\omega)^{-3}$, which is invariant under translation by a lattice generator. Thus $\wp(z+\omega)-\wp(z)$ is constant. For a primitive generator, evaluating at $z=-\omega/2$ and using evenness makes this constant zero. Two generators establish lattice periodicity. Hence any polynomial in $\wp,\wp'$ is an [elliptic function](../../../../../elliptic-function.md).

Set $c_1=3G_4$ and $c_2=5G_6$. The first terms are $\wp=z^{-2}+c_1z^2+c_2z^4+O(z^6)$. Squaring its derivative and cubing the function give

$$
\wp'^2=4z^{-6}-8c_1z^{-2}-16c_2+O(z^2),\qquad
4\wp^3=4z^{-6}+12c_1z^{-2}+12c_2+O(z^2).
$$

Consequently $H=\wp'^2-4\wp^3+20c_1\wp+28c_2$ has no pole at zero and has value zero there. Lattice periodicity removes the poles at every lattice point; there are no others. Thus $H$ is an [entire function](../../../../../entire-function.md) and an [elliptic function](../../../../../elliptic-function.md), bounded on a closed fundamental parallelogram and therefore throughout the plane. The [Liouville theorem](../../../../../liouville-theorem.md) makes it constant, and its value at zero makes it zero. This proves the [Weierstrass elliptic differential equation](../../../../../weierstrass-elliptic-differential-equation.md)

$$
\boxed{\wp'^2=4\wp^3-g_2\wp-g_3,\qquad g_2=60G_4,\quad g_3=140G_6.}
$$

Differentiating and cancelling $\wp'$ wherever it is nonzero gives $\wp''=6\wp^2-g_2/2$; the identity extends across its isolated zeros by holomorphy. Write $\wp=z^{-2}+\sum_{n\geq1}c_nz^{2n}$. For $n\geq3$, compare coefficients of $z^{2n-2}$:

$$
\big(2n(2n-1)-12\big)c_n=6\sum_{r=1}^{n-2}c_rc_{n-1-r},
\qquad
\boxed{c_n=\frac{3}{(2n+3)(n-2)}\sum_{r=1}^{n-2}c_rc_{n-1-r}.}
$$

The denominator is positive and rational, and $c_1=3G_4,c_2=5G_6$. Induction therefore gives a polynomial with positive rational coefficients on every monomial that occurs. Since $G_{2k}=c_{k-1}/(2k-1)$, the same holds for every $k>3$. This is the [positive polynomial recurrence for lattice Eisenstein sums](../../../../../positive-polynomial-recurrence-for-lattice-eisenstein-sums.md); for example

$$
\boxed{G_8=\frac37G_4^2,\qquad G_{10}=\frac5{11}G_4G_6,\qquad G_{12}=\frac{18}{143}G_4^3+\frac{25}{143}G_6^2.}
$$

Positive coefficients do not assert that the complex values of the lattice sums themselves are positive.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 88](../../paper-88-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
