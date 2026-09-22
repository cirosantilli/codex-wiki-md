<h1 id="8b/solution">Solution</h1>

↑ **Parent:** [8B](../8b.md)

Near zero the integrand is asymptotic to $t^{z-1}/2$, and at infinity it decays exponentially. The defining integral therefore converges and is analytic for **$\operatorname{Re}z>0$**, by locally uniform domination, also allowing logarithmic factors for differentiation. Multiplication by the [entire function](../../../../../entire-function.md) $1/\Gamma(z)$ does not enlarge the domain of the unevaluated integral itself.

On $\operatorname{Re}z>1$, subtract the two convergent integrals and use

$$
\frac1{e^t+1}-\frac1{e^t-1}=-\frac2{e^{2t}-1}.
$$

The substitution $s=2t$ gives $I(z)-\zeta(z)=-2^{1-z}\zeta(z)$. Thus

$$
\boxed{I(z)=(1-2^{1-z})\zeta(z),}
$$

first there and then wherever the two analytic continuations agree. The [Riemann zeta function](../../../../../riemann-zeta-function.md) is [meromorphic](../../../../../meromorphic-function.md) on the plane with its only pole a simple pole at one. The prefactor has a simple zero there, $1-2^{1-z}=(z-1)\log2+O((z-1)^2)$. It cancels the pole, giving $I(1)=\log2$. Elsewhere both factors are [holomorphic](../../../../../complex-differentiability-at-a-point.md). **The [analytic continuation](../../../../../analytic-continuation.md) of $I$ is entire**; it is the [Dirichlet eta function](../../../../../dirichlet-eta-function.md).

## ↑ Ancestors (10)

1. [8B](../8b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
