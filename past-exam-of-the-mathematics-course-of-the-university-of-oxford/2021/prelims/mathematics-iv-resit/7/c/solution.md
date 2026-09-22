<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Rearrange the [polynomial](../../../../../../polynomial-split.md) equation as a [fixed point](../../../../../../fixed-point.md) equation:

$$
\boxed{g(x)=\frac{1-x^5}{7},\qquad [a,b]=[0,1/7].}
$$

First establish existence and uniqueness of the target [root of a polynomial](../../../../../../root-of-a-polynomial.md). Since $f$ is a [continuous function](../../../../../../continuous-function.md), $f(0)=-1<0$ and $f(1/7)=1/7^5>0$, the [intermediate value theorem](../../../../../../intermediate-value-theorem.md) gives a [root of a polynomial](../../../../../../root-of-a-polynomial.md) $\xi\in(0,1/7)$. Moreover $f'(x)=5x^4+7>0$ for all real $x$, so $f$ is [strictly increasing](../../../../../../strictly-increasing-function.md) and this is its only real [root of a polynomial](../../../../../../root-of-a-polynomial.md).

For $x\in[0,1/7]$,

$$
0<\frac{1-7^{-5}}7\leq g(x)\leq\frac17,
$$

so $g$ maps the [closed interval](../../../../../../closed-real-interval.md) into itself. Also

$$
|g'(x)|=\frac{5x^4}{7}\leq\frac5{7^5}=q<1.
$$

The [mean value theorem](../../../../../../mean-value-theorem.md) therefore gives $|g(x)-g(y)|\leq q|x-y|$ on the [closed interval](../../../../../../closed-real-interval.md): $g$ is a [contraction mapping](../../../../../../contraction-mapping.md). For any starting value $x_0\in[0,1/7]$, all iterates remain in that [closed interval](../../../../../../closed-real-interval.md), and since $g(\xi)=\xi$,

$$
|x_k-\xi|=|g(x_{k-1})-g(\xi)|\leq q|x_{k-1}-\xi|\leq q^k|x_0-\xi|\longrightarrow0.
$$

Thus **the [fixed-point iteration](../../../../../../fixed-point-iteration.md) converges to the unique real [root of a polynomial](../../../../../../root-of-a-polynomial.md) from every $x_0\in[0,1/7]$**. This explicit error estimate proves the needed convergence directly.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
3. [Mathematics IV resit](../../../mathematics-iv-resit-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
