<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Define the [diffusion generator](../../../../../../diffusion-generator.md) $L=b\partial_x+\sigma^2\partial_{xx}/2$. Fix a horizon $t$ and start the strong solution from the deterministic state $x$. The [Itô formula](../../../../../../ito-s-lemma.md) applied to the time-reversed test function gives

$$
d\,u(t-s,X_s)=\bigl[-u_t+Lu\bigr](t-s,X_s)\,ds+\sigma(X_s)u_x(t-s,X_s)\,dW_s.
$$

The drift vanishes by the [Kolmogorov backward equation](../../../../../../kolmogorov-backward-equation.md). This is initially a [local martingale](../../../../../../local-martingale.md); localization on compact state/time sets justifies the [stochastic integral](../../../../../../stochastic-integral.md) without a global derivative bound. Since $u$ itself is bounded, this [local martingale](../../../../../../local-martingale.md) is a true [martingale](../../../../../../martingale-split.md) on $[0,t]$. Its two endpoint expectations give

$$
\boxed{u(t,x)=\mathbb E_x[f(X_t)].}
$$

This is the [bounded backward-equation stochastic representation](../../../../../../bounded-backward-equation-stochastic-representation.md). Starting the strong solution at deterministic $x$ is the precise meaning of the conditional notation at $X_0=x$. Also $f=u(0,\cdot)$ is bounded, even though boundedness was not separately imposed on $f$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
