<h1 id="6/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

On $(0,1)$, the [product rule](../../../../../../../product-rule.md) and [chain rule](../../../../../../../chain-rule.md) give $f'(x)=2x\sin(1/x)-\cos(1/x)$. On $(-1,0)$, the [function](../../../../../../../function-split.md) is constant and has [derivative](../../../../../../../derivative.md) zero. At zero,

$$
\frac{f(h)-f(0)}h=\begin{cases}h\sin(1/h),&h>0,\\0,&h<0.\end{cases}
$$

Its [absolute value](../../../../../../../absolute-value.md) is at most $|h|$, so the [squeeze theorem](../../../../../../../squeeze-theorem.md) gives $f'(0)=0$. Therefore

$$
\boxed{f'(x)=\begin{cases}2x\sin(1/x)-\cos(1/x),&0<x<1,\\0,&-1<x\leq0.\end{cases}}
$$

For $x_n=1/(2\pi n)$, we have $x_n\to0$ but $f'(x_n)=-1$ for every $n$. This differs from $f'(0)=0$, so $f'$ is not [continuous](../../../../../../../continuous-function.md) at zero. Indeed, $y_n=1/((2n+1)\pi)$ gives $f'(y_n)=1$, so the right-hand [limit of a function](../../../../../../../limit-of-a-function.md) does not exist. Thus **$f$ is [differentiable](../../../../../../../differentiable-function.md) everywhere on $(-1,1)$, while $f'$ is discontinuous at zero.**

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
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
