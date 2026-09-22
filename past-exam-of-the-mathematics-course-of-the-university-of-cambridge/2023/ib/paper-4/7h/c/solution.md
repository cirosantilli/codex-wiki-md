<h1 id="7h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $u(i)$ be the expected number of visits to state $3$ before absorption, counting the present state when $i=3$. Its reward equations are

$$
u(0)=0,
\qquad
u(1)=\frac12u(2),
$$



$$
u(2)=\frac12u(1)+\frac12u(3),
\qquad
u(3)=1+\frac12u(2)+\frac12u(3).
$$

The last equation gives $u(3)=2+u(2)$, so the second nontrivial equation gives $u(2)=2+u(1)$. Hence $u(1)=1+u(1)/2$, and

$$
\boxed{u(1)=2}.
$$

**Thus the expected occupation count is two; together with the previous parts, this is the [four-state reflecting absorbing random walk](../../../../../../four-state-reflecting-absorbing-random-walk.md) calculation.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [7H](../../7h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
