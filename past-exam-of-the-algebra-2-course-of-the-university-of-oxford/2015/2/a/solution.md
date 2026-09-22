<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [Euclidean domain](../../../../euclidean-domain.md) is a [principal ideal domain](../../../../principal-ideal-domain.md). The [structure theorem for finitely generated modules over a principal ideal domain](../../../../structure-theorem-for-finitely-generated-modules-over-a-principal-ideal-domain.md) therefore gives, for every [finitely generated module](../../../../finitely-generated-module.md) $M$ over $R$,

$$
M\cong R^r\oplus R/(d_1)\oplus\cdots\oplus R/(d_s),
$$

where the $d_i$ are nonzero nonunits and $d_1\mid d_2\mid\cdots\mid d_s$. The factors $d_i$ are unique up to multiplication by [units](../../../../unit-in-a-ring.md); $r$ is uniquely determined.

The [rank of a module](../../../../rank-of-a-module-over-an-integral-domain.md) is this integer $r$. Equivalently, with $K$ the [field of fractions](../../../../field-of-fractions.md) of $R$,

$$
\boxed{\operatorname{rank}_R M=\dim_K(K\otimes_R M)=r.}
$$

The [tensor product of modules](../../../../tensor-product-of-modules.md) kills each displayed torsion summand after extending scalars to $K$, while sending $R^r$ to $K^r$, explaining the equality.

If $M$ is a [torsion-free module](../../../../torsion-free-module.md), no summand $R/(d_i)$ can occur: its nonzero element $1+(d_i)$ is killed by the nonzero scalar $d_i$. Hence $s=0$ and

$$
\boxed{M\cong R^r,\quad\text{so $M$ is a free module}.}
$$

This also covers $M=0$, with $r=0$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the algebra 2 course of the University of Oxford](../../../split.md)
5. [Algebra 2 course of the University of Oxford](../../../../algebra-2-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
