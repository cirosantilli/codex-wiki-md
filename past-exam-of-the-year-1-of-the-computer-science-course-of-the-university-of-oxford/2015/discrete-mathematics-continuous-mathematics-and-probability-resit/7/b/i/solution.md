<h1 id="7/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

To obtain the $(k+1)$st head on toss $n+1$, the first $n$ tosses must contain exactly $k$ heads, and the last toss must be a head. There are $\binom nk$ choices of the first $k$ head positions. By [independence](../../../../../../independent-random-variables.md), each such arrangement followed by a head has [probability](../../../../../../probability.md) $r^k(1-r)^{n-k}r$. The arrangements are disjoint, so

$$
\boxed{h_{n,k}(r)=\binom nk(1-r)^{n-k}r^{k+1},\qquad n\geq k\geq0.}
$$

This is the [negative binomial stopping argument](../../../../../../negative-binomial-stopping-argument.md), with $n+1$ counting all tosses up to and including the $(k+1)$st success. It is not merely the [probability](../../../../../../probability.md) of $k+1$ heads somewhere among $n+1$ tosses: the last toss is prescribed to be a head.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Discrete mathematics, continuous mathematics, and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
