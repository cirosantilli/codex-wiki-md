<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Prove the stronger equation, quantified over the accumulator:

$$
f(\operatorname{foldl}\ g\ a\ xs)=\operatorname{foldl}\ h\ (f\ a)\ xs\qquad\text{for all }a,xs.
$$

For `[]`, both sides are `f a`. For the [bottom value](../../../../../bottom-value.md), both sides are bottom because `f` is a [strict function](../../../../../strict-function.md). For the cons step, the universal [induction hypothesis](../../../../../induction-hypothesis.md) allows the accumulator to become `g a x`:
```
f (foldl g a (x:xs))
 = f (foldl g (g a x) xs)
 = foldl h (f (g a x)) xs
 = foldl h (h (f a) x) xs
 = foldl h (f a) (x:xs).
```
Thus [structural induction](../../../../../structural-induction.md) proves the claim for finite and finite partial spines; definable continuity extends it to infinite [lazy lists](../../../../../lazy-list.md). Pointwise equality is exactly the asserted equality of [function compositions](../../../../../function-composition.md). This is the [left-fold fusion law](../../../../../left-fold-fusion-law.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
