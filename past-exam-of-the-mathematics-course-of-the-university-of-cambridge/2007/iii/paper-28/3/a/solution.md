<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Any extending absolute value is also non-Archimedean. Indeed its values on integers are the given base-field values, bounded by one, so the [integer criterion for a non-Archimedean absolute value](../../../../../../integer-criterion-for-a-non-archimedean-absolute-value.md) applies. For the criterion's sufficiency, the binomial theorem gives $|x+y|^n\le(n+1)\max(|x|,|y|)^n$; taking $n$th roots yields the ultrametric inequality.

Fix a $K$-basis of $L$ and its coordinate maximum norm. Every extending absolute value is a vector-space norm satisfying $\|av\|=|a|\|v\|$. The [finite-dimensional non-Archimedean norm equivalence over a complete field](../../../../../../finite-dimensional-non-archimedean-norm-equivalence-over-a-complete-field.md) makes it equivalent to that coordinate norm. Here is the relevant proof: induct on dimension. The span $W$ of all but the last basis vector $e$ is complete by the induction hypothesis, hence closed in the given norm. Therefore $\delta=\inf_{w\in W}\|e-w\|>0$. For $v=w+ae$, one has $|a|\le\|v\|/\delta$ and $\|w\|\le\max(\|v\|,|a|\|e\|)$. The induction bound on $W$ bounds all its coordinates by a constant times $\|v\|$. The reverse bound follows from the triangle inequality. This proof applies to every complete base field here, without a local compactness assumption.

Thus two extending absolute values satisfy $c|x|_1\le|x|_2\le C|x|_1$ for fixed positive constants. Apply this to $x^n$ and take $n$th roots:

$$
c^{1/n}|x|_1\le|x|_2\le C^{1/n}|x|_1.
$$

Letting $n\to\infty$ proves equality. The [bounded comparison forces equality of multiplicative absolute values](../../../../../../bounded-comparison-forces-equality-of-multiplicative-absolute-values.md) argument gives the required [unique extension of an absolute value to a finite extension](../../../../../../unique-extension-of-an-absolute-value-to-a-finite-extension.md), without proving existence.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
