<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Expand the three [matrix exponentials](../../../../../../matrix-exponential.md) and retain terms through degree two. Their product is

$$
E(t)=I+t(A+B)+\frac{t^2}{2}(A^2+AB+BA+B^2)+O(t^3),
$$

which agrees with $e^{t(A+B)}$ to that order. Keeping the cubic terms gives the more informative defect

$$
E(t)-e^{t(A+B)}=t^3\left(-\frac1{24}[A,[A,B]]+\frac1{12}[B,[B,A]]\right)+O(t^4),
$$

where $[A,B]=AB-BA$ is the [commutator](../../../../../../commutator.md). For example, the coefficients of $A^2B,ABA,BA^2$ in the product are $1/8,1/4,1/8$, instead of the exact $1/6,1/6,1/6$. The cubic defect is generically nonzero. Therefore **[Strang splitting](../../../../../../strang-splitting.md) has order $p=2$**. The symmetry $E(-t)=E(t)^{-1}$ is consistent with this cancellation of the quadratic defect; for commuting $A,B$ the composition is exact rather than merely second order.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
