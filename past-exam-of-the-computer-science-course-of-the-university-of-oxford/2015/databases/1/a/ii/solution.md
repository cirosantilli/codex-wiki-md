<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Construct the required models and the actual customer–model purchases using [relational projection](../../../../../../relational-projection.md) and a [natural join](../../../../../../natural-join.md):

$$
M=\pi_{\mathsf{model}}C,\qquad I=\pi_{\mathsf{customerid}}U,\qquad V=\pi_{\mathsf{customerid,model}}(S\bowtie C).
$$

The [Cartesian product](../../../../../../cartesian-product.md) $I\times M$ lists every obligation: every customer paired with every model present in `Car`. The [relational difference](../../../../../../relational-difference.md) $(I\times M)-V$ consists of unfulfilled obligations. Remove the customer identifiers occurring in this [database relation](../../../../../../database-relation.md) and only then recover names:

$$
\begin{aligned}
G&=I-\pi_{\mathsf{customerid}}\bigl((I\times M)-V\bigr),\\
&\boxed{\text{answer}=\pi_{\mathsf{name}}(U\bowtie G).}
\end{aligned}
$$

This is an explicit [relational division](../../../../../../relational-division.md) construction with all customers as the candidate universe. If there are no models, there are no missing obligations, so every customer qualifies. A version starting solely from customers occurring in $V$ would incorrectly omit customers with no purchases in that empty-model case.

The quantified object here is the `model` [database attribute](../../../../../../database-attribute.md), so two makes sharing a model value contribute one required value. If a different application identified a model by the pair `(make, model)`, both the required and purchased [relational projections](../../../../../../relational-projection.md) would use that pair. Also, `Car` contains unsold cars: a model available only in unsold inventory is still a required model, and then nobody qualifies. Testing identifiers before names prevents different customers with the same name from pooling their purchases.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Databases](../../../../databases-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
