<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A gauge-invariant observable is [BRST-closed](../../../../../../brst-closed-operator.md): replacing its infinitesimal gauge parameter by the ghost gives $s\mathcal O=0$. Change the gauge functional continuously, or interpolate between two admissible choices, by changing the [gauge-fixing fermion](../../../../../../gauge-fixing-fermion.md) to $\Psi_t$. The action changes by the [BRST-exact operator](../../../../../../brst-exact-operator.md) $\partial_tS=s(\partial_t\Psi_t)$.

For a normalized correlator of $\mathcal O=\prod_i\mathcal O_i$ with each insertion [BRST-closed](../../../../../../brst-closed-operator.md), differentiation of the [functional integral](../../../../../../functional-measure.md) gives

$$
\partial_t\langle\mathcal O\rangle
=i\left[\langle\mathcal O\,s(\partial_t\Psi_t)\rangle
-\langle\mathcal O\rangle\langle s(\partial_t\Psi_t)\rangle\right].
$$

The [BRST Ward identity](../../../../../../brst-ward-identity.md) says $\langle sX\rangle=0$ for an invariant measure and action, with appropriate boundary conditions. Since $s\mathcal O=0$, the [graded Leibniz rule](../../../../../../graded-leibniz-rule.md) makes the first insertion an exact variation of $\mathcal O\,\partial_t\Psi_t$ up to its harmless parity sign, and both terms vanish. Thus

$$
\boxed{\partial_t\langle\mathcal O_1\cdots\mathcal O_n\rangle=0.}
$$

**Physical gauge-invariant correlation functions are independent of this gauge condition**, even though individual gauge-field and ghost [Feynman diagrams](../../../../../../feynman-diagram.md) change. This argument assumes an admissible perturbative gauge fixing, a [BRST symmetry](../../../../../../brst-symmetry.md)-preserving regulator/measure and no uncanceled boundary contribution. A global failure of those assumptions is not settled by the formal local calculation.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
