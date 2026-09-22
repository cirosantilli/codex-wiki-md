<h1 id="5h/solution">Solution</h1>

↑ **Parent:** [5H](../5h.md)

Take characteristic coordinates $\xi=ct-x$ and $\eta=ct+x$. Then $c^{-2}y_{tt}-y_{xx}=4y_{\xi\eta}$. The [wave equation](../../../../../wave-equation-split.md) is therefore $y_{\xi\eta}=0$, whose general twice-differentiable solution is

$$
\boxed{y(x,t)=f(ct-x)+g(ct+x).}
$$

The first fixed-end boundary gives $f(s)=-g(s)$. The second gives $g(s+L)=g(s-L)$, hence $g(s+2L)=g(s)$; $f$ has the same period. Thus $y=g(ct+x)-g(ct-x)$ with a $2L$-periodic function $g$.

Let $A=g'(ct+x)$ and $B=g'(ct-x)$. Then $y_t=c(A-B)$ and $y_x=A+B$, so the quadratic energy density reduces to $\tfrac12[(A-B)^2+(A+B)^2]=A^2+B^2$. Changing $x$ to $-x$ in the second integral proves

$$
\boxed{\frac12\int_0^L(c^{-2}y_t^2+y_x^2)\,dx=\int_{-L}^L g'(ct+x)^2\,dx.}
$$

The right side integrates a periodic function over one full period and is independent of its starting point. More explicitly its time derivative is $c[g'(ct+L)^2-g'(ct-L)^2]=0$. This is **conservation of the fixed-end wave energy**.

## ↑ Ancestors (10)

1. [5H](../5h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
