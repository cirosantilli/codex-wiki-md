<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The constraints give the valid [upper bound](../../../../upper-bound-in-a-partially-ordered-set.md)

$$
x_1+x_2+x_3+x_4=(x_1+x_2+x_4)+x_3\leq5+x_3\leq8-x_1\leq8.
$$

For example $(x_1,x_2,x_3,x_4)=(0,1,3,4)$ satisfies every constraint: the first left side is four, the next three are three, five and two, and $x_4\geq1$. Its objective is eight. Hence the [upper bound](../../../../upper-bound-in-a-partially-ordered-set.md) is attained by an [integer](../../../../integer-split.md) point, proving

$$
\boxed{z_{IP}=8.}
$$

All optimal solutions can also be identified. Equality forces $x_1=0$, $x_3=3$ and $x_2+x_4=5$. The remaining constraints reduce to $x_2\geq1$ and $x_4\geq1$. Thus exactly four [integer](../../../../integer-split.md) optima occur:

$$
\boxed{(x_1,x_2,x_3,x_4)=(0,k,3,5-k),\qquad k=1,2,3,4.}
$$

This is an optimality certificate by a valid relaxation bound and a feasible [integer](../../../../integer-split.md) solution; no assumption of total unimodularity is needed. The source's $\mathbb Z_+$ denotes nonnegative integers, as is also necessary for its assignment equations in the next question.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the integer programming course of the University of Oxford](../../../split.md)
5. [Integer programming course of the University of Oxford](../../../../integer-programming-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
