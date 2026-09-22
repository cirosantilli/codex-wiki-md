<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Thomson principle](../../../../../../thomson-principle.md) states that the effective resistance is the minimum energy of a unit flow from $a$ to $z$:

$$
R_{\mathrm{eff}}(a,z)=\inf_\theta
\sum_e\frac{\theta(e)^2}{c(e)}.
$$

An edge cutset separating $a$ and $z$ is a set of edges whose removal disconnects them. Every unit flow has net flux one across each such cutset $\Pi_k$. By [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md),

$$
1=\left(\sum_{e\in\Pi_k}\theta(e)\right)^2
\leq\left(\sum_{e\in\Pi_k}\frac{\theta(e)^2}{c(e)}\right)
\left(\sum_{e\in\Pi_k}c(e)\right).
$$

For disjoint cutsets, summing these energy lower bounds and applying Thomson's principle gives the [Nash-Williams inequality](../../../../../../nash-williams-inequality.md)

$$
R_{\mathrm{eff}}(a,z)
\geq\sum_{k=1}^m\left(\sum_{e\in\Pi_k}c(e)\right)^{-1}.
$$

The [commute time identity](../../../../../../commute-time-identity.md) is

$$
\boxed{\mathbb E_aT_z+\mathbb E_zT_a
=2\left(\sum_{e\in E}c(e)\right)R_{\mathrm{eff}}(a,z).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
