<h1 id="m/m5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Stationarity at zero gives $\pi_0=q\pi_0+q\pi_1$, hence $\pi_1=(p/q)\pi_0$. At one, $\pi_1=p\pi_0+q\pi_2$; substituting $p\pi_0=q\pi_1$ gives $q\pi_2=p\pi_1$. More generally the interior equations are $\pi_i=p\pi_{i-1}+q\pi_{i+1}$. Induction gives

$$
\pi_i=(p/q)^i\pi_0.
$$

Since $p/q<1$, normalization of this [geometric series](../../../../../geometric-series.md) gives

$$
\boxed{\pi_i=(1-p/q)(p/q)^i,\qquad i=0,1,\ldots}.
$$

These probabilities satisfy [detailed balance](../../../../../detailed-balance.md) $\pi_ip=\pi_{i+1}q$, including the boundary balance with the holding probability. Thus they do define a [stationary distribution](../../../../../stationary-distribution.md). Irreducibility then gives its uniqueness.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [M5](../../m5.md)
3. [M](../../../m.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
