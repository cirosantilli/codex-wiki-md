<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

An [omega-saturated model](../../../../../omega-saturated-model.md) realizes every complete one-type over every finite subset of its domain that is consistent with the [first-order structure](../../../../../first-order-structure.md)'s [first-order theory](../../../../../first-order-theory.md) with those named parameters. Equivalently, every [partial type](../../../../../partial-type.md) in a finite tuple over finitely many parameters that is finitely satisfiable in the [first-order structure](../../../../../first-order-structure.md) has a realization there. The equivalence follows by extending a [partial type](../../../../../partial-type.md) to a [complete type](../../../../../complete-type.md); finite tuples can be handled one coordinate at a time.

For an example, take a countably infinite set in the language of equality alone. Over finitely many named elements, a complete one-type either requires equality with one of them or inequality with all of them. Both possibilities are realized. [quantifier elimination](../../../../../quantifier-elimination.md) for an infinite pure set follows by choosing a quantified variable either equal to one of the finitely many named values or distinct from all of them. Indeed every permutation fixing the parameters is a [structure automorphism](../../../../../automorphism-of-a-first-order-structure.md), and all other elements have the same type, so there are no further one-types. This [first-order structure](../../../../../first-order-structure.md) is **omega-saturated**.

For a counterexample, take $(\mathbb N;0,S)$, where $S(n)=n+1$. The parameter-free [partial type](../../../../../partial-type.md)

$$
\boxed{p(x)=\{x\ne S^n(0):n=0,1,2,\ldots\}}
$$

is finitely satisfiable: choose an integer beyond the finitely many excluded numerals. It is not realized in the [first-order structure](../../../../../first-order-structure.md), because every natural number is one of those numerals. Any complete extension of this [partial type](../../../../../partial-type.md) is therefore omitted as well. Thus the standard successor [first-order structure](../../../../../first-order-structure.md) is **not omega-saturated**.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the model theory course of the University of Oxford](../../../../split.md)
6. [Model theory course of the University of Oxford](../../../../../model-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
