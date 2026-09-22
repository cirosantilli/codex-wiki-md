<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [metric signature](../../../../../../metric-signature.md) $(-,+,+,+)$ and units $c=1$. Write $\dot x^\mu=dx^\mu/d\lambda$ in this part. Varying the [worldline einbein](../../../../../../worldline-einbein.md), without first fixing it, gives

$$
0=\frac{\partial L}{\partial e}=\frac m2\left(-\frac{g_{\mu\nu}\dot x^\mu\dot x^\nu}{e^2}-1\right),\qquad \boxed{g_{\mu\nu}\dot x^\mu\dot x^\nu=-e^2.}
$$

The canonical four-momentum is $p_\mu=mg_{\mu\nu}\dot x^\nu/e$, so the same [mass shell](../../../../../../mass-shell.md) constraint is the [mass shell](../../../../../../mass-shell.md) $g^{\mu\nu}p_\mu p_\nu=-m^2$.

The [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) for the trajectory is

$$
\frac{d}{d\lambda}\left(\frac{g_{\mu\nu}\dot x^\nu}{e}\right)-\frac1{2e}\partial_\mu g_{\alpha\beta}\dot x^\alpha\dot x^\beta=0.
$$

Multiplying by $e$ and then by the [inverse metric](../../../../../../inverse-metric.md), and collecting the [metric tensor](../../../../../../metric-tensor.md) derivatives into the [Christoffel symbols](../../../../../../christoffel-symbol.md), gives

$$
\boxed{\ddot x^\mu+\Gamma^\mu_{\alpha\beta}\dot x^\alpha\dot x^\beta=\frac{\dot e}{e}\dot x^\mu.}
$$

This is a [geodesic equation](../../../../../../geodesic-equation.md) in a possibly nonaffine parameter.

Under a change of parameter, $e'(\lambda')=e(\lambda)d\lambda/d\lambda'$, so $e\,d\lambda$ is invariant. On the positive branch, the [mass shell](../../../../../../mass-shell.md) constraint identifies this invariant with the [proper time](../../../../../../proper-time.md) increment $ds=\sqrt{-g_{\mu\nu}dx^\mu dx^\nu}=e\,d\lambda$. Choosing $\lambda'=s$ therefore sets $e'=1$. The trajectory equation is then the affinely parametrized [geodesic equation](../../../../../../geodesic-equation.md) and its tangent has norm minus one. This is [proper-time gauge for a massive worldline einbein](../../../../../../proper-time-gauge-for-a-massive-worldline-einbein.md). The [mass shell](../../../../../../mass-shell.md) constraint must still be imposed: fixing $e$ in the action before varying would lose it. A fixed parameter interval can retain a [proper-time modulus](../../../../../../proper-time-modulus.md); here changing to the actual proper-time interval is permitted.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
