<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [canonical anticommutation relations](../../../../canonical-anticommutation-relations.md) are

$$
\{a_{\mathbf p}^s,a_{\mathbf q}^{r\dagger}\}
=\{b_{\mathbf p}^s,b_{\mathbf q}^{r\dagger}\}
=(2\pi)^3\delta^{sr}\delta^{(3)}(\mathbf p-\mathbf q),
$$

with the mixed and equal-type [anticommutators](../../../../anticommutator.md) zero. Insert the [mode expansion of a Dirac field](../../../../mode-expansion-of-a-dirac-field.md). The phases cancel at equal time, and [a](../a.md) gives

$$
\begin{aligned}
\{\psi_\alpha(t,\mathbf y),\psi_\beta^\dagger(t,\mathbf x)\}
&=\int\frac{d^3p}{(2\pi)^3}\,e^{i\mathbf p\cdot(\mathbf y-\mathbf x)}
\frac{\sum_s[u^s_\alpha(\mathbf p)u^{s*}_\beta(\mathbf p)
+v^s_\alpha(-\mathbf p)v^{s*}_\beta(-\mathbf p)]}{2E}\\
&=\delta_{\alpha\beta}\delta^{(3)}(\mathbf x-\mathbf y).
\end{aligned}
$$

Since $\bar\psi\gamma^0=\psi^\dagger$, the requested componentwise answer is

$$
\boxed{\{(i\bar\psi\gamma^0)_\alpha(t,\mathbf x),\psi_\beta(t,\mathbf y)\}
=i\delta_{\alpha\beta}\delta^{(3)}(\mathbf x-\mathbf y).}
$$

This is the [Equal-time canonical anticommutator of a Dirac field](../../../../equal-time-canonical-anticommutator-of-a-dirac-field.md): the [canonical momentum](../../../../canonical-momentum.md) conjugate to $\psi_\alpha$ is $\pi_\alpha=i\psi_\alpha^\dagger$. It is the fermionic counterpart of the canonical field [canonical commutation relation](../../../../canonical-commutation-relation.md), ensuring the correct local [canonical quantization](../../../../canonical-quantization.md). For this first-order [Lagrangian density](../../../../lagrangian-density.md), the conjugate variables are constrained; the displayed relation is the standard result after handling that constraint. It does not assert a nonzero [anticommutator](../../../../anticommutator.md) between the fields at separated spatial points.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
