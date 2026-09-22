<h1 id="14a/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $s=\log r$, so the two circular boundaries are $s=0$ and $s=2$. The zero angular mode must interpolate between $-1$ and $1$, giving $s-1=\log r-1$.

For the $n$th cosine mode, the radial factor has equal value $A_n$ at both boundaries. The unique [harmonic function](../../../../../../../harmonic-function.md) with those data is

$$
A_n\frac{\cosh(n(s-1))}{\cosh n}\cos(n\theta).
$$

Hence the solution of the annular [Dirichlet problem](../../../../../../../dirichlet-problem.md) is

$$
\boxed{
\phi(r,\theta)
=\log r-1
+\sum_{n=1}^{\infty}
A_n\frac{\cosh(n(\log r-1))}{\cosh n}\cos(n\theta)
}.
$$

At $r=1$ and $r=e^2$, the [hyperbolic cosine](../../../../../../../hyperbolic-cosine.md) quotient equals one, so the [boundary conditions](../../../../../../../boundary-condition.md) are satisfied term by term.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [14A](../../../14a.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ib](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
