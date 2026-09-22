<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Suppose that $f$ is not [surjective](../../../../../../surjective-function.md), and choose $y\notin f(Y)$. If $y$ lies in the open two-cell, then $Y\setminus\{y\}$ deformation retracts onto the target circle of the degree-$n$ attaching map, so its first [integral homology](../../../../../../integral-homology.md) is $\mathbb Z$. If $y\in Z$, the punctured space deformation retracts onto a finite graph and again has free abelian first homology. The factorization

$$
Y\xrightarrow{f}Y\setminus\{y\}\hookrightarrow Y
$$

therefore makes $f_*:H_1(Y)\to H_1(Y)$ factor through a free abelian group. Every homomorphism from the finite group $H_1(Y)\cong\mathbb Z/n$ to a free abelian group is zero, contradicting the assumed surjectivity of $f_*$.

The converse is false. The radial coordinate descends to a surjection $r:Y\to[0,1]$. The finite CW complex $Y$ is a [Peano continuum](../../../../../../peano-continuum.md), so the [Hahn-Mazurkiewicz theorem](../../../../../../hahn-mazurkiewicz-theorem.md) supplies a continuous surjection $g:[0,1]\to Y$. Then $g\circ r:Y\to Y$ is surjective, but its induced map on $H_1$ is zero because it factors through the contractible interval.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 114](../../../paper-114-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
