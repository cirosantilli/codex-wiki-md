<h1 id="b/6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Differentiating the Rodrigues identity gives $H_0=1$ and $H_{n+1}=2tH_n-H_n'$. Induct with the proposed finite sum. The coefficient at $t^{n+1-2j}$ in this recurrence is the contribution from $2tH_n$ minus the derivative contribution with previous index $j-1$:

$$
\frac{n!(-1)^j2^{n+1-2j}}{j!(n-2j)!}-\frac{n!(-1)^{j-1}2^{n-2j+2}}{(j-1)!(n-2j+1)!}.
$$

Using a common denominator, this equals $(n+1)!(-1)^j2^{n+1-2j}/[j!(n+1-2j)!]$. At an endpoint omit terms whose factorial indices would be negative; the same formula then covers the sole remaining term. Thus

$$
\boxed{H_n(t)=n!\sum_{j=0}^{\lfloor n/2\rfloor}\frac{(-1)^j2^{n-2j}}{j!(n-2j)!}t^{n-2j}.}
$$

The initial value and recurrence identify these polynomials with the given Rodrigues definition.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the analysis course of the University of Oxford](../../../../split.md)
6. [Analysis course of the University of Oxford](../../../../../analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
