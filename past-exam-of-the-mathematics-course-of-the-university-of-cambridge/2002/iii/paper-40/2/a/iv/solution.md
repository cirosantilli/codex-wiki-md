<h1 id="2/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Put $A=\int|\theta(x)|f(x)\,dx$, with $0<A<\infty$. The [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md) applied to $|\theta|f/\sqrt g$ and $\sqrt g$ gives

$$
A^2\leq\left(\int\frac{\theta^2f^2}{g}\right)\left(\int g\right)=\int\frac{\theta^2f^2}{g}.
$$

Equality holds exactly when $|\theta|f/\sqrt g$ is proportional to $\sqrt g$ on the contributing [probability support](../../../../../../../support-of-a-probability-distribution.md). Therefore the [minimum-variance importance distribution](../../../../../../../minimum-variance-importance-distribution.md) is

$$
\boxed{g_0(x)=\frac{|\theta(x)|f(x)}A,\qquad\min_g\operatorname{Var}(\widehat\mu_g)=\frac{A^2-\mu^2}{n}.}
$$

If $\theta$ has one sign, $A=|\mu|$ and the ideal proposal gives zero [variance](../../../../../../../variance-split.md). Its normalization or exact sampling may nevertheless be impractical. If $A=0$, the integrand vanishes almost everywhere and the [estimator](../../../../../../../estimator.md) is identically zero.

The minimizing [probability density function](../../../../../../../probability-density-function.md) may vanish where $\theta=0$ even though $f>0$ there. This is valid for the ordinary [estimator](../../../../../../../estimator.md), which needs [probability support](../../../../../../../support-of-a-probability-distribution.md) only for its integrand. If one insists on exactly the same positive [probability support](../../../../../../../support-of-a-probability-distribution.md) as $f$, the bound is instead an infimum whenever this vanishing occurs, approached by $g_\delta=(1-\delta)g_0+\delta f$ as $\delta\downarrow0$: because $g_\delta\geq(1-\delta)g_0$, the second moment lies between $A^2$ and $A^2/(1-\delta)$, proving convergence to the bound.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 40](../../../../paper-40-split.md)
5. [Iii](../../../../split.md)
6. [2002](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
