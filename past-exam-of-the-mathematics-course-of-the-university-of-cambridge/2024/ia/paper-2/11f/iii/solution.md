<h1 id="11f/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $m_j$ be the expected remaining time when the walk is at $j$. The first-step recurrence for [gambler's ruin](../../../../../../gambler-s-ruin.md) is

$$
m_j=1+\frac12m_{j-1}+\frac12m_{j+1},
\qquad -a<j<b,
$$

with $m_{-a}=m_b=0$. The quadratic

$$
m_j=(j+a)(b-j)
$$

satisfies both the recurrence and the [boundary conditions](../../../../../../boundary-condition.md), and their finite linear system has a unique solution. Starting from zero therefore gives

$$
\boxed{\mathbb E(T)=m_0=ab}.
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [11F](../../11f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
