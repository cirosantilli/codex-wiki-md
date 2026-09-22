<h1 id="7/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Set $H(x)=g(x)-x$. This [function](../../../../../../../function-split.md) is [continuous](../../../../../../../continuous-function.md) on $[a,b]$. Since $g$ takes values in $[a,b]$,

$$
H(a)=g(a)-a\ge0,\qquad H(b)=g(b)-b\le0.
$$

The [intermediate value theorem](../../../../../../../intermediate-value-theorem.md) therefore supplies $\xi\in[a,b]$ with $H(\xi)=0$, equivalently $g(\xi)=\xi$. This includes the possibility that one endpoint is already a [fixed point](../../../../../../../fixed-point.md).

For uniqueness, the [mean value theorem](../../../../../../../mean-value-theorem.md) gives, for any $x,y\in[a,b]$,

$$
|g(x)-g(y)|\le\gamma|x-y|.
$$

If both $\xi$ and $\eta$ are [fixed points](../../../../../../../fixed-point.md), then

$$
|\xi-\eta|=|g(\xi)-g(\eta)|\le\gamma|\xi-\eta|.
$$

Since $\gamma<1$, this forces $|\xi-\eta|=0$. Thus **there exists exactly one [fixed point](../../../../../../../fixed-point.md)**. When $a=b$, the conclusion follows immediately from $g(a)=a$; otherwise the argument above applies. The [contraction mapping](../../../../../../../contraction-mapping.md) estimate also proves convergence of the associated [fixed-point iteration](../../../../../../../fixed-point-iteration.md), as used next.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [7](../../../7.md)
4. [Mathematics IV](../../../../mathematics-iv-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
