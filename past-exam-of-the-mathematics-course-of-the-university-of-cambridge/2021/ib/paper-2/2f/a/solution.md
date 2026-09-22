<h1 id="2f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\|K\|_\infty=\max_{[0,1]^2}|K|$. For $f,g\in C([0,1])$,

$$
|Tf(x)-Tg(x)|
\leq\int_0^1|K(x,y)|\,|f(y)-g(y)|\,dy
\leq\|K\|_\infty\|f-g\|_\infty.
$$

Taking the supremum over $x$ proves that the [integral operator](../../../../../../integral-operator.md) $T$ is [Lipschitz continuous](../../../../../../lipschitz-continuity.md), hence continuous, in the [uniform norm](../../../../../../supremum-norm.md).

It remains to see that $Tf$ is continuous. Since $K$ is [uniformly continuous](../../../../../../uniform-continuity.md) on the compact square and $f$ is bounded,

$$
|Tf(x)-Tf(x')|
\leq\|f\|_\infty\int_0^1|K(x,y)-K(x',y)|\,dy\to0
$$

as $x'\to x$. Therefore $T:C([0,1])\to C([0,1])$ is well defined and continuous.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2F](../../2f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
