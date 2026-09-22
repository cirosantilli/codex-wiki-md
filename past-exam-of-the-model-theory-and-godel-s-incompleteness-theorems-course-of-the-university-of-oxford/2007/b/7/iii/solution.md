<h1 id="b/7/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Every automorphism preserves all [logical formulas](../../../../../logical-formula.md) by [induction](../../../../../mathematical-induction.md) on their construction, so an automorphism taking $\vec a$ to $\vec b$ necessarily gives equal [partial types](../../../../../partial-type.md).

For the converse, first note that a finite [first-order structure](../../../../../first-order-structure.md) is atomic by (ii). Thus in both cases every realized finite-tuple [partial type](../../../../../partial-type.md) has an isolating [logical formula](../../../../../logical-formula.md). Suppose two finite [tuples](../../../../../finite-tuple.md) $\vec u,\vec v$ have the same [complete type](../../../../../complete-type.md), and choose a new element $x$ to extend the first [tuple](../../../../../finite-tuple.md). Let $\theta(\vec z,w)$ isolate the realized [partial type](../../../../../partial-type.md) of $(\vec u,x)$. Since

$$
\mathcal A\models\exists w\,\theta(\vec u,w),
$$

[logical equality](../../../../../logical-equality.md) of [partial types](../../../../../partial-type.md) gives $\mathcal A\models\exists w\,\theta(\vec v,w)$. Choose a witness $y$. Isolation ensures $(\vec u,x)$ and $(\vec v,y)$ have the same [complete type](../../../../../complete-type.md). In particular, if $x$ is distinct from the entries already used, their inequality [logical formulas](../../../../../logical-formula.md) ensure $y$ is distinct from its corresponding entries. The resulting finite map is [injective](../../../../../injective-function.md) and partial elementary.

Start from $\vec a\mapsto\vec b$, which is well-defined even for repeated coordinates because their [logical equality](../../../../../logical-equality.md) patterns agree. Enumerate the carrier and extend alternately to include the next missing element in the domain and the next missing element in the range. For a range step apply the same extension argument to the inverse finite map. The [union](../../../../../set-union.md) is an elementary [bijection](../../../../../bijection.md) from $A$ onto itself: every finite [tuple](../../../../../finite-tuple.md) and every [logical formula](../../../../../logical-formula.md) involving it is handled at some stage. It is therefore an automorphism taking $\vec a$ to $\vec b$. In the finite case the construction terminates once all elements have been included.

Hence

$$
\boxed{\operatorname{tp}(\vec a)=\operatorname{tp}(\vec b)
\iff\exists\pi\in\operatorname{Aut}(\mathcal A),\ \pi(\vec a)=\vec b.}
$$

Countability makes the back-and-forth [numeralwise enumeration in arithmetic](../../../../../numeralwise-enumeration-in-arithmetic.md) exhaust the entire [first-order structure](../../../../../first-order-structure.md); it cannot simply be dropped.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../split.md)
6. [Model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
