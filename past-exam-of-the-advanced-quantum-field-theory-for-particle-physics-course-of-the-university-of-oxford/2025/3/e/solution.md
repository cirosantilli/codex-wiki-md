<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

After the quadratic mixing cancellation, the vector inverse quadratic operator is

$$
K=-(k^2-m_A^2)P^T-\left(\frac{k^2}{\xi}-m_A^2\right)P^L.
$$

Inverting its two [orthogonal projectors](../../../../orthogonal-projection.md) and multiplying by $i$ gives

$$
\boxed{D^{(\xi)}_{\mu\nu}(k)=\frac{-i}{k^2-m_A^2+i0}
\left[g_{\mu\nu}-(1-\xi)\frac{k_\mu k_\nu}{k^2-\xi m_A^2+i0}\right].}
$$

Equivalently $D^{(\xi)}=-iP^T/(k^2-m_A^2+i0)-i\xi P^L/(k^2-\xi m_A^2+i0)$. At fixed finite $\xi$, both sectors fall as $k^{-2}$ at large [momentum](../../../../momentum-split.md) in [Euclidean space](../../../../euclidean-norm.md); $\xi=1$ gives $-ig_{\mu\nu}/(k^2-m_A^2+i0)$, and taking $\xi\to\infty$ at fixed $k$ recovers [unitary gauge](../../../../unitary-gauge.md). The latter limit is not uniform in [ultraviolet](../../../../ultraviolet.md) [momentum](../../../../momentum-split.md).

The expected [power counting](../../../../power-counting-in-quantum-field-theory.md) conclusion is that this $k^{-2}$ behaviour, together with polynomial interactions of [mass dimension](../../../../mass-dimension.md) at most four in Cartesian scalar variables and the [gauge symmetry](../../../../gauge-invariance.md) identities, permits [renormalization of spontaneously broken gauge theories](../../../../renormalization-of-spontaneously-broken-gauge-theories.md) using a finite set of physical parameters. **The propagator alone is not sufficient to establish that claim in the polar variables of this question.** In fact, part [b](../b.md) contains $h(\partial\pi)^2/f$ and $h^2(\partial\pi)^2/(2f^2)$, of dimensions five and six, and the nonlinear [gauge fixing](../../../../gauge-fixing.md) term contains $-\xi e^2h^4\pi^2/(2f^2)$, also of dimension six. Ordinary [power counting](../../../../power-counting-in-quantum-field-theory.md) is consequently not manifest in these variables.

For a representation where it is manifest, write $\phi=(f+H+i\chi)/\sqrt2$ and choose the usual polynomial [R-xi gauge](../../../../r-xi-gauge.md) function $\partial\cdot A-\xi ef\chi$. It yields the same free vector [propagator](../../../../propagator.md), cancels the quadratic mixing, and leaves only dimension-at-most-four interactions, including its [Faddeev-Popov ghosts](../../../../faddeev-popov-ghost.md). This supplies the missing vertex condition in the source's proposed inference; the [equivalence theorem for field redefinitions](../../../../equivalence-theorem-for-field-redefinitions.md) relates physical predictions near the [vacuum](../../../../vacuum.md). Good [propagator](../../../../propagator.md) falloff is the necessary ingredient illustrated by the requested formula, rather than a complete proof for arbitrary parametrizations or nonlinear choices of [gauge fixing](../../../../gauge-fixing.md).

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
