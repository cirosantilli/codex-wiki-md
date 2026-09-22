<h1 id="9/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume $a<b$. An increasing [affine map](../../../../../../affine-map.md) sends the two endpoints to zero and one when $ca+d=0$ and $cb+d=1$. Solving gives

$$
\boxed{c=\frac1{b-a},\qquad d=-\frac a{b-a}.}
$$

Indeed, for $0\leq t\leq1$, the [cumulative distribution function](../../../../../../cumulative-distribution-function.md) of the transformed [random variable](../../../../../../random-variable-split.md) is

$$
\mathbb P\left(\frac{V-a}{b-a}\leq t\right)=\mathbb P(V\leq a+(b-a)t)=\frac{a+(b-a)t-a}{b-a}=t,
$$

which is the [cumulative distribution function](../../../../../../cumulative-distribution-function.md) of the [continuous uniform distribution](../../../../../../continuous-uniform-distribution.md) on $[0,1]$.

A decreasing [affine map](../../../../../../affine-map.md) works too, by swapping the endpoints:

$$
\boxed{c=-\frac1{b-a},\qquad d=\frac b{b-a}.}
$$

These are the two possible choices, since the image interval must have endpoints zero and one. The case $a=b$ cannot be transformed into a nondegenerate [continuous uniform distribution](../../../../../../continuous-uniform-distribution.md) by deterministic constants.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [9](../../../9.md)
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
