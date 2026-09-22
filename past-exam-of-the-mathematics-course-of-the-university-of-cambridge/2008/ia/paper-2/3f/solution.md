<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

The [sampling without replacement](../../../../../sampling-without-replacement.md) makes all $\binom n2$ unordered pairs equally likely. The count of red-red pairs is $\binom32=3$, while the count of mixed pairs is $3(n-3)$. Thus their [probabilities](../../../../../probability.md) satisfy

$$
\frac{3(n-3)}{\binom n2}=3\frac3{\binom n2},
$$

and cancellation gives $n-3=3$. Hence $\boxed{n=6}$, with three black socks. The count of black-black pairs is also $\binom32=3$, so

$$
\boxed{\mathbb P(\text{two black socks})=\frac{\binom32}{\binom62}=\frac15.}
$$

The mixed, red-red and black-black [probabilities](../../../../../probability.md) are respectively $3/5,1/5,1/5$, which add to one and verify the given ratio.

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
