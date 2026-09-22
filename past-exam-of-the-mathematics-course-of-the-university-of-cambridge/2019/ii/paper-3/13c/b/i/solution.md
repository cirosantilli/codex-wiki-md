<h1 id="13c/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The additional transition is $n\to n+k$ at rate $\epsilon(n)$. Its gain term at state $n$ comes from state $n-k$, so the new [master equation](../../../../../../../master-equation.md) is

$$
\boxed{
\frac{dp_n}{dt}
=\lambda(p_{n-1}-p_n)
+\beta\bigl((n+1)p_{n+1}-np_n\bigr)
+\epsilon(n-k)p_{n-k}-\epsilon(n)p_n,}
$$

where the gain term is zero when $n<k$. In the generating-function equation the new contribution is

$$
(s^k-1)\sum_{n\geq0}\epsilon(n)p_n s^n.
$$

For a general state-dependent $\epsilon$, this is not closed in $\phi$. Even when it is closed, $s^k-1$ is not proportional to $s-1$ for $k>1$, so the Poisson ansatz used in part (a) is not preserved.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [13C](../../../13c.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
