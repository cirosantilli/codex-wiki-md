<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Define the [stress-energy tensor](../../../../../../../stress-energy-tensor.md) by [metric variation](../../../../../../../metric-variation.md) with the scalar held fixed:

$$
\delta S=\frac12\int d^4x\,\sqrt{-g}\,T^{ab}\delta g_{ab}.
$$

Use compactly supported variations to remove boundary terms. The first [covariant derivative](../../../../../../../covariant-derivative.md) of a [scalar field](../../../../../../../scalar-field.md) is an ordinary derivative, so it has no connection variation. Varying the kinetic term and the [volume form](../../../../../../../volume-form.md) gives

$$
T^{\mathrm{kin}}_{ab}=\nabla_a\Phi\nabla_b\Phi-\frac12g_{ab}\nabla_c\Phi\nabla^c\Phi.
$$

For the curvature term set $f=\Phi^2$. Using part (a), its variation is

$$
\delta S_\xi=-\xi\int\sqrt{-g}\left[
\left(\frac12Rf\,g^{ab}-fR^{ab}\right)h_{ab}
-f\Box h+f\nabla^a\nabla^b h_{ab}\right]d^4x.
$$

Applying [integration by parts](../../../../../../../integration-by-parts.md) twice moves each pair of derivatives from the metric variation onto $f$. The result is

$$
\delta S_\xi=\xi\int\sqrt{-g}
\left[fG^{ab}+g^{ab}\Box f-\nabla^a\nabla^b f\right]h_{ab}\,d^4x,
$$

where $G_{ab}=R_{ab}-Rg_{ab}/2$ is the [Einstein tensor](../../../../../../../einstein-tensor.md) and $\Box=\nabla^c\nabla_c$ is the [d'Alembert operator](../../../../../../../d-alembert-operator.md). Comparing with the defining variation gives the [stress-energy tensor of a nonminimally coupled scalar field](../../../../../../../stress-energy-tensor-of-a-nonminimally-coupled-scalar-field.md):

$$
\boxed{T_{ab}=\nabla_a\Phi\nabla_b\Phi
-\frac12g_{ab}(\nabla\Phi)^2
+2\xi\left[\Phi^2G_{ab}+g_{ab}\Box(\Phi^2)-\nabla_a\nabla_b(\Phi^2)\right].}
$$

The factor $2\xi$ follows from the action's coupling $-\xi R\Phi^2$; a convention using $-\xi R\Phi^2/2$ would instead give $\xi$ in that bracket. At $\xi=0$ this reduces to the massless [Klein-Gordon scalar stress-energy tensor](../../../../../../../klein-gordon-scalar-stress-energy-tensor.md).

## ↑ Ancestors (12)

1. [I](../i.md)
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
