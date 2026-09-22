<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write the two [formal pseudodifferential operators](../../../../../../formal-pseudodifferential-operator.md) in normal order as

$$
P_1=a\partial^p+a_1\partial^{p-1}+\cdots,\qquad
P_2=b\partial^q+b_1\partial^{q-1}+\cdots,
$$

where $p=\alpha_1$ and $q=\alpha_2$. The [formal pseudodifferential composition rule](../../../../../../formal-pseudodifferential-composition-rule.md) gives

$$
P_1P_2=ab\partial^{p+q}
+\bigl(pa b'+ab_1+a_1b\bigr)\partial^{p+q-1}+\cdots.
$$

Thus $\boxed{\operatorname{ord}(P_1P_2)=p+q}$ whenever $ab$ is not identically zero, in particular when both leading [coefficients](../../../../../../coefficient.md) are nowhere zero. In general the rigorous statement over the specified [coefficient](../../../../../../coefficient.md) algebra is $\operatorname{ord}(P_1P_2)\leq p+q$.

The leading scalar [coefficients](../../../../../../coefficient.md) commute. Subtracting the reversed composition also cancels the terms involving $a_1,b_1$, leaving

$$
[P_1,P_2]=(pa b'-qb a')\partial^{p+q-1}+\cdots.
$$

Therefore the [order filtration of formal pseudodifferential operators](../../../../../../order-filtration-of-formal-pseudodifferential-operators.md) gives

$$
\boxed{\operatorname{ord}[P_1,P_2]\leq p+q-1,}
$$

with equality precisely when the displayed [coefficient](../../../../../../coefficient.md) is not identically zero. The bound can be strict: constant-coefficient powers of $\partial$ commute, giving the zero operator, whose order can be assigned $-\infty$.

There is also a genuine qualification to product-order addition in $C^\infty(\mathbb R)$. Choose nonzero [smooth functions](../../../../../../smooth-function.md) $a,b$ with disjoint [compact supports](../../../../../../compact-support.md) and take $P_1=m_a,P_2=m_b$. Each has order zero, but their product is zero. Nonzero [coefficients](../../../../../../coefficient.md) as elements of this algebra need not have a nonzero product. Thus an unqualified assertion of exact product order requires an additional leading-symbol hypothesis.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
