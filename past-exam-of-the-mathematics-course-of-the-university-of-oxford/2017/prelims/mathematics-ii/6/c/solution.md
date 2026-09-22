<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**No.** On $(-1,1)$ take $c=0$ and

$$
f(x)=\begin{cases}x^2\sin(1/x),&x\ne0,\\0,&x=0.\end{cases}
$$

At zero, its [difference quotient](../../../../../../difference-quotient.md) has [absolute value](../../../../../../absolute-value.md) $|x\sin(1/x)|\leq|x|\to0$, so $f'(0)=0$. Away from zero, the [product rule](../../../../../../product-rule.md) and [chain rule](../../../../../../chain-rule.md) apply. Define

$$
A_n=2\pi n,\qquad B_n=\begin{cases}\pi/2,&n\text{ even},\\3\pi/2,&n\text{ odd},\end{cases}\qquad x_n=\frac1{A_n},\quad y_n=\frac1{A_n+B_n}\qquad(n\geq1).
$$

These are distinct positive inputs tending to zero. Since $\sin A_n=0$ and $\sin(A_n+B_n)=\sin B_n$,

$$
\frac{f(y_n)-f(x_n)}{y_n-x_n}=-\frac{\sin B_n}{B_n}\frac{A_n}{A_n+B_n}.
$$

The even-indexed [subsequence](../../../../../../subsequence.md) tends to $-2/\pi$, whereas the odd-indexed [subsequence](../../../../../../subsequence.md) tends to $2/(3\pi)$. Thus the [limit of a sequence](../../../../../../limit-of-a-sequence.md) does not exist. The two points lie on the same side of $c$, so the nonnegative-weight estimate in part (b) is unavailable. This is a concrete instance of [differentiability does not imply continuity of the derivative](../../../../../../differentiability-does-not-imply-continuity-of-the-derivative.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [Mathematics II](../../../mathematics-ii-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
