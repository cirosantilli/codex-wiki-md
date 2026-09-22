# Cross-product operator with a longitudinal rank-one term

↑ **Parent:** [Inverse of a scalar plus a cross-product operator](inverse-of-a-scalar-plus-a-cross-product-operator.md)

For any real three-dimensional [vectors](vector.md) $a,b$, the displayed [linear equation](linear-equation.md) has the unique solution

$$
x=\frac{a-b\times a}{1+|b|^2}.
$$

Taking a [dot product](dot-product.md) with $b$ first yields $(1+|b|^2)(b\cdot x)=a\cdot b$. Taking a [cross product](cross-product.md) with $b$ and using the [vector triple product identity](vector-triple-product.md) gives

$$
b\times x=b\times a-b(b\cdot x)+|b|^2x.
$$

Substitution into the original equation cancels the longitudinal terms and proves the formula. Conversely direct substitution verifies it for all $b$, including $b=0$, since the denominator is positive. If $C_bx=b\times x$, the underlying identity for [linear maps](linear-map.md) is $(I-C_b)(I+C_b+bb^T)=(1+|b|^2)I$, using $C_b^2=bb^T-|b|^2I$.

## ↑ Ancestors (9)

1. [Inverse of a scalar plus a cross-product operator](inverse-of-a-scalar-plus-a-cross-product-operator.md)
2. [Cross product](cross-product.md)
3. [Vector](vector.md)
4. [Vector space](vector-space-split.md)
5. [Linear algebra](linear-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-1/15/a/solution.md)
