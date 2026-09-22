<h1 id="m/m4/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Under the intended [independent](../../../../../../independent-random-variables.md)-marking interpretation, the coach colors are [independent](../../../../../../independent-random-variables.md) also of the arrival process. Let $K$ be the index of the first white coach. Then $P(K=k)=p(1-p)^{k-1}$, $k\ge1$, independently of the exponential interarrival times. For $p>0$, $T=\sum_{j=1}^KX_j$, so conditioning on $K$ gives

$$
M_T(\theta)=\sum_{k\ge1}p(1-p)^{k-1}\left(\frac\lambda{\lambda-\theta}\right)^k=\frac{\lambda p}{\lambda p-\theta}\quad(\theta<\lambda p).
$$

Thus $\boxed{T\sim\operatorname{Exponential}(\lambda p)}$, the waiting time in the thinned [Poisson process](../../../../../../poisson-process-split.md). If $p=0$, no white coach arrives and $T=+\infty$. [Independence](../../../../../../independent-random-variables.md) of colors from arrival times is needed for this distribution; mutual [independence](../../../../../../independent-random-variables.md) of colors alone would not rule out marks chosen using the interarrival durations.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [D](../../d.md)
3. [M4](../../../m4.md)
4. [M](../../../../m.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options II course of the University of Oxford](../../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
