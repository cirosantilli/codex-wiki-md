<h1 id="7/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Each position is equally likely to receive any coin, so the [law of total probability](../../../../../../law-of-total-probability.md) gives $\mathbb P(A_i)=(1/3+1/2+2/3)/3=1/2$. For two specified positions, the ordered pair of distinct coin biases is uniform over six possibilities. Assuming independent tosses conditional on the order,

$$
\mathbb P(A_1\cap A_2)
=\frac13\left(\frac13\frac12+\frac13\frac23+\frac12\frac23\right)
=\frac{13}{54}\ne\frac14.
$$

Thus **the events are not independent**, even pairwise. The [covariance of draws without replacement](../../../../../../covariance-of-draws-without-replacement.md) explains the difference: the head [indicator random variables](../../../../../../indicator-random-variable.md) have [covariance](../../../../../../covariance.md) $13/54-1/4=-1/108$. Independent physical tosses given the assigned coins do not imply [independence](../../../../../../independent-random-variables.md) after that hidden assignment is averaged out.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [7](../../../7.md)
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
