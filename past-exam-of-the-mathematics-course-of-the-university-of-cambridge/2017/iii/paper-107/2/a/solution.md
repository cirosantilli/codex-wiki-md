<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume an [interior sphere condition](../../../../../../interior-sphere-condition.md) at $y$, and assume the coefficients are bounded and the principal part defines a [uniformly elliptic operator](../../../../../../uniformly-elliptic-operator.md) near its tangent [Euclidean ball](../../../../../../euclidean-ball.md). Shrinking the [Euclidean ball](../../../../../../euclidean-ball.md) while keeping it tangent if necessary, arrange that $\overline{B_R(z)}\setminus\{y\}\subset\Omega$. Write $\nu=(y-z)/R$, the outward radial direction. The conclusion of the [Hopf boundary point lemma](../../../../../../hopf-lemma.md) in the regularity stated in the question is

$$
\boxed{\liminf_{t\downarrow0}\frac{u(y)-u(y-t\nu)}{t}>0.}
$$

If the one-sided [normal derivative](../../../../../../normal-derivative.md) exists, this says $\partial_\nu u(y)>0$. For a $C^1$ boundary its outward normal agrees with the tangent [Euclidean ball](../../../../../../euclidean-ball.md)'s radial normal. Continuity alone does not guarantee that the derivative exists, so its existence must be added when asserting a finite derivative.

On the annulus $R/2<r=|x-z|<R$, use the barrier

$$
h(x)=e^{-kr^2}-e^{-kR^2}>0.
$$

The operator has no zeroth-order term, and differentiation gives

$$
Lh=e^{-kr^2}\left(4k^2a^{ij}(x_i-z_i)(x_j-z_j)-2k\operatorname{tr}a-2kb^i(x_i-z_i)\right)>0
$$

for sufficiently large $k$: the quadratic-in-$k$ term is at least $k^2\lambda R^2$, while the remaining terms are bounded multiples of $k$.

On the inner sphere, compactness and strict inequality give a positive minimum of $u(y)-u(x)$. Choose $\varepsilon>0$ small enough that $u-u(y)+\varepsilon h\leq0$ there. The same inequality holds on the outer sphere since $h=0$. The [weak maximum principle for elliptic operators](../../../../../../weak-maximum-principle-for-elliptic-operators.md) yields $u-u(y)+\varepsilon h\leq0$ throughout the annulus. Along the inward radius,

$$
\frac{u(y)-u(y-t\nu)}{t}\geq\varepsilon\frac{e^{-k(R-t)^2}-e^{-kR^2}}{t}
\longrightarrow2\varepsilon kRe^{-kR^2}>0.
$$

This proves the lemma. The [interior sphere condition](../../../../../../interior-sphere-condition.md) supplies precisely the geometry needed for the barrier; no global boundary regularity is used.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
