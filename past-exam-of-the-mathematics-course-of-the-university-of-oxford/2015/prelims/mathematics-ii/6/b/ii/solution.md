<h1 id="6/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose $h_n=\min\{1/n,(b-c)/2\}>0$. Then $h_n\to0$ and $[c,c+h_n]\subset(a,b)$. The [mean value theorem](../../../../../../../mean-value-theorem.md) states that a [continuous function](../../../../../../../continuous-function.md) on a [closed interval](../../../../../../../closed-real-interval.md), [differentiable](../../../../../../../differentiable-function.md) in its interior, has an interior [derivative](../../../../../../../derivative.md) equal to its endpoint [difference quotient](../../../../../../../difference-quotient.md). It gives $x_n\in(c,c+h_n)$ with

$$
f'(x_n)=\frac{f(c+h_n)-f(c)}{h_n}.
$$

Here $x_n\ne c$, $x_n\to c$, and the right-hand side tends to $f'(c)$ by [differentiability](../../../../../../../differentiability.md) at $c$. If $L=\lim_{x\to c}f'(x)$ exists, the same values $f'(x_n)$ must tend to $L$. Uniqueness of the [limit of a sequence](../../../../../../../limit-of-a-sequence.md) gives

$$
\boxed{\lim_{x\to c}f'(x)=f'(c).}
$$

Thus a [derivative](../../../../../../../derivative.md) cannot have a [removable discontinuity](../../../../../../../removable-discontinuity.md) at a point where the original [function](../../../../../../../function-split.md) is [differentiable](../../../../../../../differentiable-function.md). The proof also excludes an infinite [limit of a function](../../../../../../../limit-of-a-function.md) there, since the displayed [difference quotients](../../../../../../../difference-quotient.md) have a finite [limit of a sequence](../../../../../../../limit-of-a-sequence.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
