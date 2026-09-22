<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Apply the [splitting principle for complex vector bundles](../../../../../splitting-principle-for-complex-vector-bundles.md) simultaneously to $E$ and $F$. This can be implemented by successive projective bundle pullbacks; the projective bundle theorem makes their composite pullback injective on integral [cohomology](../../../../../cohomology-split.md). After pullback write $E=L_1\oplus L_2$ and $F=M_1\oplus M_2$, with [Chern roots](../../../../../chern-root.md) $x_1,x_2$ and $y_1,y_2$. Let

$$
A=x_1+x_2=c_1(E),\quad C=x_1x_2=c_2(E),\qquad
B=y_1+y_2=c_1(F),\quad D=y_1y_2=c_2(F).
$$

Since the [First Chern class](../../../../../first-chern-class.md) of a tensor product of [complex line bundles](../../../../../complex-line-bundle.md) is the sum of their first [Chern classes](../../../../../chern-class.md), the four roots of $E\otimes F$ are $x_i+y_j$, $1\leq i,j\leq2$.

Compute their six pairwise products integrally. The two pairs within a fixed $x_i$ row contribute

$$
\sum_{i=1}^2(x_i+y_1)(x_i+y_2)=x_1^2+x_2^2+AB+2D=A^2-2C+AB+2D.
$$

The four pairs between the two rows contribute

$$
\sum_{j,k=1}^2(x_1+y_j)(x_2+y_k)=4C+2AB+B^2.
$$

Their sum is the second elementary symmetric [polynomial](../../../../../polynomial-split.md) of the tensor roots. Injectivity of the pullback returns the resulting identity to $X$, giving

$$
\boxed{c_2(E\otimes F)=c_1(E)^2+3c_1(E)c_1(F)+c_1(F)^2+2c_2(E)+2c_2(F).}
$$

Products here are [cup products](../../../../../cup-product.md) in integral [cohomology](../../../../../cohomology-split.md). This [second Chern class of a tensor product of rank-two bundles](../../../../../second-chern-class-of-a-tensor-product-of-rank-two-bundles.md) formula uses no division by two and therefore holds without assuming the integral [cohomology](../../../../../cohomology-split.md) of $X$ is torsion-free.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
