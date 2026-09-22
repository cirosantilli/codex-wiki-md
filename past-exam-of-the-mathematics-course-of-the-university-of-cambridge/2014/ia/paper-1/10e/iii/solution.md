<h1 id="10e/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $D=f'_+(a)$ and write $g(t)=(f(t)-f(a))/(t-a)$ for $t>a$. By the assumed right [derivative](../../../../../../derivative.md), choose $\delta>0$ with $|g(t)-D|<\epsilon/2$ whenever $a<t<a+\delta$. Choose $b_0\in(a,\min(b,a+\delta))$.

Apply the [mean value theorem](../../../../../../mean-value-theorem.md) to $f$ on $[a,b_0]$. It gives $x\in(a,b_0)$ with $f'(x)=g(b_0)$. Both $g(x)$ and $g(b_0)$ are within $\epsilon/2$ of $D$, so

$$
\boxed{\left|\frac{f(x)-f(a)}{x-a}-f'(x)\right|
\leq|g(x)-D|+|g(b_0)-D|<\epsilon.}
$$

This proves the [endpoint secant-tangent approximation](../../../../../../endpoint-secant-tangent-approximation.md) without any [continuity](../../../../../../continuous-function.md) assumption on $f'$. The [continuity](../../../../../../continuous-function.md) required by the theorem is only that of $f$ itself.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [10E](../../10e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
