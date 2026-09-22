<h1 id="9e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [arithmetic-geometric mean inequality](../../../../../../arithmetic-geometric-mean-inequality.md) gives

$$
0<a_n\leq\sqrt{a_nb_n}=a_{n+1}\leq b_{n+1}=\frac{a_n+b_n}{2}\leq b_n.
$$

By induction these inequalities hold at every step, so $(a_n)$ is increasing and bounded above by $b$, while $(b_n)$ is decreasing and bounded below by $a$. The [bounded monotone sequence theorem](../../../../../../bounded-monotone-sequence-theorem.md) gives limits $\alpha,\beta$ with $0<a\leq\alpha\leq\beta\leq b$. Taking limits in the [arithmetic mean](../../../../../../arithmetic-mean.md) recurrence gives $\beta=(\alpha+\beta)/2$, whence **$\boxed{\alpha=\beta}$**. Thus both [sequences](../../../../../../sequence.md) converge to the same positive limit, the [arithmetic-geometric mean iteration](../../../../../../arithmetic-geometric-mean-iteration.md)'s limit. No elementary closed formula for that limit is needed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [9E](../../9e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
