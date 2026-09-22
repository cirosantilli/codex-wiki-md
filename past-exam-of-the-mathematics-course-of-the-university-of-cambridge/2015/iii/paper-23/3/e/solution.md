<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

A [formally real field](../../../../../../formally-real-field.md) is a [field](../../../../../../field.md) in which $-1$ is not a finite sum of squares. The [theory of formally real fields](../../../../../../theory-of-formally-real-fields.md) consists of the field axioms and, for each $m\geq1$, the sentence

$$
\forall x_1\cdots\forall x_m\ \bigl(1+x_1^2+\cdots+x_m^2\ne0\bigr).
$$

A [real closed field](../../../../../../real-closed-field.md) is a [formally real field](../../../../../../formally-real-field.md) with no proper formally real algebraic extension. An equivalent first-order axiomatization of the [Theory of real closed fields](../../../../../../theory-of-real-closed-fields.md) adds: every $a$ or its negative is a square, and every odd-degree polynomial has a root. Explicitly the square axiom is

$$
\forall a\,\exists b\,(a=b^2\vee -a=b^2),
$$

and the polynomial axioms say that every monic polynomial of degree $2d+1$ has a root, for each $d\geq0$.

The [Artin-Schreier ordering criterion](../../../../../../artin-schreier-ordering-criterion.md) says that every [formally real field](../../../../../../formally-real-field.md) can be ordered, and the [real closure theorem](../../../../../../real-closure-theorem.md) embeds each ordered field into an algebraic [real closed field](../../../../../../real-closed-field.md) extension. Consequently every [FRF](../../../../../../theory-of-formally-real-fields.md) model embeds into an [RCF](../../../../../../theory-of-real-closed-fields.md) model. Conversely every [RCF](../../../../../../theory-of-real-closed-fields.md) model is itself an [FRF](../../../../../../theory-of-formally-real-fields.md) model, so the reverse embedding requirement is automatic.

It remains to establish [model completeness](../../../../../../model-complete-theory.md). A [real closed field](../../../../../../real-closed-field.md) has a unique order, definable in the field language by

$$
a>0\quad\Longleftrightarrow\quad a\ne0\text{ and }\exists b\,(b^2=a).
$$

Any [field embedding](../../../../../../field-embedding.md) between [real closed fields](../../../../../../real-closed-field.md) preserves this order: positive elements are nonzero squares, and negative elements have positive negatives. The [quantifier elimination for ordered real closed fields](../../../../../../quantifier-elimination-for-ordered-real-closed-fields.md) theorem makes every such ordered embedding elementary, by the preceding part. Restricting to formulas of the field language makes the original embedding elementary as well. Thus [RCF](../../../../../../theory-of-real-closed-fields.md) is [model-complete](../../../../../../model-complete-theory.md) in the field language.

The embedding conditions and [model completeness](../../../../../../model-complete-theory.md) prove

$$
\boxed{\mathrm{RCF}\text{ is the model companion of }\mathrm{FRF}.}
$$

The [quantifier elimination](../../../../../../quantifier-elimination.md) invoked here is in the ordered language. In the unordered field language, [model completeness](../../../../../../model-complete-theory.md) still holds, but full [quantifier elimination](../../../../../../quantifier-elimination.md) does not follow from forgetting the order.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
