<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For the [period lattice](../../../../../period-lattice.md) $\Lambda=\mathbb Z\omega_1+\mathbb Z\omega_2$, define the [Weierstrass elliptic function](../../../../../weierstrass-elliptic-function.md) by

$$
\wp(z)=\frac1{z^2}+\sum_{0\ne\omega\in\Lambda}\left(\frac1{(z-\omega)^2}-\frac1{\omega^2}\right).
$$

On a [compact set](../../../../../compact-space.md) away from $\Lambda$, the summand is $O(|\omega|^{-3})$ uniformly for sufficiently large $|\omega|$. The permitted lattice convergence estimate therefore gives [Normal convergence of the Weierstrass elliptic-function series](../../../../../normal-convergence-of-the-weierstrass-elliptic-function-series.md). Consequently $\wp$ is a [meromorphic function](../../../../../meromorphic-function.md), with a double [pole](../../../../../pole.md) of principal part $(z-\omega)^{-2}$ at each lattice point and no other [poles](../../../../../pole.md). Termwise differentiation gives the normally and absolutely convergent series

$$
\wp'(z)=-2\sum_{\omega\in\Lambda}(z-\omega)^{-3}.
$$

Pairing $\omega$ with $-\omega$ shows that $\wp$ is even and $\wp'$ is odd. Reindexing the absolutely convergent derivative series gives $\wp'(z+\lambda)=\wp'(z)$ for every $\lambda\in\Lambda$. Thus $\wp(z+\lambda)-\wp(z)$ is constant, with removable singularities at the lattice points. For either basis period $\lambda=\omega_1,\omega_2$, evaluate at $z=-\lambda/2$: evenness makes this constant [zero](../../../../../zero-of-a-function.md). These two [periods](../../../../../period-of-a-function.md) imply all periods in $\Lambda$. Hence **$\wp$ is a nonconstant [elliptic function](../../../../../elliptic-function.md) with [period lattice](../../../../../period-lattice.md) $\Lambda$.**

To obtain the [Laurent coefficients of the Weierstrass elliptic function](../../../../../laurent-coefficients-of-the-weierstrass-elliptic-function.md), take $0<|z|<\min_{\omega\ne0}|\omega|$ and expand

$$
\frac1{(z-\omega)^2}-\frac1{\omega^2}=\sum_{j\geq1}(j+1)\frac{z^j}{\omega^{j+2}}.
$$

The expansion and lattice summation can be interchanged uniformly on smaller disks, using the same convergent majorant. The odd powers cancel in pairs. In terms of the [lattice Eisenstein sums](../../../../../lattice-eisenstein-sum.md), the answer is

$$
\boxed{\wp(z)=z^{-2}+\sum_{r\geq1}(2r+1)G_{2r+2}(\Lambda)z^{2r}
=z^{-2}+3G_4z^2+5G_6z^4+O(z^6).}
$$

Only the absolutely convergent [lattice Eisenstein sums](../../../../../lattice-eisenstein-sum.md) of weights at least four occur here; no conditionally defined $G_2$ is needed.

Put $g_2=60G_4$ and $g_3=140G_6$. The [Laurent series](../../../../../laurent-series.md) just found gives

$$
\wp'(z)^2-4\wp(z)^3=-60G_4z^{-2}-140G_6+O(z^2).
$$

Therefore $F=\wp'^2-4\wp^3+g_2\wp+g_3$ has no [pole](../../../../../pole.md) at [zero](../../../../../zero-of-a-function.md), and its value there is [zero](../../../../../zero-of-a-function.md). By periodicity it has no [poles](../../../../../pole.md) anywhere. An entire [elliptic function](../../../../../elliptic-function.md) is bounded on a closed [fundamental parallelogram](../../../../../fundamental-parallelogram-of-a-period-lattice.md), hence on the plane, and is constant by [Liouville theorem](../../../../../liouville-theorem.md). Since $F(0)=0$, this proves the [Weierstrass elliptic differential equation](../../../../../weierstrass-elliptic-differential-equation.md)

$$
\wp'^2=4\wp^3-g_2\wp-g_3.
$$

We still need to identify the three roots without assuming their distinctness. For a nonconstant [elliptic function](../../../../../elliptic-function.md) $u$, the [argument principle](../../../../../argument-principle.md) applied to $u'/u$ around a [fundamental parallelogram](../../../../../fundamental-parallelogram-of-a-period-lattice.md) makes the opposite-edge integrals cancel. Thus its [zeros](../../../../../zero-of-a-function.md) and [poles](../../../../../pole.md), counted with [multiplicity](../../../../../multiplicity-mathematics.md), have equal total number. In particular $\wp-a$ has exactly two [zeros](../../../../../zero-of-a-function.md) in a period cell for every finite $a$.

Let $h_i=\omega_i/2$, with $\omega_3=-\omega_1-\omega_2$. Their classes are the three nonzero [two-torsion points of a complex torus](../../../../../two-torsion-point-of-a-complex-torus.md). Oddness and periodicity give $\wp'(h_i)=-\wp'(h_i)$, so $\wp'(h_i)=0$. Thus $\wp-e_i$, where $e_i=\wp(h_i)$, has a [zero](../../../../../zero-of-a-function.md) of [multiplicity](../../../../../multiplicity-mathematics.md) at least two at $h_i$, and the preceding count says its [multiplicity](../../../../../multiplicity-mathematics.md) is exactly two. If two of the [half-period values of the Weierstrass elliptic function](../../../../../half-period-values-of-the-weierstrass-elliptic-function.md) were equal, the same function would have at least four [zeros](../../../../../zero-of-a-function.md), a contradiction. Evaluating the [Weierstrass elliptic differential equation](../../../../../weierstrass-elliptic-differential-equation.md) at the three half-periods now gives three distinct roots of its cubic. Consequently

$$
\boxed{\wp'(z)^2=4\prod_{i=1}^3(\wp(z)-e_i).}
$$

For the remaining identity, fix $i$ and put $A_i=(e_i-e_j)(e_i-e_l)$, where $\{i,j,l\}=\{1,2,3\}$. The [elliptic function](../../../../../elliptic-function.md)

$$
H_i(z)=(\wp(z+h_i)-e_i)(\wp(z)-e_i)
$$

has possible [poles](../../../../../pole.md) only at $z=0,-h_i$ modulo $\Lambda$. At each, the other factor has an exact double [zero](../../../../../zero-of-a-function.md), so these [poles](../../../../../pole.md) are removable. Thus $H_i$ is constant, and its limit at [zero](../../../../../zero-of-a-function.md) is $\wp''(h_i)/2$. Differentiating the cubic [differential equation](../../../../../differential-equation-split.md) first where $\wp'\ne0$, then extending the resulting identity holomorphically, gives $\wp''=6\wp^2-g_2/2$. Since $e_i$ is a root of $P(X)=X^3-g_2X/4-g_3/4$, we obtain

$$
\frac12\wp''(h_i)=3e_i^2-\frac{g_2}{4}=P'(e_i)=A_i,
\qquad
\wp(z+h_i)=e_i+\frac{A_i}{\wp(z)-e_i}.
$$

This proves the [Weierstrass half-period translation formula](../../../../../weierstrass-half-period-translation-formula.md) by [pole](../../../../../pole.md) cancellation. Set $u_i=h_i/2=\omega_i/4$. Since $u_i+h_i\equiv-u_i\pmod\Lambda$, evenness gives $\wp(u_i+h_i)=\wp(u_i)$, and therefore

$$
A_i=(\wp(u_i)-e_i)^2.
$$

The denominator here is nonzero: the only [zero](../../../../../zero-of-a-function.md) of $\wp-e_i$ modulo $\Lambda$ is $h_i$, whereas $u_i$ is not congruent to $h_i$. Finally differentiate the [Weierstrass half-period translation formula](../../../../../weierstrass-half-period-translation-formula.md) and use $z-h_i\equiv z+h_i\pmod\Lambda$ to obtain the [Weierstrass quarter-period derivative identity](../../../../../weierstrass-quarter-period-derivative-identity.md)

$$
\boxed{\frac{\wp'(z-\omega_i/2)}{\wp'(z)}=-\left(\frac{\wp(\omega_i/4)-e_i}{\wp(z)-e_i}\right)^2.}
$$

The equality holds wherever these quotients are initially defined, and hence as an identity of [meromorphic functions](../../../../../meromorphic-function.md) at all remaining points.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
