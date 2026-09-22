<h1 id="8f/solution">Solution</h1>

↑ **Parent:** [8F](../8f.md)

Let $L(f)=f'(0)-\mu(f)$. Direct evaluation on $1,x,x^2$ gives $L=0$, so the [Peano kernel theorem](../../../../../peano-kernel-theorem.md) gives

$$
L(f)=\int_0^2K(t)f^{(3)}(t)\,dt,\qquad K(t)=L\left(\frac{(x-t)_+^2}{2}\right).
$$

This representation also follows by applying $L$ to the [Taylor expansion](../../../../../taylor-expansion.md) of $f$ with [integral](../../../../../integral.md) remainder. The [derivative](../../../../../derivative.md) at zero of the truncated quadratic is zero for $t\ge0$, and its sampled values give

$$
K(t)=-(1-t)_+^2+\frac14(2-t)^2=\begin{cases}t-\frac34t^2,&0\le t\le1,\\\frac14(2-t)^2,&1\le t\le2.\end{cases}
$$

The [Peano kernel](../../../../../peano-kernel.md) is nonnegative, and

$$
\int_0^2|K(t)|\,dt=\left[\frac{t^2}{2}-\frac{t^3}{4}\right]_0^1+\int_1^2\frac{(2-t)^2}{4}\,dt=\frac14+\frac1{12}=\frac13.
$$

Hence $|L(f)|\le\frac13\|f^{(3)}\|_\infty$. For $f(x)=x^3/6$, the third [derivative](../../../../../derivative.md) is $1$, while $f'(0)=0$ and $\mu(f)=-1/3$. Thus equality holds, proving **the least constant is $c=1/3$, attained by $f(x)=x^3/6$**.

## ↑ Ancestors (10)

1. [8F](../8f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
