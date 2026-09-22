<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $w=N(U)/N(R)$, so $1-w=N(V)/N(R)$. Since class counts add,

$$
\widehat p(R)=w\widehat p(U)+(1-w)\widehat p(V).
$$

The function $g(p)=p(1-p)$ is [concave function](../../../../../../concave-function.md) on $[0,1]$. [Jensen inequality](../../../../../../jensen-s-inequality.md) therefore gives

$$
G(R)=g(\widehat p(R))
\geq wg(\widehat p(U))+(1-w)g(\widehat p(V)),
$$

which is precisely $Q\leq0$. Thus an axis-aligned split cannot increase the weighted empirical Gini impurity.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
