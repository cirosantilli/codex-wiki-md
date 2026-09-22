<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $A_N(f)=(N+1)^{-1}\sum_{n=0}^N f(e^{in\xi})$. For a monomial $z^k$, $k\in\mathbb Z$, the [geometric series](../../../../geometric-series.md) gives

$$
A_N(z^k)=\begin{cases}1,&e^{ik\xi}=1,\\ \displaystyle\frac{1-e^{ik(N+1)\xi}}{(N+1)(1-e^{ik\xi})},&e^{ik\xi}\ne1.\end{cases}
$$

Thus every such average converges, and by [linearity](../../../../linearity.md) so does the average of every [trigonometric polynomial](../../../../trigonometric-polynomial.md). Also $|A_N(f)|\leq\|f\|_\infty$ uniformly in $N$.

Given $\varepsilon>0$, choose a [trigonometric polynomial](../../../../trigonometric-polynomial.md) $P$ with $\|f-P\|_\infty<\varepsilon$. Then

$$
|A_N(f)-A_M(f)|\leq2\varepsilon+|A_N(P)-A_M(P)|.
$$

The last term tends to zero as $N,M\to\infty$. The scalar sequence is Cauchy and therefore **the limit exists for every continuous $f$ and every real $\xi$**.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the real and harmonic analysis course of the University of Oxford](../../../split.md)
5. [Real and harmonic analysis course of the University of Oxford](../../../../real-and-harmonic-analysis-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
