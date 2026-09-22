<h1 id="9/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

This is a [regular language](../../../../../../regular-language.md). A [deterministic finite automaton](../../../../../../deterministic-finite-automaton.md) needs only to remember the number of consecutive trailing ones, up to three, and whether a forbidden run of four has already occurred. Use states $q_0,q_1,q_2,q_3,q_\times$, start at $q_0$, and accept in $q_0,q_1,q_2,q_3$. Its [transition function of a finite automaton](../../../../../../transition-function-of-a-finite-automaton.md) is:

| State | On $0$ | On $1$ |
| --- | --- | --- |
| $q_0$ | $q_0$ | $q_1$ |
| $q_1$ | $q_0$ | $q_2$ |
| $q_2$ | $q_0$ | $q_3$ |
| $q_3$ | $q_0$ | $q_\times$ |
| $q_\times$ | $q_\times$ | $q_\times$ |

Reading a zero resets the trailing count unless rejection has already occurred. A fourth successive one enters the permanent rejecting state $q_\times$. Thus the accepted [strings](../../../../../../string.md) are exactly those with no substring $1111$, and

$$
\boxed{\text{the bounded-run language is regular}.}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [Calculus, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../../calculus-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
5. [2005](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
