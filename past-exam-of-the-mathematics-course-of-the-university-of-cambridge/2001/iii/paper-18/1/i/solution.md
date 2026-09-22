<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the reverse absorption order on the [incline](../../../../../../incline.md):

$$
\boxed{a\preceq b\quad\Longleftrightarrow\quad a+b=a.}
$$

This is exactly the relation given by the pairs $(x+y,x)$. Indeed, if $a=x+y$ and $b=x$, then $a+b=x+y+x=a$ by additive [idempotence](../../../../../../idempotence.md), [associativity](../../../../../../associative-property.md) and [commutativity](../../../../../../commutativity.md). Conversely $a+b=a$ expresses $a$ as $b+a$, so $(a,b)$ is one of these pairs.

Additive [idempotence](../../../../../../idempotence.md) gives $a+a=a$, hence reflexivity. If $a+b=a$ and $b+c=b$, then

$$
a+c=(a+b)+c=a+(b+c)=a+b=a,
$$

so the relation is transitive. In fact it is antisymmetric as well: $a+b=a$ and $b+a=b$, together with [commutativity](../../../../../../commutativity.md), imply $a=b$. Thus **the relation is a partial order, and therefore a quasi-order**. It is the reverse of the usual join order of an [incline](../../../../../../incline.md); keeping this reversal is essential for the [well-quasi-ordering](../../../../../../well-quasi-ordering.md) conclusion.

Both operations are [order-preserving](../../../../../../order-preserving-function.md) for this order. If $a\preceq b$, then $(a+c)+(b+c)=a+c$ by additive [idempotence](../../../../../../idempotence.md), while [distributivity](../../../../../../distributive-property.md) gives $ac+bc=(a+b)c=ac$. The multiplicative absorption identity also says

$$
a\preceq ab.
$$

Thus multiplying a [monomial](../../../../../../monomial.md) by another factor moves upward in the reverse absorption order.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
