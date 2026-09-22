<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the ideal guaranteed-delay model, the total untreated yearly input at $250$ operating days is

$$
D_{y,0}=250(7.992\times10^{11})=1.998\times10^{14} \mathrm{Bq}.
$$

Since the discharge is a decreasing function of the [residence time](../../../../../residence-time.md), the minimum is obtained at equality:

$$
D_{y,0}e^{-\lambda\tau_{\min}}=10^{12},\qquad
\tau_{\min}=\frac{\ln(199.8)}{\lambda}=9308.46 \mathrm s
=\boxed{155.14 \mathrm{min}=2.586 \mathrm h}.
$$

This is $7.642$ [half-lives](../../../../../half-life.md) and corresponds to **$3.444$ L of carbon-dioxide-equivalent delay volume**. The three-hour choice provides margin; operating every day instead would require at least $166.22$ minutes under the same assumptions.

This minimum is conditional on a guaranteed [residence time](../../../../../residence-time.md). More generally the surviving fraction is

$$
\frac{a_{\rm out}}{a_0}=\int_0^\infty E(t)e^{-\lambda t}\,dt,
$$

where $E(t)$ is the [residence time distribution](../../../../../residence-time-distribution.md). Because the [exponential function](../../../../../exponential-function.md) is [convex function](../../../../../convex-function.md), a spread of transit times gives more surviving [radioactive activity](../../../../../radioactive-activity.md) than [plug flow](../../../../../plug-flow.md) at the same mean time. A perfectly mixed continuously flowing vessel has a steady-state survival fraction $1/(1+\lambda V/Q)$, not $e^{-\lambda V/Q}$. Thus no unique minimum _tank filling time_ follows without specifying the filling, retention and emptying schedule. The boxed minimum applies to the explicitly specified delay system, and must not be represented as approval of an unspecified tank.

## ↑ Ancestors (10)

1. [D](../d.md)
2. [2](../../2.md)
3. [Module NE4](../../../paper-ne4-split.md)
4. [2021](../../../split.md)
5. [Past exam of the MPhil in nuclear energy course of the University of Cambridge](../../../../split.md)
6. [MPhil in nuclear energy course of the University of Cambridge](../../../../../mphil-in-nuclear-energy-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
