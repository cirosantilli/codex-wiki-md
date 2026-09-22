# Agreement of two path integrals does not imply conservativeness

↑ **Parent:** [Path independence](path-independence.md)

Equality of [line integrals](line-integral.md) on two selected paths is a necessary test for a [conservative vector field](conservative-vector-field.md), but it is not sufficient. The paths may both miss the component responsible for nonzero [curl](curl.md).

For an explicit example, take $W(x,y,z)=(z-y,x-z,y-x)^T$. Its [curl](curl.md) is the nonzero constant $2(1,1,1)^T$, so it is not a [gradient field](gradient-field.md) on $\mathbb R^3$. Nevertheless, on the [plane](plane.md) $x=y$, the field equals $(z-x,x-z,0)^T$. Every [tangent vector](tangent-vector-split.md) to that [plane](plane.md) has equal first and second components, giving zero [dot product](dot-product.md) with $W$. Thus every [line integral](line-integral.md) of $W$ along a path confined to that [plane](plane.md) is zero, regardless of endpoints or the path's shape.

In particular, a broken straight path and a genuinely curved path in that [plane](plane.md) can have matching [line integrals](line-integral.md) while revealing nothing about global [path independence](path-independence.md). To establish a [conservative vector field](conservative-vector-field.md), construct a [vector-field potential](potential-of-a-conservative-vector-field.md), or verify the appropriate global criterion such as zero [curl](curl.md) on a simply connected domain.

## ↑ Ancestors (10)

1. [Path independence](path-independence.md)
2. [Fundamental theorem for line integrals](fundamental-theorem-for-line-integrals.md)
3. [Vector calculus](vector-calculus.md)
4. [Multivariable calculus](multivariable-calculus-split.md)
5. [Calculus](calculus-split.md)
6. [Real analysis](real-analysis-split.md)
7. [Analysis](analysis-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)
