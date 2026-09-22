<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

Substitute the [linear recurrence relation](../../../../../linear-recurrence-relation.md) for each of $p_{n+2}$ and $q_{n+2}$ in the [discrete Wronskian](../../../../../discrete-wronskian.md):

$$
\begin{aligned}
W_{n+1}
&=p_{n+1}[-b(n)q_{n+1}-c(n)q_n]
 -[-b(n)p_{n+1}-c(n)p_n]q_{n+1}\\
&=c(n)(p_nq_{n+1}-p_{n+1}q_n)=c(n)W_n.
\end{aligned}
$$

Iterating gives

$$
\boxed{W_{n+1}=W_1\prod_{m=1}^nc(m).}
$$

No division was used, so vanishing $c(m)$ cause no exception.

For constant coefficients, seek a solution $x_n=r^n$. The [characteristic equation of a linear recurrence](../../../../../characteristic-equation-of-a-linear-recurrence.md) is $r^2+\alpha r+1=0$. Choose $\theta\in[0,\pi]$ with $\cos\theta=-\alpha/2$. Its roots are $r=e^{i\theta}$ and $e^{-i\theta}$, since $r+r^{-1}=2\cos\theta$. For the two resulting solutions,

$$
\boxed{W_n=e^{-i\theta}-e^{i\theta}=-2i\sin\theta.}
$$

It is independent of $n$, exactly as the product identity predicts when $c(n)=1$.

When $-2<\alpha<2$ the roots are distinct and the [discrete Wronskian](../../../../../discrete-wronskian.md) is nonzero. At $\alpha=-2$ or $2$, the two displayed solutions coincide and $W_n=0$; the identity still holds. If an independent pair is wanted at these endpoints, take $r^n$ and $nr^n$, where $r=1$ or $-1$ respectively. Direct substitution verifies both, and their [discrete Wronskian](../../../../../discrete-wronskian.md) is $r^{2n+1}=r\ne0$.

## ↑ Ancestors (11)

1. [6B](../6b.md)
2. [Section II](../section-ii.md)
3. [Paper 2](../../paper-2-split.md)
4. [Ia](../../split.md)
5. [2004](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
