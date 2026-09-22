<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the [Witten-Reshetikhin-Turaev invariant](../../../../witten-reshetikhin-turaev-invariant.md) with the source's [normalized Kirby color](../../../../normalized-kirby-color.md) on all $2g+1$ surgery components. Since the [signature](../../../../signature-of-a-quadratic-form.md) of the [linking matrix](../../../../linking-matrix.md) is zero, the framing-anomaly factor is one, and the [TQFT partition function](../../../../topological-quantum-field-theory-partition-function.md) is

$$
Z(\Sigma_g\times S^1)=\frac1{\mathcal D}\,\langle L(\Omega,\ldots,\Omega)\rangle.
$$

All evaluations in this part use the [isotopy normalization of anyon diagrams](../../../../isotopy-normalization-of-anyon-diagrams.md) and preserve the indicated [blackboard framing](../../../../blackboard-framing.md).

Expand the long component as $\mathcal D^{-1}\sum_a d_a a$ and fix its charge $a$. Each pair of auxiliary components is in the [Borromean rings](../../../../borromean-rings.md) arrangement with this component. Eliminate such a pair using the [two-strand Kirby projector](../../../../two-strand-kirby-projector.md) from [c](../c.md): bend the long component to expose its two oppositely oriented portions, viewed as equally oriented strands labeled $a,\bar a$. The first encircling [normalized Kirby color](../../../../normalized-kirby-color.md) loop replaces these by a vacuum cup-cap with coefficient $\mathcal D/d_a$. This vacuum connection opens the second encircling loop so that the same [two-strand Kirby projector](../../../../two-strand-kirby-projector.md) applies once more. Removing the resulting vacuum edges and straightening the bends restores the original charge-$a$ strand. Thus the [Borromean handle-pair evaluation](../../../../borromean-handle-pair-evaluation.md) multiplies the bare strand by

$$
H_a=\left(\frac{\mathcal D}{d_a}\right)^2.
$$

There is no residual twist. This is a relative strand evaluation: the final closure of the long component is counted separately. As a normalization check, when $a=1$ the two auxiliary components become two unlinked [normalized Kirby color](../../../../normalized-kirby-color.md) loops, each of value $\mathcal D$, giving $H_1=\mathcal D^2$.

The $g$ pairs occupy disjoint portions of the long component, so their factors multiply. Closing that component gives its [quantum dimension](../../../../quantum-dimension.md) $d_a$. Combining this with its [normalized Kirby color](../../../../normalized-kirby-color.md) coefficient $d_a/\mathcal D$ gives

$$
\begin{aligned}
\langle L(\Omega,\ldots,\Omega)\rangle
&=\sum_a\frac{d_a}{\mathcal D}\,d_a\left(\frac{\mathcal D^2}{d_a^2}\right)^g\\
&=\mathcal D^{2g-1}\sum_a d_a^{2-2g}.
\end{aligned}
$$

Applying the overall surgery prefactor yields

$$
\boxed{Z(\Sigma_g\times S^1)=\mathcal D^{2g-2}\sum_a d_a^{2-2g}.}
$$

Finally, the [topological quantum field theory](../../../../topological-quantum-field-theory.md) assigns the identity map to a cylinder over $\Sigma_g$. Closing its time direction takes the [trace](../../../../matrix-trace.md) of that identity, so

$$
\boxed{\operatorname{GSD}(\Sigma_g)=\dim V(\Sigma_g)=Z(\Sigma_g\times S^1).}
$$

This independently reproduces [b](../b.md). For $g=0$ the surgery link is one zero-framed [normalized Kirby color](../../../../normalized-kirby-color.md) [unknot](../../../../unknot.md): its value $\mathcal D$ cancels the surgery prefactor and gives $Z(S^2\times S^1)=1$. For $g=1$ the result is the number of simple [anyons](../../../../anyon.md), as required for the [torus](../../../../torus.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the anyons and topological quantum field theories course of the University of Oxford](../../../split.md)
5. [Anyons and topological quantum field theories course of the University of Oxford](../../../../anyons-and-topological-quantum-field-theories-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
