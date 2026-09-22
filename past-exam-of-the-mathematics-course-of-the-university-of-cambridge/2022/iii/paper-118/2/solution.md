<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [holomorphic line bundle](../../../../../holomorphic-line-bundle.md) is a complex line bundle with holomorphic transition functions, and a [holomorphic section](../../../../../holomorphic-section.md) is one whose coefficient in every holomorphic local frame is holomorphic. Given a [Hermitian metric on a holomorphic vector bundle](../../../../../hermitian-metric-on-a-holomorphic-vector-bundle.md) $h$, its [Chern connection](../../../../../chern-connection.md) is the connection $\nabla$ satisfying

$$
\nabla^{0,1}=\bar\partial_L,
\qquad
d\,h(s,t)=h(\nabla s,t)+h(s,\nabla t).
$$

Let $e$ be a nonvanishing [holomorphic local frame](../../../../../holomorphic-local-trivialization.md), put $H=h(e,e)>0$, and write $\nabla e=Ae$. The first condition forces $A^{0,1}=0$, while metric compatibility forces

$$
A=H^{-1}\partial H=\partial\log H.
$$

This determines $\nabla$ uniquely and also constructs it. If $e'=ge$ for a nowhere-zero holomorphic function $g$, then $A'=A+g^{-1}\partial g$, exactly the [connection one-form](../../../../../connection-one-form.md) transformation law, so the local constructions glue.

For a line bundle, $A\wedge A=0$, and the [curvature form of a connection](../../../../../curvature-form.md) is

$$
F(\nabla)=dA=\bar\partial\partial\log H=-\partial\bar\partial\log H.
$$

It has type $(1,1)$. Under $e'=ge$, the extra term $g^{-1}\partial g$ is closed, so the curvature is unchanged and therefore global. This is the [local formula for the Chern connection on a line bundle](../../../../../local-formula-for-the-chern-connection-on-a-line-bundle.md).

Any other Hermitian metric has the form $\widehat h=e^u h$ for a global smooth real function $u$. Its local squared norm is $\widehat H=e^uH$, whence

$$
F(\widehat\nabla)-F(\nabla)=\bar\partial\partial u.
$$

Connections $\nabla_1$ and $\nabla_2$ induce the [tensor product connection](../../../../../tensor-product-connection.md)

$$
(\nabla_1\otimes\nabla_2)(s_1\otimes s_2)
=\nabla_1s_1\otimes s_2+s_1\otimes\nabla_2s_2.
$$

Its connection form in a product frame is $A_1+A_2$, so the [curvature of a tensor product connection](../../../../../curvature-of-a-tensor-product-connection.md) is $F_1+F_2$. For Chern connections, equip $L_1\otimes L_2$ with the product metric

$$
h(s_1\otimes s_2,t_1\otimes t_2)=h_1(s_1,t_1)h_2(s_2,t_2).
$$

The tensor product connection has the correct $(0,1)$ part and preserves this metric, so uniqueness identifies it with the Chern connection of $h$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 118](../../paper-118-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
