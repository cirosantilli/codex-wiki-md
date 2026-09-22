<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Brans-Dicke theory](../../../../../brans-dicke-theory.md) couples a [scalar field](../../../../../scalar-field.md) $\Phi$ to the [Ricci scalar](../../../../../ricci-scalar.md). Assume $\Phi\ne0$, constant $\omega$, matter independent of $\Phi$, and variations of compact support so [boundary terms](../../../../../boundary-term.md) may be discarded. Use the paper's [curvature sign convention](../../../../../curvature-sign-convention.md) and signature $(+---)$. Set $X=g^{ab}\partial_a\Phi\,\partial_b\Phi$ and $\Box\Phi=\nabla_a\nabla^a\Phi$. Define the [stress-energy tensor](../../../../../stress-energy-tensor.md) consistently by

$$
\delta S_m=\frac12\int\sqrt{-g}\,T_{ab}\,\delta g^{ab}\,d^4x
=-\frac12\int\sqrt{-g}\,T^{ab}\,\delta g_{ab}\,d^4x.
$$

This convention fixes the sign of the matter term.

Vary with respect to $g^{ab}$. The [variation of metric volume density](../../../../../variation-of-metric-volume-density.md) contributes $-g_{ab}/2$ times each [scalar](../../../../../scalar.md) Lagrangian, while $\delta R=R_{ab}\delta g^{ab}+g^{ab}\delta R_{ab}$. Applying the [Palatini identity](../../../../../palatini-identity.md) followed by two rounds of [integration by parts](../../../../../integration-by-parts.md) gives the [metric variation of a scalar-curvature coupling](../../../../../metric-variation-of-a-scalar-curvature-coupling.md),

$$
\delta\int\sqrt{-g}\,\Phi R\,d^4x
=\int\sqrt{-g}\left[
\Phi G_{ab}+\nabla_a\nabla_b\Phi-g_{ab}\Box\Phi
\right]\delta g^{ab}\,d^4x.
$$

The differentiated $\Phi$ terms remain because the [curvature](../../../../../curvature.md) multiplier is not constant. Varying the kinetic term at fixed $\Phi$ gives

$$
\delta\int\sqrt{-g}\,\omega\Phi^{-1}X\,d^4x
=\int\sqrt{-g}\,\omega\Phi^{-1}
\left(\partial_a\Phi\,\partial_b\Phi-\frac12g_{ab}X\right)
\delta g^{ab}\,d^4x.
$$

Combining these terms with the matter variation, the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) is

$$
\boxed{\Phi G_{ab}+\nabla_a\nabla_b\Phi-g_{ab}\Box\Phi
+\omega\Phi^{-1}
\left(\partial_a\Phi\,\partial_b\Phi-\frac12g_{ab}X\right)
=-8\pi G T_{ab}.}
$$

Raising both free indices reproduces the contravariant form, because $\nabla_ag_{bc}=0$.

The independent [scalar](../../../../../scalar.md) variation gives

$$
R-\omega\Phi^{-2}X
-2\omega\nabla_a(\Phi^{-1}\nabla^a\Phi)=0,
$$

or $R+\omega\Phi^{-2}X-2\omega\Phi^{-1}\Box\Phi=0$. The [trace](../../../../../matrix-trace.md) of the [metric tensor](../../../../../metric-tensor.md) equation in four dimensions is

$$
-\Phi R-3\Box\Phi-\omega\Phi^{-1}X=-8\pi G T,
\qquad T=g^{ab}T_{ab}.
$$

Multiplying the [scalar](../../../../../scalar.md) equation by $\Phi$ eliminates the same combination $\Phi R+\omega\Phi^{-1}X$. Thus the [scalar equation of Brans-Dicke theory](../../../../../scalar-equation-of-brans-dicke-theory.md) is

$$
\boxed{(3+2\omega)\Box\Phi=8\pi G T,\qquad
\Box\Phi=\frac{8\pi G}{3+2\omega}\,g_{ab}T^{ab}
\quad(\omega\ne-3/2).}
$$

At the [degenerate coupling of Brans-Dicke theory](../../../../../degenerate-coupling-of-brans-dicke-theory.md), $\omega=-3/2$, the combined equations impose $T=0$ instead; division by $3+2\omega$ is unavailable. If matter depended directly on $\Phi$, its [scalar](../../../../../scalar.md) variation would add a source and the displayed [scalar](../../../../../scalar.md) equation would change.

The following lettered sections justify the supplied variation identities; they are supporting identities in the PDF, rather than three independent field-equation problems.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
