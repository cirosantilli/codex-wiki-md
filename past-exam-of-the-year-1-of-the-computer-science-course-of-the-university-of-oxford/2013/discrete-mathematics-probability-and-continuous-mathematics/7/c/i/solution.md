<h1 id="7/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $H$ mean the added ball was red, and $D$ mean the first draw was red. Their relevant [probabilities](../../../../../../probability.md) are $\mathbb P(H)=\mathbb P(H^c)=1/2$, $\mathbb P(D\mid H)=1$, and $\mathbb P(D\mid H^c)=1/2$. The [law of total probability](../../../../../../law-of-total-probability.md) gives $\mathbb P(D)=3/4$.

Given the observed red draw, the remaining ball is red precisely when $H$ occurred. [Bayes' theorem](../../../../../../bayes-theorem.md) therefore gives

$$
\boxed{\mathbb P(\text{remaining ball red}\mid D)=\mathbb P(H\mid D)=\frac{1\cdot(1/2)}{3/4}=\frac23.}
$$

The observation increases the weight of the two-red-ball box, because that box is more likely to yield a red first draw.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [7](../../../7.md)
4. [Discrete mathematics, probability and continuous mathematics](../../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
5. [2013](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
