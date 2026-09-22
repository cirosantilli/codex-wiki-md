<h1 id="t/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Against $q$, choosing row $i$ gives Player I expected payoff $(Aq)_i=\sum_ja_{ij}q_j$. The best response maximizes this number; randomizing among rows cannot exceed the largest row payoff. Player II therefore minimizes that maximum, exactly the printed optimization problem.

The [minimax theorem](../../../../../minimax-theorem.md) for a finite [zero-sum game](../../../../../zero-sum-game.md) states

$$
\boxed{v=\min_{q\in\Delta_n}\max_i(Aq)_i
=\max_{p\in\Delta_m}\min_j(p^{\mathsf T}A)_j.}
$$

This common number is the [value of a zero-sum game](../../../../../value-of-a-zero-sum-game.md): Player I can guarantee an expected payoff of at least $v$, and Player II can hold it to at most $v$. At optimal mixed strategies their expected transfer is $v$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [T](../../../t.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
