<h1 id="6/b/i/solution">Solution</h1>

↑ **Parent:** [i](../i.md)

Fix $x\in G$. The [integer powers of a group element](../../../../../../../integer-power-of-a-group-element.md) satisfy

$$
x^{z+w}=x^zx^w,\qquad (x^w)^z=x^{wz}=x^{zw}\qquad(z,w\in\mathbb Z).
$$

For [nonnegative integers](../../../../../../../natural-number.md) these rules follow by [associativity](../../../../../../../associative-property.md) and counting factors; negative [integers](../../../../../../../integer-split.md) are handled by $x^{-r}=(x^{-1})^r$, and opposite signs by cancellation of adjacent [inverse elements](../../../../../../../inverse-element.md). All factors are powers of the same element, so no [abelian group](../../../../../../../abelian-group.md) assumption is involved.

It follows that $z\mapsto\rho(z,x)=x^z$ is a [group homomorphism](../../../../../../../group-homomorphism.md) from the [additive group of integers](../../../../../../../additive-group-of-integers.md) to $G$, and

$$
\boxed{\rho(z,\rho(w,x))=\rho(zw,x).}
$$

The homomorphism uses ordinary [addition](../../../../../../../addition.md) on $\mathbb Z$; composition of the power [functions](../../../../../../../function-split.md) corresponds to ordinary [multiplication](../../../../../../../multiplication.md) of exponents.

## ↑ Ancestors (13)

1. [i](../i.md)
2. [b](../../b.md)
3. [6](../../../6.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
