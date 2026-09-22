<h1 id="5c/solution">Solution</h1>

↑ **Parent:** [5C](../5c.md)

Put $u=ct-x$ and $v=ct+x$. The [chain rule](../../../../../chain-rule.md) turns the [wave equation](../../../../../wave-equation-split.md) into $4y_{uv}=0$. Integrating first in $v$ and then in $u$ gives the [D'Alembert formula](../../../../../d-alembert-s-formula.md)

$$
y(x,t)=f(ct-x)+g(ct+x).
$$

At the left endpoint, $g(u)=-f(u)$ for $u>0$. At the right endpoint, $f(ct-L)+g(ct+L)=0$, hence

$$
f(v+2L)=f(v)\qquad(v>-L).
$$

Thus the travelling waves can be represented by **$g=-f$, with $f$ and $g$ both $2L$-periodic**. More precisely, the positive-time boundary conditions constrain only $f$ on $(-L,\infty)$ and $g$ on $(0,\infty)$; their unused arguments may be filled in by this periodic extension. They do not constrain arbitrary pre-existing choices outside those ranges. This is [periodic reflection for a fixed-end string](../../../../../periodic-reflection-for-a-fixed-end-string.md).

Using $g=-f$, differentiation gives $y_t=c(f'(ct-x)-f'(ct+x))$ and $y_x=-f'(ct-x)-f'(ct+x)$. The cross terms in the [wave energy](../../../../../wave-energy.md) cancel, so

$$
E(t)=\int_0^L\left(f'(ct-x)^2+f'(ct+x)^2\right)dx
=\int_{ct-L}^{ct+L}f'(s)^2\,ds.
$$

This integrates a $2L$-periodic function over exactly one period. **$E(t)$ is constant.** Equivalently, the [wave equation](../../../../../wave-equation-split.md) gives $E'(t)=[y_ty_x]_0^L=0$, because the fixed endpoint values imply $y_t=0$ there.

## ↑ Ancestors (10)

1. [5C](../5c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
