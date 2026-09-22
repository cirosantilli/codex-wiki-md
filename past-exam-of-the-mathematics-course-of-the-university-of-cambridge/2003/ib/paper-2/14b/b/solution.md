<h1 id="14b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The error $e(f)=f''(0)-f(-1)+2f(0)-f(1)$ is linear and annihilates all degree-at-most-two [polynomials](../../../../../../polynomial-split.md). The [Peano kernel theorem](../../../../../../peano-kernel-theorem.md) with [derivative](../../../../../../derivative.md) order three gives

$$
e(f)=\int_{-1}^1K(t)f'''(t)\,dt,\qquad
K(t)=e_x\left(\frac{(x-t)_+^2}{2}\right).
$$

For $t\ne0$, the second [derivative](../../../../../../derivative.md) of the truncated quadratic at $x=0$ is $\mathbf1_{\{t<0\}}$. Its values at $x=-1,0,1$ then give

$$
K(t)=\mathbf1_{\{t<0\}}+(-t)_+^2-\frac{(1-t)^2}{2}
=\begin{cases}\tfrac12(1+t)^2,&-1<t<0,\\-\tfrac12(1-t)^2,&0<t<1.\end{cases}
$$

The value at the single point $t=0$ is irrelevant to the integral. This is the [centered second-derivative Peano kernel](../../../../../../centered-second-derivative-peano-kernel.md). Its absolute integral is

$$
\int_{-1}^1|K(t)|\,dt
=\frac12\int_{-1}^0(1+t)^2dt+\frac12\int_0^1(1-t)^2dt
=\frac13.
$$

Consequently

$$
\boxed{|e(f)|\le\frac13\|f'''\|_{C[-1,1]}.}
$$

Its changing sign explains why cubic [polynomials](../../../../../../polynomial-split.md) also have zero error: their third [derivative](../../../../../../derivative.md) is constant and $\int_{-1}^1K=0$. No fourth [derivative](../../../../../../derivative.md) is needed for the claimed bound.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [14B](../../14b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
