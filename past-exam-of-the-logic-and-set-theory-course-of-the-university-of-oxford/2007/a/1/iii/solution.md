<h1 id="a/1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Assume first that $\phi$ is false on the all-true and all-false [Boolean valuations](../../../../../boolean-valuation.md). Use the truth-table normal form from part (ii). Every satisfying [Boolean valuation](../../../../../boolean-valuation.md) on the finitely many [propositional variables](../../../../../propositional-variable.md) must have at least one true [propositional variable](../../../../../propositional-variable.md) and at least one false [propositional variable](../../../../../propositional-variable.md). Its [minterm](../../../../../minterm.md) therefore has the form

$$
C_s\wedge\neg D_s,
$$

where $C_s$ conjoins its true [propositional variables](../../../../../propositional-variable.md) and $D_s$ disjoins its false [propositional variables](../../../../../propositional-variable.md); both lists are nonempty. This is equivalent to $\neg(C_s\to D_s)$. If the satisfying [Boolean valuations](../../../../../boolean-valuation.md) are indexed by $1,\ldots,N$, [De Morgan's laws](../../../../../de-morgan-s-laws.md) gives

$$
\boxed{\phi\equiv\bigvee_{i=1}^N\neg(C_i\to D_i)
\equiv\neg\bigwedge_{i=1}^N(C_i\to D_i).}
$$

If there are no satisfying [Boolean valuations](../../../../../boolean-valuation.md), take $N=1$ and $C_1=D_1=p$: the result is $\neg(p\to p)$, again always false.

Conversely, on the all-true [Boolean valuation](../../../../../boolean-valuation.md) every nonempty $D_i$ is true, so every $C_i\to D_i$ is true. On the all-false [Boolean valuation](../../../../../boolean-valuation.md) every nonempty $C_i$ is false, so every [logical implication](../../../../../logical-implication.md) is again true. Negating their [logical conjunction](../../../../../logical-conjunction.md) gives false on both [Boolean valuations](../../../../../boolean-valuation.md). [Logical equivalence](../../../../../logical-equivalence.md) transfers these values to $\phi$. The usual nonempty meaning of [logical conjunction](../../../../../logical-conjunction.md) and [logical disjunction](../../../../../logical-disjunction.md) of [propositional variables](../../../../../propositional-variable.md) is used here; allowing empty $C_i$ or $D_i$ without qualification would destroy this converse.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
