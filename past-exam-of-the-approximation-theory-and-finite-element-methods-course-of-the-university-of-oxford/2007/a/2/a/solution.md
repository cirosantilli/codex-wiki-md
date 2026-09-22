<h1 id="a/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the usual approximation-space convention $P_n=\{p:\deg p\leq n\}$. The source's phrase “degree $n$” must include lower degrees for its later space and [interpolation](../../../../../interpolation-split.md) statements; the consequence of a literal exact-degree reading is addressed in part (d).

Order the alternating points as $x_0<\cdots<x_{n+1}$. If $q$ had strictly smaller error than $E_n$, the values

$$
(q-p)(x_j)=(u-p)(x_j)-(u-q)(x_j)
$$

would have the alternating signs of $(u-p)(x_j)$: the second term has magnitude strictly less than $E_n$. The [intermediate value theorem](../../../../../intermediate-value-theorem.md) would then give at least $n+1$ distinct zeros of $q-p$, one in each gap. A nonzero [polynomial](../../../../../polynomial-split.md) of degree at most $n$ cannot have that many zeros. Thus no such $q$ exists, proving

$$
\boxed{\|u-p\|_\infty\leq\|u-q\|_\infty\quad(q\in P_n).}
$$

The remainder of the equioscillation theorem says that a best uniform approximating [polynomial](../../../../../polynomial-split.md) exists, is unique, and is characterized by this $n+2$-point alternating extreme-error condition. For positive error, alternation is necessary as well as sufficient. If $u$ itself lies in $P_n$, the unique best [polynomial](../../../../../polynomial-split.md) is $u$ with zero error.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
