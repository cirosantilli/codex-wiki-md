<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $p_{xy}=\mathbb P(X=x,Y=y)$, $p_x=\sum_y p_{xy}$, and $q_y=\sum_x p_{xy}$. In bits the [mutual information](../../../../../mutual-information.md) is

$$
I(X;Y)=\sum_{p_{xy}>0}p_{xy}\log_2\frac{p_{xy}}{p_xq_y}.
$$

Terms with zero joint probability contribute zero. On its positive support apply $-\log t\ge1-t$ with $t=p_xq_y/p_{xy}$:

$$
(\log_e2)I(X;Y)\ge\sum_{p_{xy}>0}(p_{xy}-p_xq_y)
=1-\sum_{p_{xy}>0}p_xq_y\ge0.
$$

Equality requires equality in every logarithmic inequality and no product mass outside the joint support, hence $p_{xy}=p_xq_y$ everywhere. Conversely that factorization makes every term zero. Thus **[mutual information](../../../../../mutual-information.md) is nonnegative and vanishes exactly for [independence](../../../../../independent-random-variables.md)**. For countable alphabets the same conclusion follows from the [relative-entropy inequality](../../../../../gibbs-inequality.md), allowing the value $+\infty$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the communication Theory course of the University of Oxford](../../../../split.md)
6. [Communication Theory course of the University of Oxford](../../../../../communication-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
