<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Give $U(\mathfrak g)$ its degree [filtration](../../../../../../filtration-probability-theory.md). The [Poincaré-Birkhoff-Witt theorem](../../../../../../poincare-birkhoff-witt-theorem.md) identifies its [associated graded ring](../../../../../../associated-graded-ring.md) with $\operatorname{Sym}_k\mathfrak g$, a [polynomial ring](../../../../../../polynomial-ring.md) in $\dim_k\mathfrak g$ variables. The [Hilbert basis theorem](../../../../../../hilbert-basis-theorem.md) makes this graded [algebra](../../../../../../algebra-split.md) [Noetherian](../../../../../../noetherian-ring.md) on both sides.

Here is the required transfer, including why a finite list of symbols gives actual generators. For a [right ideal](../../../../../../right-ideal.md) $I$ of a nonnegatively filtered [ring](../../../../../../ring.md) $A$, its induced graded [ideal](../../../../../../ideal.md) $\operatorname{gr}I$ is a homogeneous [right ideal](../../../../../../right-ideal.md) of $\operatorname{gr}A$. Choose finite homogeneous generators and lift them to $u_1,\ldots,u_m\in I$. For $u\in I$ of degree $d$, express its leading symbol as a graded right linear combination of these symbols, using homogeneous coefficients of complementary degrees. Lift the coefficients to $A$ and subtract the corresponding $\sum_i u_ia_i$. The remainder has degree strictly below $d$. Induction, terminating because degrees are nonnegative, proves $I=\sum_i u_iA$. The identical argument with coefficients on the left treats [left ideals](../../../../../../left-ideal.md).

This [ascending filtered-graded transfer of Noetherianity](../../../../../../ascending-filtered-graded-transfer-of-noetherianity.md) proves that $U(\mathfrak g)$ is right and left [Noetherian](../../../../../../noetherian-ring.md). A [quotient ring](../../../../../../quotient-ring.md) inherits either property: pull an ascending ideal chain back to the original [ring](../../../../../../ring.md), or take images of ideal generators. Part (a) therefore gives **$R$ right and left Noetherian**. Alternatively, under the broader [almost commutative algebra](../../../../../../almost-commutative-algebra.md) convention, its commutative finitely generated [associated graded ring](../../../../../../associated-graded-ring.md) is directly a quotient of a finite-variable [polynomial ring](../../../../../../polynomial-ring.md), and the same leading-symbol argument proves the conclusion.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 85](../../../paper-85-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
