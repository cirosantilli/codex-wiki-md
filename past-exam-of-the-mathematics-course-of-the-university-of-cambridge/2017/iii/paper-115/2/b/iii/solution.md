<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For a decomposable [tensor field](../../../../../../../tensor-field.md), consider a selected pairing $\omega(Y)$ in a [tensor contraction](../../../../../../../tensor-contraction.md). Its derivative is

$$
D(\omega(Y))=(D\omega)(Y)+\omega(DY)
$$

by the defining one-form formula. In the [Leibniz rule](../../../../../../../leibniz-rule.md) expansion of the uncontracted tensor, the terms differentiating these two selected factors combine into exactly this derivative of the pairing. Every term differentiating another factor passes unchanged through the contraction. Thus, first on local decomposable tensors and then by linearity on every local tensor expansion,

$$
\boxed{DC_j^i=C_j^iD.}
$$

This is basis independent; in components the negative covector term and positive vector term for the two contracted slots cancel.

For uniqueness, any extension satisfying the tensor-product rule is local. If $T$ vanishes near $p$, multiply it by a [smooth cutoff function](../../../../../../../smooth-cutoff-function.md) $h$ equal to one near $p$ and supported where $T=0$. The identity $D(hT)=(Dh)T+hDT$ implies $DT(p)=0$. Any allowed extension on a [differential one-form](../../../../../../../one-form.md) is forced by differentiating its contraction with every [vector field](../../../../../../../vector-field.md). Its value on every local frame tensor is then forced by the tensor-product rule and its value on scalar coefficients. These local tensors span each tensor bundle, so two extensions agree everywhere.

Together with the preceding construction, this proves **existence and uniqueness of the contraction-compatible [tensor derivation](../../../../../../../tensor-derivation.md)**, with the scalar-rule qualification already stated. No claim that every global [tensor field](../../../../../../../tensor-field.md) is a finite sum of products of global [vector fields](../../../../../../../vector-field.md) is needed.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 115](../../../../paper-115-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
