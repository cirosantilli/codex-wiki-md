<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write a local frame as $e_a$, its [dual basis](../../../../../../../dual-basis.md) as $\epsilon^a$, and set $De_a=A^b{}_a e_b$. The one-form definition gives $D\epsilon^a=-A^a{}_b\epsilon^b$. Repeated indices are summed. Every [tensor field](../../../../../../../tensor-field.md) has a unique local expansion

$$
T=T_{a_1\ldots a_k}^{b_1\ldots b_l}\,\epsilon^{a_1}\otimes\cdots\otimes\epsilon^{a_k}\otimes e_{b_1}\otimes\cdots\otimes e_{b_l}.
$$

Define $DT$ by applying the scalar operator to its coefficient and applying $D$ to one frame factor at a time, adding all these terms. In components this is

$$
\boxed{(DT)_{a_1\ldots a_k}^{b_1\ldots b_l}
=Z\!\left(T_{a_1\ldots a_k}^{b_1\ldots b_l}\right)
-\sum_{r=1}^k A^c{}_{a_r}T_{a_1\ldots c\ldots a_k}^{b_1\ldots b_l}
+\sum_{s=1}^l A^{b_s}{}_cT_{a_1\ldots a_k}^{b_1\ldots c\ldots b_l}.}
$$

In each term only the indicated slot is replaced. This formula is real-linear and satisfies the [Leibniz rule](../../../../../../../leibniz-rule.md) for a [tensor product](../../../../../../../tensor-product.md): differentiating a coefficient product uses the scalar product rule, and the list of differentiated frame factors splits into the two factors' lists.

To check that it is intrinsic, write $e$ as the row of frame fields and $\epsilon$ as the column of dual fields. Change frame by $e'=eP$, where $P$ is an invertible smooth [matrix](../../../../../../../matrix.md). Then

$$
A'=P^{-1}(AP+ZP),\qquad \epsilon'=P^{-1}\epsilon.
$$

Differentiating the inverse [matrix](../../../../../../../matrix.md) gives $Z(P^{-1})=-P^{-1}(ZP)P^{-1}$; it cancels the extra frame-change terms in the dual factors. The same cancellation in each tensor slot makes the two local formulas agree. Thus they glue to a global [tensor derivation](../../../../../../../tensor-derivation.md).

In particular, for arbitrary tensor types, not necessarily the same type,

$$
\boxed{D(S\otimes T)=DS\otimes T+S\otimes DT.}
$$

The resulting type is the sum of their two covariant counts and their two contravariant counts. This also supplies the required real-linearity for every type, including functions as type $(0,0)$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
