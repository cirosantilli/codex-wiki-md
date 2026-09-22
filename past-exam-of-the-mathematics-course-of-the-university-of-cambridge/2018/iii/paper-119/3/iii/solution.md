<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the [category of commutative monoids](../../../../../../category-of-commutative-monoids.md), which is a [semi-additive category](../../../../../../semi-additive-category.md): hom-sets have pointwise addition, composition is additive in each variable, and finite cartesian products are also coproducts. Explicitly, maps $M_i\to N$ extend from the coordinate injections by $(m_i)\mapsto\sum_i f_i(m_i)$.

Take the submonoid

$$
A=\{(m,n)\in\mathbb N^2:m\leq n\leq2m\},\qquad B=\mathbb N,
$$

with coordinatewise addition, and the two projections $f(m,n)=m$, $g(m,n)=n$. The homomorphism $r(m)=(m,m)$ satisfies $fr=gr=1_B$, so this is a [reflexive pair](../../../../../../reflexive-pair.md). For $C=\mathbb N$, evaluation at $1$ identifies $\mathcal C(C,B)$ with $B$ and $\mathcal C(C,A)$ with $A$.

The element $(1,2)$ gives an arrow from $1$ to $2$ in the prescribed graph. An inverse would require an element $(2,1)$ of $A$, which does not exist. Therefore no [groupoid](../../../../../../groupoid.md) structure with these source and target maps is possible, regardless of the proposed composition rule:

$$
\boxed{\text{Semi-additivity does not suffice for the groupoid conclusion.}}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 119](../../../paper-119-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
