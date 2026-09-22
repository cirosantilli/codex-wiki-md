<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $x(P)=A/B^2$ in lowest terms, take the logarithmic naive height $h(P)=\log\max\{|A|,B^2\}$. Its required properties are

$$
h(2P)=4h(P)+O(1)
$$

and

$$
h(P+Q)+h(P-Q)=2h(P)+2h(Q)+O(1),
$$

with constants depending only on the curve. Define the [canonical height of an elliptic curve](../../../../../../canonical-height-of-an-elliptic-curve.md) by

$$
\widehat h(P)=\lim_{r\to\infty}4^{-r}h(2^rP).
$$

The first bounded-error relation makes this a convergent telescoping correction to $h(P)$. Apply the second relation to $2^rP,2^rQ$, divide by $4^r$, and let $r\to\infty$ to obtain

$$
\widehat h(P+Q)+\widehat h(P-Q)=2\widehat h(P)+2\widehat h(Q).
$$

Also $\widehat h(2P)=4\widehat h(P)$, and the parallelogram identity then gives $\widehat h(nP)=n^2\widehat h(P)$ for every integer $n$. Thus $\widehat h$ is a quadratic form.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
