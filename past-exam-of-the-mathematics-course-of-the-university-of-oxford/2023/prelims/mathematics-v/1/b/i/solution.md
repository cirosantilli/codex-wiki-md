<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For an oriented piecewise smooth [parametric curve](../../../../../../../parametric-curve.md) $\mathbf r:[a,b]\to\mathbb R^3$ and a continuous [vector field](../../../../../../../vector-field.md) $\mathbf F$ along it, the vector-field [line integral](../../../../../../../line-integral.md) is

$$
\boxed{\int_C\mathbf F\cdot d\mathbf r=\int_a^b\mathbf F(\mathbf r(t))\cdot\mathbf r'(t)\,dt.}
$$

For a piecewise smooth curve, sum these integrals over its smooth pieces. The [dot product](../../../../../../../dot-product.md) selects the component of the [vector field](../../../../../../../vector-field.md) in the direction of motion.

If $\mathbf F=\nabla\phi$ for a [smooth function](../../../../../../../smooth-function.md) $\phi$, the [multivariable chain rule](../../../../../../../multivariable-chain-rule.md) gives

$$
\mathbf F(\mathbf r(t))\cdot\mathbf r'(t)=\frac{d}{dt}\phi(\mathbf r(t)).
$$

The [fundamental theorem of calculus](../../../../../../../fundamental-theorem-of-calculus.md), with cancellation at intermediate endpoints, therefore proves the [fundamental theorem for line integrals](../../../../../../../fundamental-theorem-for-line-integrals.md):

$$
\int_C\nabla\phi\cdot d\mathbf r=\phi(\mathbf r(b))-\phi(\mathbf r(a)).
$$

On a closed curve $\mathbf r(a)=\mathbf r(b)$, so $\boxed{\oint_C\nabla\phi\cdot d\mathbf r=0}$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Mathematics V](../../../../mathematics-v-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
