<h1 id="10f/solution">Solution</h1>

↑ **Parent:** [10F](../10f.md)

Let $h_k$ be the probability that the [simple random walk](../../../../../simple-random-walk.md) started at $k$ hits $n$ before zero. The [first-step analysis](../../../../../first-step-analysis.md) recurrence and [boundary conditions](../../../../../boundary-condition.md) are

$$
h_k=ph_{k+1}+qh_{k-1},
\qquad h_0=0,\quad h_n=1.
$$

If $p\ne q$, the [characteristic equation of a linear recurrence](../../../../../characteristic-equation-of-a-linear-recurrence.md) has roots $1$ and $q/p$, so the boundary conditions give

$$
\boxed{h_m=\frac{1-(q/p)^m}{1-(q/p)^n}}.
$$

If $p=q=1/2$, the repeated root gives the limiting formula $\boxed{h_m=m/n}$. This is the [gambler's ruin](../../../../../gambler-s-ruin.md) probability.

For a fixed integer stake $a\leq N$, the fact that $a$ divides $N!$ lets us measure Patricia's wealth in units of £$a$. She starts at $M=N!/a$ and succeeds upon reaching $2M$. The formula above factors as

$$
h_M=\frac{1-r^M}{1-r^{2M}}=\frac1{1+r^M},
\qquad r=\frac qp.
$$

For $p=18/37$, $r=19/18>1$, so this probability increases as $M$ decreases. She should therefore choose the largest stake, $\boxed{a=N}$. For $p=19/37$, $r=18/19<1$, so the probability increases as $M$ increases; she should choose the smallest stake, $\boxed{a=1}$.

## ↑ Ancestors (10)

1. [10F](../10f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
