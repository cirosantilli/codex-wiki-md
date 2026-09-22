<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $r:B\to A$ split the [reflexive pair](../../../../../../reflexive-pair.md) $f,g$. Fix $C$, and take objects $u:C\to B$ and arrows $a:C\to A$ with source $fa$ and target $ga$. Since $\mathcal C$ is an [additive category](../../../../../../additive-category.md), its hom-sets are [abelian groups](../../../../../../abelian-group.md), and composition is additive.

The identity at $u$ is $ru$. For $a:u\to v$ and $b:v\to w$, define

$$
b\star a=a-rv+b.
$$

Its source is $fa-v+fb=u-v+v=u$ and its target is $ga-v+gb=v-v+w=w$. The two identity laws follow from $a-rv+rv=a$ and $ru-ru+a=a$. For $c:w\to x$, both parenthesizations of the triple composite are $a-rv+b-rw+c$, so composition is associative.

Define the inverse by

$$
a^{-1}=ru+rv-a.
$$

Its source is $u+v-u=v$ and its target is $u+v-v=u$. Moreover $a^{-1}\star a=ru$ and $a\star a^{-1}=rv$. Thus these data form a [groupoid](../../../../../../groupoid.md), proving the represented form of [reflexive pair in an additive category is an internal groupoid](../../../../../../reflexive-pair-in-an-additive-category-is-an-internal-groupoid.md):

$$
\boxed{b\star a=a-rv+b,\qquad a^{-1}=r(fa)+r(ga)-a.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
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
