<h1 id="8/e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**Yes: the mutable specification omits important state and frame clauses.** Queries do not explicitly preserve the receiver, so an implementation could clear its state during `present`, return an empty [sequence](../../../../../../sequence.md), and satisfy the displayed coverage condition in the resulting state. Arithmetic does not explicitly preserve a distinct operand, so it could corrupt that operand as well as update the receiver. No initial value or independence requirement for `copy` is stated.

The missing old-state annotation on the other operand is particularly serious under [reference aliasing](../../../../../../reference-aliasing.md). If `other` is the receiver, the printed addition equation becomes $a'=a_0+a'$, which is impossible for a nonzero old count. Self-subtraction becomes $a'=a_0-a'$ rather than the intended zero; self-maximum admits arbitrarily increased counts. Specify instead, for every key,

$$
a'(t)=op(a_0(t),b_0(t)),
$$

with both operands evaluated in their pre-states. Queries preserve all states; updates change only the receiver's abstract value and preserve a distinct operand; `copy` produces an independent snapshot of the argument's pre-state. Specify an empty initial state and checked representable arithmetic, or use unbounded counts.

The fact that `present` may contain duplicates or zero-count keys is **not itself a violation**: the printed condition expressly requires only a support-covering [sequence](../../../../../../sequence.md). An implementation may strengthen this to an exact, duplicate-free support. Efficiency also needs a cost model or explicit bounds if it is to be a formal guarantee rather than an informal aspiration.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [E](../../e.md)
3. [8](../../../8.md)
4. [Imperative programming (resit)](../../../../imperative-programming-resit-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
