<h1 id="5/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Use the parameters from (e), and interpret overflow as the number needing simultaneous care exceeding capacity at a randomly chosen time in [stationary distribution](../../../../../stationary-distribution.md). The occupancy of the [immigration--death process](../../../../../immigration-death-process.md) is not fixed at its mean. [Detailed balance](../../../../../detailed-balance.md) gives

$$
\pi_n\alpha=\pi_{n+1}(n+1)\delta,\qquad\pi_n=\pi_0\frac{(\alpha/\delta)^n}{n!}.
$$

Normalizing yields $\pi_0=e^{-25}$, so **stationary occupancy has a [Poisson distribution](../../../../../poisson-distribution.md) with mean 25**. Thus integer capacity $K$ must satisfy

$$
P(X>K)=1-e^{-25}\sum_{n=0}^{K}\frac{25^n}{n!}<0.1.
$$

The adjacent tails are

$$
P(X>31)\approx0.1000679170,\qquad P(X>32)\approx0.0714560312.
$$

Since the tail decreases with $K$, the **minimum capacity is $\boxed{32\ \text{animals}}$**. The small excess above $0.1$ at 31 matters; a [normal approximation](../../../../../normal-approximation.md) rounded too early can choose the wrong integer.

This is a stationary occupancy criterion. If the event is instead an offered arrival finding at least $K$ animals already present in this unrestricted process, [Poisson arrivals see time averages](../../../../../poisson-arrivals-see-time-averages.md) gives $P(X\geq K)$, whose minimum qualifying capacity is 33. That uses a different event definition. From an initially empty centre, occupancy at a finite time is [Poisson distributed](../../../../../poisson-distribution.md) with mean $N(t)\leq25$, so the stationary criterion also bounds the fixed-time overflow probability during initial filling. A probability of ever exceeding capacity over an unlimited future is a different question: this irreducible recurrent process will eventually exceed every finite capacity with probability one. If instead arrivals are refused when all places are occupied, that changes the model to an [loss network](../../../../../loss-network.md), whose blocking probability is not the unrestricted occupancy tail calculated here.

## ↑ Ancestors (13)

1. [F](../f.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
