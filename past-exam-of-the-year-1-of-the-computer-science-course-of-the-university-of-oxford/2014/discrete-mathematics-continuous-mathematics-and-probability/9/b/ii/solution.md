<h1 id="9/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $X_i$ be the head [indicator random variable](../../../../../../indicator-random-variable.md) for toss $i$. These are [independent and identically distributed random variables](../../../../../../independent-and-identically-distributed-random-variables.md) with a [Bernoulli distribution](../../../../../../bernoulli-distribution.md) of parameter $1/2$, so $\mu=1/2$, $\sigma=1/2$, and $W=N/n$. Taking $h=1/5$ makes $h\sigma=1/10$. The preceding [Chebyshev's inequality](../../../../../../chebyshev-s-inequality.md) bound gives

$$
\boxed{\mathbb P\left(0.4\leq\frac Nn\leq0.6\right)
\geq1-\frac{25}{n}\geq\frac34,\qquad n\geq100.}
$$

The endpoints are included because this event is exactly $|W-1/2|\leq1/10$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [Discrete mathematics, continuous mathematics and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2014](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
