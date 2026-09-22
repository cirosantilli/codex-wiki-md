<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $Q$ be the configuration [smooth manifold](../../../../../../smooth-manifold.md), and let $L(t,q,v)$ be a [smooth](../../../../../../smooth-function.md) [Lagrangian](../../../../../../lagrangian.md) on its [tangent bundle](../../../../../../tangent-bundle.md). For a path with fixed endpoints, its [action](../../../../../../action.md) is

$$
S[q]=\int_a^b L(t,q(t),\dot q(t))\,dt.
$$

The [principle of stationary action](../../../../../../principle-of-stationary-action.md) requires the [first variation](../../../../../../first-variation.md) to vanish for every fixed-endpoint [variation](../../../../../../variation.md). In a coordinate chart take $q_s=q+s\eta$, with $\eta(a)=\eta(b)=0$. Differentiation under the integral and [integration by parts](../../../../../../integration-by-parts.md) give

$$
\left.\frac d{ds}S[q_s]\right|_{s=0}
=\int_a^b\left(\frac{\partial L}{\partial q^i}\eta^i+\frac{\partial L}{\partial v^i}\dot\eta^i\right)dt
=\int_a^b\left(\frac{\partial L}{\partial q^i}-\frac d{dt}\frac{\partial L}{\partial v^i}\right)\eta^i\,dt.
$$

Repeated coordinate indices are summed. The endpoint term vanishes. Since compactly supported [variations](../../../../../../variation.md) can be chosen independently in each coordinate, the [fundamental lemma of the calculus of variations](../../../../../../fundamental-lemma-of-the-calculus-of-variations.md) yields the [Euler-Lagrange equations](../../../../../../euler-lagrange-equation.md)

$$
\boxed{\frac d{dt}\frac{\partial L}{\partial\dot q^i}=\frac{\partial L}{\partial q^i}.}
$$

Conversely these equations make the displayed [first variation](../../../../../../first-variation.md) zero for every fixed-endpoint [variation](../../../../../../variation.md). Variations localized in coordinate charts establish the same assertion for paths on $Q$. Thus **the [Euler-Lagrange equations](../../../../../../euler-lagrange-equation.md) are exactly the stationary-path condition**, not necessarily a condition for an [action](../../../../../../action.md) minimum.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
