<h1 id="12d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $G(t)=\int_a^t f(x)\,dx$. At an interior point and for $h\ne0$ small enough,

$$
\frac{G(t+h)-G(t)}h-f(t)=\frac1h\int_t^{t+h}[f(x)-f(t)]\,dx.
$$

By [continuity](../../../../../../continuous-function.md) at $t$, the modulus is bounded by the supremum of $|f(x)-f(t)|$ between $t$ and $t+h$, which tends to zero. Thus **the fundamental theorem of calculus gives**

$$
\boxed{G'(t)=f(t).}
$$

At the interval endpoints the same argument supplies the corresponding one-sided derivatives.

For an integrable discontinuous function, the single-point spike from part (i) has $G\equiv0$, so $G'(c)=0\ne f(c)=1$; this disproves the derivative identity even when the primitive is differentiable. To see that differentiability itself may fail, take the [step function](../../../../../../step-function.md) $f(x)=0$ for $x<c$ and $f(x)=1$ for $x\ge c$. It is [Riemann integrable](../../../../../../riemann-integrable-function.md), but its primitive is $G(t)=\max(0,t-c)$ and has left derivative zero and right derivative one at $c$. Hence the full assertion is false for general [Riemann-integrable functions](../../../../../../riemann-integrable-function.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [12D](../../12d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
