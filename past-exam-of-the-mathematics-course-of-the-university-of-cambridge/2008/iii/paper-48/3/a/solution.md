<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Maxwell field](../../../../../../electromagnetic-field.md) has the [gauge symmetry](../../../../../../gauge-invariance.md) $A_\mu\mapsto A_\mu+\partial_\mu\alpha(x)$ for an arbitrary smooth scalar function $\alpha$. Commuting the two derivatives shows that $F_{\mu\nu}$ is unchanged, so the [Maxwell Lagrangian](../../../../../../maxwell-lagrangian.md) is invariant. Vary the action, use antisymmetry of $F$ and integrate by parts with variations vanishing on the boundary:

$$
\delta S=-\frac12\int d^4x\,F^{\mu\nu}\delta F_{\mu\nu}
=-\int d^4x\,F^{\mu\nu}\partial_\mu\delta A_\nu
=\int d^4x\,(\partial_\mu F^{\mu\nu})\delta A_\nu.
$$

The [Euler-Lagrange field equations](../../../../../../euler-lagrange-field-equation.md) are therefore $\partial_\mu F^{\mu\nu}=0$. Expanding $F$ gives

$$
\Box A^\nu-\partial^\nu(\partial_\mu A^\mu)=0,
\qquad \Box=\partial_\mu\partial^\mu.
$$

In [Lorenz gauge](../../../../../../lorenz-gauge-condition.md) the second term vanishes, leaving

$$
\boxed{\Box A_\nu=0.}
$$

The PDF calls this “Lorentz gauge”; the standard name is [Lorenz gauge](../../../../../../lorenz-gauge-condition.md). A residual [gauge symmetry](../../../../../../gauge-invariance.md) preserves this condition when $\Box\alpha=0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
