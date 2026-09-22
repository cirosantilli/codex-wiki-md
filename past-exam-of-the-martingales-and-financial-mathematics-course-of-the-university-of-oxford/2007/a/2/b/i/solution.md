<h1 id="a/2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Expand the fourth power and take [expected values](../../../../../../expected-value-split.md). [independence](../../../../../../independent-random-variables.md) factors products involving distinct indices, and centering makes every term with an index occurring just once have [expected value](../../../../../../expected-value-split.md) zero. The only surviving index patterns are four equal indices and two pairs. There are six orderings of each pair pattern, so

$$
\mathbb ES_n^4
=\sum_{i=1}^n\mathbb EX_i^4
+6\sum_{i<j}\mathbb EX_i^2\,\mathbb EX_j^2.
$$

Uniform boundedness gives $\mathbb EX_i^4\leq c^4$ and $\mathbb EX_i^2\leq c^2$. Hence

$$
\mathbb ES_n^4\leq nc^4+6\binom n2c^4
=(3n^2-2n)c^4\leq\boxed{3c^4n^2.}
$$

Identical distributions were never used: only [independence](../../../../../../independent-random-variables.md), the common bound, and zero means are needed.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [A](../../../../a.md)
5. [2007](../../../../../2007-split.md)
6. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../../split.md)
7. [Martingales and financial mathematics course of the University of Oxford](../../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
