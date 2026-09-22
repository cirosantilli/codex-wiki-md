<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For a [convex cone](../../../../../../convex-cone.md) $D$ in an [inner product](../../../../../../inner-product.md) space, use the nonnegative-pairing convention

$$
D^*=\{B:\langle A,B\rangle\geq0\text{ for every }A\in D\}.
$$

Here the pairing is the [Frobenius inner product](../../../../../../frobenius-inner-product.md) on real [symmetric matrices](../../../../../../symmetric-matrix.md). Let $C_0$ be the [conic hull](../../../../../../conic-hull.md) of the nonnegative [rank-one matrices](../../../../../../rank-one-matrix.md) $xx^T$, and let $C=\overline{C_0}$. For $A\in K$, $\langle A,xx^T\rangle_F=x^TAx\geq0$. This extends to [conic combinations](../../../../../../conic-combination.md), and by [continuity](../../../../../../continuous-function.md) to their limits. Hence $C\subseteq K^*$.

For the converse, if $B\notin C$, [separation from a closed convex cone](../../../../../../separation-from-a-closed-convex-cone.md) supplies a symmetric $H$ with

$$
\langle H,B\rangle_F<0,\qquad
\langle H,Z\rangle_F\geq0\quad(Z\in C).
$$

In particular $x^THx\geq0$ for every $x\geq0$, so $H\in K$. The negative pairing then excludes $B$ from $K^*$. Therefore

$$
\boxed{K^*=\overline{\operatorname{cone}\{xx^T:x\geq0\}}}.
$$

The same generator test gives $C^*=K$. This is the [duality of copositive and completely positive cones](../../../../../../duality-of-copositive-and-completely-positive-cones.md); the next argument removes the closure.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
