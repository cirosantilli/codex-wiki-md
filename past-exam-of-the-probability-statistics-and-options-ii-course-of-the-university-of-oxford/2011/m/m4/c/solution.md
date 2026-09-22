<h1 id="m/m4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At each index the two independent uniform symbols match with [probability](../../../../../probability.md) $p=k/k^2=1/k$. The match indicators are independent across indices. Consequently the waiting times between successive matches are independent geometric random variables on $1,2,\ldots$ with success [probability](../../../../../probability.md) $p$, and $S_m$ is their sum.

For one waiting time $G$, summing the [geometric series](../../../../../geometric-series.md) gives $\mathbb Ee^{tG}=pe^t/[1-(1-p)e^t]$. Independence yields

$$
\boxed{M_{S_m}(t)=\left(\frac{e^t/k}{1-(1-1/k)e^t}\right)^m,\qquad
\mathbb ES_m=mk.}
$$

For $k>1$ the [moment-generating function](../../../../../moment-generating-function.md) is finite for $t<\log(k/(k-1))$. When $k=1$, every index matches, $S_m=m$ deterministically and the formula reduces to $e^{mt}$ for every real $t$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [M4](../../m4.md)
3. [M](../../../m.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
