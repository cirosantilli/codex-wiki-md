<h1 id="section-b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [orthogonal projection](../../../../../orthogonal-projection.md) onto the full spin-$\eta$ subspace is

$$
\Pi_\eta=|\eta\rangle\langle\eta|\otimes I_{\mathrm{osc}}
=\sum_{\{n'\}}|\eta,\{n'\}\rangle\langle\eta,\{n'\}|.
$$

Here the identity acts on all oscillator states. The finite-time [scattering operator](../../../../../s-matrix.md) $S(t)$ in the question is the [interaction picture](../../../../../interaction-picture.md) [time-evolution operator](../../../../../time-evolution-operator.md), so $|\psi_\sigma^I(t)\rangle=S(t)|\sigma,\{n\}\rangle$. Projecting its two orthogonal spin components yields

$$
\boxed{c_{\eta\sigma}(t)|\phi_\eta(t)\rangle
=\Pi_\eta S(t)|\sigma,\{n\}\rangle.}
$$

Expand the right-hand side in the [orthonormal basis](../../../../../orthonormal-basis.md) $|\eta,\{n'\}\rangle$. Taking its squared [norm](../../../../../norm.md), and using the normalization of $|\phi_\eta\rangle$, gives

$$
\boxed{|c_{\eta\sigma}(t)|^2
=\sum_{\{n'\}}|\langle\eta,\{n'\}|S(t)|\sigma,\{n\}\rangle|^2
=\sum_{\{n'\}}P_{\sigma,\{n\}\to\eta,\{n'\}}.}
$$

Thus one sums [probabilities](../../../../../probability.md) over unobserved final oscillator states, not their [probability amplitudes](../../../../../probability-amplitude.md). [Unitarity](../../../../../unitary-operator.md) of $S(t)$ makes the sum over both $\eta$ equal to one.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [6](../../6.md)
3. [Section B](../../../section-b.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the advanced quantum physics course of the University of Cambridge](../../../../split.md)
6. [Advanced Quantum Physics course of the University of Cambridge](../../../../../advanced-quantum-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
