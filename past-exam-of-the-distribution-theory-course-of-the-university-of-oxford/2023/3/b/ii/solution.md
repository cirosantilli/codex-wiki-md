<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

If $F$ is any other [fundamental solution](../../../../../fundamental-solution-of-a-linear-differential-operator.md), then $H=F-E$ satisfies $\partial_{\bar z}H=0$ as a [distribution](../../../../../distribution-mathematical-analysis.md). Applying $4\partial_z$ gives $\Delta H=0$. [Elliptic regularity](../../../../../elliptic-regularity.md) for the [Laplacian](../../../../../laplacian.md) implies that the initially arbitrary [distribution](../../../../../distribution-mathematical-analysis.md) $H$ is a [smooth function](../../../../../smooth-function.md). Its equation is then the ordinary [Cauchy-Riemann equation](../../../../../cauchy-riemann-equations.md), so $H$ is an [entire function](../../../../../entire-function.md).

For a direct justification of the needed regularity, choose a radial [mollifier](../../../../../mollifier.md) $\eta_r$. Locally, $H*\eta_\varepsilon$ is a smooth [harmonic function](../../../../../harmonic-function.md). On a ball with sufficient room for both radii, the [mean value property](../../../../../mean-value-property-for-harmonic-functions.md) gives $(H*\eta_\varepsilon)*\eta_r=H*\eta_\varepsilon$. Passing to the [weak convergence of distributions](../../../../../weak-convergence-of-distributions.md) limit $\varepsilon\to0$ yields $H*\eta_r=H$ on a smaller ball. The left side is smooth, proving the claim locally. This establishes the [distributional Cauchy-Riemann lemma](../../../../../distributional-cauchy-riemann-lemma.md) without assuming in advance that $H$ is a [locally integrable function](../../../../../locally-integrable-function.md).

Conversely every [entire function](../../../../../entire-function.md) $h$ satisfies $\partial_{\bar z}h=0$ and can be added to $E$. Hence all [fundamental solutions](../../../../../fundamental-solution-of-a-linear-differential-operator.md) are

$$
\boxed{F(z)=\frac1{\pi z}+h(z),\qquad h\text{ any entire function}.}
$$

No growth condition at infinity was imposed, so $h$ need not be a [polynomial](../../../../../polynomial-split.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the distribution theory course of the University of Oxford](../../../../split.md)
6. [Distribution theory course of the University of Oxford](../../../../../distribution-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
