<h1 id="7h/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $p_n=\mathbb P(X_n=A)$. Whenever the taxi is away from the airport it returns with probability $3/4$, whereas it must leave whenever it is at the airport. Hence

$$
p_{n+1}=\frac34(1-p_n),
\qquad p_0=1.
$$

Subtracting the fixed point $3/7$ gives

$$
p_{n+1}-\frac37=-\frac34
\left(p_n-\frac37\right).
$$

Therefore

$$
\boxed{
p_n=\frac37+\frac47\left(-\frac34\right)^n
}
$$

for every $n\geq0$, and in particular for the requested $n\geq1$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [7H](../../../7h.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ib](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
