<h1 id="b/5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $f(x)=rx(1-x)$, the [fixed points](../../../../../fixed-point.md) are $x=0$ and $x_*=1-1/r$ when the latter is defined. On the physical interval the nonzero branch exists for $r>1$, meeting zero at $r=1$. Their multipliers are $r$ and $2-r$, respectively. Thus zero is linearly attracting for $0\leq r<1$ and repelling for $r>1$; the positive point is linearly attracting for $1<r<3$ and repelling for $r>3$. At $r=1$ and $r=3$ the relevant multiplier has magnitude one, so [linearization](../../../../../linearization.md) is inconclusive. At $r=1$, $x_{n+1}=x_n-x_n^2$ attracts small positive points to zero nonlinearly.

Factoring $f^2(x)-x$ and removing its fixed-point factors gives $r^2x^2-r(r+1)x+(r+1)=0$. Its distinct roots are

$$
\boxed{x_\pm=\frac{r+1\pm\sqrt{(r-3)(r+1)}}{2r},\qquad r>3.}
$$

They map to each other, giving a genuine [two-cycle](../../../../../period-two-orbit.md) only beyond $r_0=3$. The cycle multiplier is

$$
M=f'(x_+)f'(x_-)=4+2r-r^2.
$$

Solving $|M|<1$ in $r>3$ gives

$$
\boxed{3<r<1+\sqrt6.}
$$

At $r=3$, the two roots coalesce with $x_*=2/3$, where the fixed-point multiplier is $-1$: a supercritical [period-doubling bifurcation](../../../../../period-doubling-bifurcation.md) creates the attracting [two-cycle](../../../../../period-two-orbit.md). At the upper endpoint its multiplier reaches $-1$, marking the next loss of [linear stability](../../../../../linear-stability.md). The [two-cycle](../../../../../period-two-orbit.md) is superstable at $r=1+\sqrt5$, where $M=0$. At exactly $r=3$ the [fixed point](../../../../../fixed-point.md) remains weakly attracting through higher-order terms: for $\eta=x-2/3$, the second iterate is $\eta\mapsto\eta-18\eta^3-27\eta^4$, showing alternating perturbations decay slowly.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../../split.md)
6. [Topics in applied mathematics course of the University of Oxford](../../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
