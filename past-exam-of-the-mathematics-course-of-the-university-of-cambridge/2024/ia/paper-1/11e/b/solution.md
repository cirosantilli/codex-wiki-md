<h1 id="11e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the [continuous function](../../../../../../continuous-function.md)

$$
h(x)=g(x+a)-g(x)-a,
\qquad 0\leq x\leq(n-1)a.
$$

At the mesh points its values telescope:

$$
\sum_{k=0}^{n-1}h(ka)
=g(na)-g(0)-na=0.
$$

If one term is zero, the result follows immediately. Otherwise the terms cannot all have the same sign, so there are mesh points at which $h$ is positive and negative. The [intermediate value theorem](../../../../../../intermediate-value-theorem.md) between those points gives an $x\in[0,(n-1)a]$ with $h(x)=0$. Thus the [telescoping increment lemma](../../../../../../telescoping-increment-lemma.md) yields

$$
\boxed{g(x+a)=g(x)+a}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11E](../../11e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
