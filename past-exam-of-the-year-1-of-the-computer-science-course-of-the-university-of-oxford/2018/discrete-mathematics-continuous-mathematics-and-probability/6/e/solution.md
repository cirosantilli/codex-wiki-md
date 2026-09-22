<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

With unit strip width, the [composite trapezoidal rule](../../../../../composite-trapezoidal-rule.md) gives

$$
T_{24}=\sum_{i=1}^{25}f(i)-\frac{f(1)+f(25)}2\approx1.037-\frac{0.500+0.002}{2}=0.786.
$$

For [Simpson's rule](../../../../../simpson-s-rule.md), the even integer arguments are the odd-numbered interior grid positions. Therefore

$$
S_{24}=\frac13\left[f(1)+f(25)+4\sum_{i=1}^{12}f(2i)+2\sum_{i=1}^{11}f(2i+1)\right]\approx\frac{0.502+4(0.336)+2(0.200)}3=0.748666\ldots.
$$

The requested two-decimal answers are **$T_{24}\approx0.79$ and $S_{24}\approx0.75$**. The supplied component sums are individually rounded; they should not be treated as exact simultaneous identities. Computing from the original [function](../../../../../function-split.md) gives approximately $0.786685$ and $0.748700$, respectively, with the same two-decimal results.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [6](../../6.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
