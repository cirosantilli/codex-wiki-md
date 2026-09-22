<h1 id="27j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For one visitor, let

$$
T_0=0,
\qquad
T_j=Z_1+\cdots+Z_j,
$$

and define

$$
p_j(u)=\mathbb P(T_{j-1}\leq u<T_j),
\qquad 1\leq j\leq10.
$$

A visitor arriving at time $s\leq t$ is in room $j$ at time $t$ exactly when its independent service-time mark satisfies $T_{j-1}\leq t-s<T_j$. Thus it receives mark $j$ with probability $p_j(t-s)$; a further mark records that it has already left the gallery.

The [Independent marking theorem for Poisson point processes](../../../../../../independent-marking-theorem-for-poisson-point-processes.md) makes the point processes carrying the different room marks independent. Consequently $V_1(t),\ldots,V_{10}(t)$ are independent, and [Poisson thinning](../../../../../../poisson-thinning-theorem.md) gives

$$
V_j(t)\sim\operatorname{Poisson}(m_j(t)),
\qquad
m_j(t)=\int_0^t\lambda(s)p_j(t-s)\,ds.
$$

Equivalently,

$$
m_j(t)=\int_0^t\lambda(s)
\mathbb P\left(
Z_1+\cdots+Z_{j-1}\leq t-s
<Z_1+\cdots+Z_j
\right)ds.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [27J](../../27j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
