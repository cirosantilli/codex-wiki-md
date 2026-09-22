<h1 id="m/m5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A state $i$ is recurrent if the probability of returning to $i$ at a strictly positive time, starting at $i$, equals one. It is transient if that probability is less than one. If $i$ and $j$ communicate, choose $r,s$ with $p_{ji}(r)>0$ and $p_{ij}(s)>0$. Chapman-Kolmogorov gives

$$
p_{jj}(r+n+s)\ge p_{ji}(r)p_{ii}(n)p_{ij}(s).
$$

If $i$ is recurrent, summing over $n$ makes the right-hand side diverge, so the allowed recurrence criterion proves $j$ recurrent. Interchanging $i,j$ proves recurrence is shared throughout a [communicating class](../../../../../communicating-class.md), and therefore transience is shared too.

For the [simple random walk](../../../../../simple-random-walk.md), an odd number of steps cannot return to its starting point, and

$$
p_{00}(2n)=\binom{2n}{n}[p(1-p)]^n\sim\frac{[4p(1-p)]^n}{\sqrt{\pi n}}.
$$

For $p=1/2$ the return series diverges like $\sum n^{-1/2}$, proving recurrence. For $0<p<1$, $p\ne1/2$, its tail is bounded by a convergent geometric series since $4p(1-p)<1$, proving transience. At $p=0$ or $1$ the walk is deterministic and never returns. Translation invariance transfers the conclusion to every state. Thus **recurrence holds exactly when $p=1/2$**.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [M5](../../m5.md)
3. [M](../../../m.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
