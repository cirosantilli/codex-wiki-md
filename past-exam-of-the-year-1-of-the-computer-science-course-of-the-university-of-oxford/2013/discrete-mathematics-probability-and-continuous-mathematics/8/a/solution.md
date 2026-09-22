<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [discrete uniform distribution](../../../../../discrete-uniform-distribution.md), each value has [probability](../../../../../probability.md) $1/n$. Using the given finite sums,

$$
\mathbb E[X]=\frac1n\sum_{r=1}^n r=\frac{n+1}{2},\qquad\mathbb E[X^2]=\frac1n\sum_{r=1}^n r^2=\frac{(n+1)(2n+1)}6.
$$

Subtracting the square of the [expected value](../../../../../expected-value-split.md) gives the [variance](../../../../../variance-split.md):

$$
\operatorname{var}(X)=\frac{(n+1)(2n+1)}6-\frac{(n+1)^2}4=\frac{(n+1)(n-1)}{12}.
$$

Hence

$$
\boxed{\mathbb E[X]=\frac{n+1}{2},\qquad\operatorname{var}(X)=\frac{n^2-1}{12}.}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
3. [Discrete mathematics, probability and continuous mathematics](../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
