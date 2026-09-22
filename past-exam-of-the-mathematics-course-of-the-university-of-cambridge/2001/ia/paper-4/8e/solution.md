<h1 id="8e/solution">Solution</h1>

↑ **Parent:** [8E](../8e.md)

[Mathematical induction](../../../../../mathematical-induction.md) consists of an [induction base case](../../../../../induction-base-case.md) $P(1)$ and an [inductive step](../../../../../inductive-step.md) $P(n)\Rightarrow P(n+1)$ for every [positive integer](../../../../../positive-integer.md) $n$. To derive it from the [well-ordering principle](../../../../../well-ordering-principle-for-the-natural-numbers.md), suppose the [set](../../../../../set-split.md) of counterexamples were nonempty and take its least element $n$. The base case excludes $n=1$. If $n>1$, minimality gives $P(n-1)$, and the step then gives $P(n)$, a [contradiction](../../../../../contradiction.md). Hence there are no counterexamples.

For the stated [integer congruence](../../../../../integer-congruence.md), the base case is $9\equiv2\pmod7$. If $9^n\equiv2^n\pmod7$, multiplication and $9\equiv2\pmod7$ give

$$
9^{n+1}\equiv9\cdot2^n\equiv2^{n+1}\pmod7,
$$

completing the induction.

The purported shifted-sum proof has a correct conditional successor calculation, but **the base case is missing and false**: at $n=1$ it would assert $1=1+126$. An [inductive step](../../../../../inductive-step.md) without a true [induction base case](../../../../../induction-base-case.md) cannot establish any instance.

## ↑ Ancestors (10)

1. [8E](../8e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
