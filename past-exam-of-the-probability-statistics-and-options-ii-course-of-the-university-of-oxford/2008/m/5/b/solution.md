<h1 id="m/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A state is recurrent if, starting there, the probability of returning at some strictly positive time is one. It is transient if that return probability is strictly less than one. Suppose $i,j$ communicate. Choose $r,s$ with $p_{ji}(r)>0$ and $p_{ij}(s)>0$. Chapman–Kolmogorov gives

$$
p_{jj}(r+n+s)\ge p_{ji}(r)p_{ii}(n)p_{ij}(s).
$$

If $i$ is recurrent, summing over $n$ and using the supplied return-series criterion makes the return series for $j$ diverge, so $j$ is recurrent. Interchanging the states proves equivalence; therefore transience is also constant on a [communicating class](../../../../../communicating-class.md).

For the nearest-neighbor walk, return in an odd number of steps is impossible. A return in $2n$ steps requires exactly $n$ steps each way, so

$$
p_{ii}(2n)=\binom{2n}{n}[p(1-p)]^n\sim\frac{[4p(1-p)]^n}{\sqrt{\pi n}}.
$$

At $p=1/2$, the return series diverges like $\sum n^{-1/2}$. If $0<p<1$ and $p\ne1/2$, then $4p(1-p)<1$, so it converges by exponential decay. At $p=0$ or one the walk never returns. Hence $\boxed{\text{recurrence occurs exactly at }p=1/2}$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [M](../../../m.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
