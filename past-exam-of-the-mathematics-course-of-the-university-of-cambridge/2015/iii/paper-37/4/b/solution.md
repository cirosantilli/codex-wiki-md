<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose a proposal [probability density function](../../../../../../probability-density-function.md) $q$ positive wherever $|h|f$ is nonzero, up to null sets, and draw [independent and identically distributed random variables](../../../../../../independent-and-identically-distributed-random-variables.md) $Y_1,\ldots,Y_n$ from $q$. The ordinary [importance sampling](../../../../../../importance-sampling.md) estimator is

$$
\boxed{\widehat\mu_{\rm IS}=\frac1n\sum_{i=1}^n\frac{h(Y_i)f(Y_i)}{q(Y_i)}.}
$$

The [support condition for importance sampling](../../../../../../support-condition-for-importance-sampling.md) and absolute integrability give $\mathbb E_q[h(Y)f(Y)/q(Y)]=\int hf=\mu$, so this is an [unbiased estimator](../../../../../../unbiased-estimator.md). Its [variance](../../../../../../variance-split.md), possibly infinite, is

$$
\operatorname{Var}(\widehat\mu_{\rm IS})=\frac1n\left[\int\frac{h(x)^2f(x)^2}{q(x)}\,dx-\mu^2\right].
$$

Let $A=\int|h|f$. If $A>0$, the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) yields

$$
A^2=\left(\int\frac{|h|f}{\sqrt q}\sqrt q\right)^2\leq\int\frac{h^2f^2}{q}.
$$

Equality holds for $q$ proportional to $|h|f$. Thus the [minimum-variance importance distribution](../../../../../../minimum-variance-importance-distribution.md) and the minimum [variance](../../../../../../variance-split.md) are

$$
\boxed{q_*(x)=\frac{|h(x)|f(x)}{A},\qquad \operatorname{Var}(\widehat\mu_{\rm IS})_{\min}=\frac{A^2-\mu^2}{n}.}
$$

For a constant-sign integrand this is zero [variance](../../../../../../variance-split.md). If $A=0$, the integrand vanishes almost everywhere and the zero estimator already has zero [variance](../../../../../../variance-split.md). Requiring the proposal to cover all of the target's support, including where $h=0$, can exclude $q_*$; in that stricter class, $(1-\epsilon)q_*+\epsilon f$ approaches the same infimum as $\epsilon\downarrow0$. This distinguishes coverage of the integral from coverage of every target event.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
