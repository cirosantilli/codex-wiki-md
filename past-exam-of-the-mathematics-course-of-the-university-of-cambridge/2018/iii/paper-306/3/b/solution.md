<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Jacobi identity for the Poisson bracket](../../../../../../jacobi-identity-for-the-poisson-bracket.md) implies

$$
\bigl(f_{ij}{}^l f_{kl}{}^m+f_{jk}{}^l f_{il}{}^m
+f_{ki}{}^l f_{jl}{}^m\bigr)\varphi_m=0.
$$

For [first-class constraints](../../../../../../first-class-constraint.md) with [linearly independent](../../../../../../linear-independence.md) differentials this gives $f_{[ij}{}^l f_{k]l}{}^m=0$, the [Jacobi identity](../../../../../../jacobi-identity.md) for the [structure constants](../../../../../../structure-constant.md) of the [constraint algebra](../../../../../../constraint-algebra.md). Independence is an implicit assumption: for constraints obeying identities or vanishing identically, only the contracted identity follows, and arbitrary coefficients multiplying such constraints need not satisfy a [Lie algebra](../../../../../../lie-algebra-split.md) identity.

With $G=\epsilon^i\varphi_i$ and $\delta F=\{F,G\}$, the [canonical variables](../../../../../../canonical-variables.md) transform as

$$
\boxed{\delta q^I=\epsilon^i\frac{\partial\varphi_i}{\partial p_I},\qquad
\delta p_I=-\epsilon^i\frac{\partial\varphi_i}{\partial q^I}.}
$$

To fix the sign convention, vary the [phase-space action](../../../../../../phase-space-action.md) directly:

$$
\delta I=\bigl[p_I\delta q^I-\epsilon^i\varphi_i\bigr]_{t_i}^{t_f}
+\int dt\,\bigl(\dot\epsilon^i+\epsilon^j\lambda^k f_{jk}{}^i-\delta\lambda^i\bigr)\varphi_i.
$$

Thus action invariance requires $\delta\lambda^i=\dot\epsilon^i+\epsilon^j\lambda^k f_{jk}{}^i$. For $F^i=\lambda^i-\bar\lambda^i$, the [Faddeev-Popov determinant](../../../../../../faddeev-popov-determinant.md) is that of

$$
\mathcal M^i{}_j=\delta^i_j\partial_t+\bar\lambda^k f_{jk}{}^i.
$$

Using anticommuting [Faddeev-Popov ghost fields](../../../../../../faddeev-popov-ghost.md), the invariant-convention result is

$$
\boxed{I_{\mathrm{FP}}=i\int dt\,b_i
\bigl(\dot c^i+c^j\bar\lambda^k f_{jk}{}^i\bigr).}
$$

**The original PDF has a sign error in the stated multiplier transformation; the TeX transcription has the consistent plus sign.** Keeping the PDF's displayed minus sign mechanically would instead give $i\int dt\,b_i(\dot c^i-c^j\bar\lambda^k f_{jk}{}^i)$. That expression exponentiates the determinant of the printed transformation, but that transformation does not preserve the stated [action](../../../../../../action.md) with the canonical convention above. It cannot be used as the invariant result without changing another convention consistently.

As for the particle, constant multiplier moduli and any residual [zero mode in field theory](../../../../../../zero-mode-in-field-theory.md) must be handled separately; the constant [gauge fixing](../../../../../../gauge-fixing.md) is understood locally on the [gauge orbit](../../../../../../gauge-orbit.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 306](../../../paper-306-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
