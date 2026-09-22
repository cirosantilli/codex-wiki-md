<h1 id="8/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Differentiate the [probability generating function](../../../../../../probability-generating-function.md) equation:

$$
G_N'(s)=pG_N(s)^2+2psG_N(s)G_N'(s).
$$

At $s=1$, $G_N(1)=1$, giving

$$
\boxed{\mathbb E[N]=G_N'(1)=\frac p{1-2p}.}
$$

The [derivative](../../../../../../derivative.md) is finite because $p<1/2$ and the explicit square root has no singularity at $s=1$. Alternatively, the expected population in generation $t$ is $(2p)^t$, so the expected number of splits in that generation is $p(2p)^t$. Summing this nonnegative [geometric series](../../../../../../geometric-series.md) gives the same answer without initially assuming a finite [expected value](../../../../../../expected-value-split.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
