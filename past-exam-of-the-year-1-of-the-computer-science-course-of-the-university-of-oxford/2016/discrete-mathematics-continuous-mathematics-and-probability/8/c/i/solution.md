<h1 id="8/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the measurable partition $B_n=\{N=n\}$ for $n\geq0$, omitting any null cells. For $0\leq s\leq1$, the [random variable](../../../../../../random-variable-split.md) $s^X$ is bounded, so the [law of total expectation](../../../../../../law-of-total-expectation.md) applies without moment assumptions. Conditional on $N=n$, the sum contains exactly $n$ terms. Independence of $N$ from the whole sequence preserves their joint law under this conditioning; independence of the $Y_k$ then gives

$$
\mathbb E(s^X\mid N=n)=\mathbb E\left(\prod_{k=1}^n s^{Y_k}\right)
=\prod_{k=1}^n\mathbb E(s^{Y_k})=[G_Y(s)]^n.
$$

For $n=0$ the [empty sum](../../../../../../empty-sum.md) is zero and the [empty product](../../../../../../empty-product.md) is one, in agreement with the formula. Therefore the [probability generating function of an independent random sum](../../../../../../probability-generating-function-of-an-independent-random-sum.md) is

$$
\boxed{G_X(s)=\sum_{n=0}^\infty\mathbb P(N=n)[G_Y(s)]^n=G_N(G_Y(s)).}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [8](../../../8.md)
4. [Discrete mathematics, continuous mathematics and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
