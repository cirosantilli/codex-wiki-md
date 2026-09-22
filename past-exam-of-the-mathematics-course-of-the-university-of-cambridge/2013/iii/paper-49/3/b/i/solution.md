<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take compactly supported [metric variations](../../../../../../../metric-variation.md), or impose [boundary conditions](../../../../../../../boundary-condition.md) that remove the [integration by parts](../../../../../../../integration-by-parts.md) terms. Let $F=f'(R)$ and $\Box=\nabla^a\nabla_a$. Since $\delta\sqrt{-g}=\frac12\sqrt{-g}\,g^{ab}h_{ab}$, the gravitational action varies as

$$
\delta S_g=\int\sqrt{-g}\left[
\left(\frac12f g^{ab}-F R^{ab}\right)h_{ab}
+F\left(\nabla^a\nabla^b h_{ab}-\Box h\right)\right]d^4x.
$$

Applying [integration by parts](../../../../../../../integration-by-parts.md) twice to the derivative terms gives

$$
\delta S_g=-\int\sqrt{-g}\,E^{ab}h_{ab}\,d^4x,\qquad
\boxed{E_{ab}=F R_{ab}-\frac12f g_{ab}-\nabla_a\nabla_bF+g_{ab}\Box F.}
$$

For the usual [stress-energy tensor](../../../../../../../stress-energy-tensor.md) definition $T_{ab}=-2(-g)^{-1/2}\delta S_m/\delta g^{ab}$, varying the covariant [metric tensor](../../../../../../../metric-tensor.md) gives $\delta S_m=\frac12\int\sqrt{-g}\,T^{ab}h_{ab}\,d^4x$. Thus the action's stated normalization implies

$$
\boxed{E_{ab}=\frac12T_{ab}.}
$$

There is no implicit $1/(16\pi)$ in this gravitational action. This is the [normalization of the metric f(R) field equation](../../../../../../../normalization-of-the-metric-f-r-field-equation.md), rather than the commonly normalized version with $8\pi T_{ab}$ on the right.

Finally, the [chain rule](../../../../../../../chain-rule.md) gives $\nabla_a\nabla_bF=f''\nabla_a\nabla_bR+f^{(3)}\nabla_aR\nabla_bR$ and $\Box F=f''\Box R+f^{(3)}(\nabla R)^2$. Substitution yields

$$
\boxed{E_{ab}=f'R_{ab}-f''\nabla_a\nabla_bR-f^{(3)}\nabla_aR\nabla_bR
+\left(-\frac12f+f''\Box R+f^{(3)}\nabla_cR\nabla^cR\right)g_{ab}.}
$$

This is a metric [f(R) gravity](../../../../../../../f-r-gravity.md) variation: the connection is always the Levi-Civita connection of the varied [metric tensor](../../../../../../../metric-tensor.md), not an independent variable.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 49](../../../../paper-49-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
