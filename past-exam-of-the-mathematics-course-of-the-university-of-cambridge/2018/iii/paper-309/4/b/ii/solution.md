<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Euler-Lagrange field equation](../../../../../../../euler-lagrange-field-equation.md) obtained by varying the [nonminimally coupled scalar field](../../../../../../../nonminimally-coupled-scalar-field.md) is

$$
\boxed{\Box\Phi-2\xi R\Phi=0.}
$$

One can check [stress-energy conservation](../../../../../../../stress-energy-conservation.md) directly. The divergence of the kinetic contribution is $(\Box\Phi)\nabla_b\Phi$, because second derivatives of a scalar commute. With $f=\Phi^2$, the [contracted Bianchi identity](../../../../../../../contracted-bianchi-identity.md) gives $\nabla^aG_{ab}=0$, while the [Ricci identity](../../../../../../../curvature-commutator-on-a-covariant-tensor.md) gives

$$
\Box\nabla_bf=\nabla_b\Box f+R_b{}^c\nabla_cf.
$$

Consequently

$$
\begin{aligned}
\nabla^a\left[fG_{ab}+g_{ab}\Box f-\nabla_a\nabla_bf\right]
&=G_{ab}\nabla^af+\nabla_b\Box f-\Box\nabla_bf\\
&=(G_{ab}-R_{ab})\nabla^af=-\frac12R\nabla_bf.
\end{aligned}
$$

Since $\nabla_bf=2\Phi\nabla_b\Phi$, the full [stress-energy tensor](../../../../../../../stress-energy-tensor.md) satisfies

$$
\boxed{\nabla^aT_{ab}=(\Box\Phi-2\xi R\Phi)\nabla_b\Phi=0\quad\text{on shell}.}
$$

The general reason is the [diffeomorphism Noether identity for a scalar field](../../../../../../../diffeomorphism-noether-identity-for-a-scalar-field.md). Under the [Lie derivative](../../../../../../../lie-derivative-of-a-differential-form.md) along a compactly supported [vector field](../../../../../../../vector-field.md) $X$, $\delta g_{ab}=2\nabla_{(a}X_{b)}$ and $\delta\Phi=X^a\nabla_a\Phi$. Invariance of the action under [diffeomorphisms](../../../../../../../diffeomorphism.md) gives, after [integration by parts](../../../../../../../integration-by-parts.md),

$$
0=\int\sqrt{-g}\,X^b\left[-\nabla^aT_{ab}
+\frac1{\sqrt{-g}}\frac{\delta S}{\delta\Phi}\nabla_b\Phi\right]d^4x.
$$

Arbitrariness of $X$ gives the same divergence identity. Conservation requires the scalar equation of motion, with no need to impose the [Einstein field equations](../../../../../../../einstein-field-equations.md) for the background metric.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 309](../../../../paper-309-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
