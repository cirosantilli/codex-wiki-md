<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the unit-width channel put $\eta=x/L(t)$, $h=h_fH(\eta)$ and $u=\dot L U(\eta)$. Fixed volume gives $V=h_fL\int_0^1H\,d\eta$, so

$$
\boxed{L\dot h_f=-h_f\dot L.}
$$

The closed rear wall has $U(0)=0$. Substituting into [volume conservation](../../../../../../volume-conservation.md) gives $-H-\eta H'+(HU)'=0$, or $[H(U-\eta)]'=0$. The wall sets this constant to zero. Wherever $H>0$, **$U(\eta)=\eta$**. Thus the [velocity](../../../../../../velocity.md) is $u=(\dot L/L)x$ and its material acceleration is $\ddot L\eta$.

Use a constant-Froude [gravity-current front condition](../../../../../../gravity-current-front-condition.md) $\dot L=F\sqrt{g'h_f}$, with the front depth normalized by $H(1)=1$. Differentiating its square and using the volume relation gives $\ddot L=-\dot L^2/(2L)$. The [Euler equation](../../../../../../euler-equations-for-an-inviscid-fluid.md) now reduces to

$$
H'=-\frac{L\ddot L}{g'h_f}\eta=\frac{F^2}{2}\eta.
$$

Integrate from $\eta=1$ to obtain

$$
H=1-\frac{F^2}{4}+\frac{F^2}{4}\eta^2,\qquad
A_F=\int_0^1H\,d\eta=1-\frac{F^2}{6},\qquad h_f=\frac{V}{A_FL}.
$$

A filled rear-wall solution needs $0<F<2$; $F=2$ is the limiting zero rear-depth profile. Integrating the front equation gives the complete [similarity solution](../../../../../../similarity-solution.md)

$$
\boxed{L^3=\frac{9F^2g'V}{4A_F}(t-t_v)^2,\quad
h(x,t)=\frac{V}{A_FL}\left(1-\frac{F^2}{4}+\frac{F^2x^2}{4L^2}\right),\quad
u(x,t)=\frac{2x}{3(t-t_v)}.}
$$

Here $u$ is the horizontal [velocity](../../../../../../velocity.md); the virtual origin $t_v$ accounts for matching to the finite initial release. With the [Benjamin deep-ambient front condition](../../../../../../benjamin-deep-ambient-front-condition.md), $F=\sqrt2$ and $A_F=2/3$, this simplifies to

$$
\boxed{L^3=\frac{27}{4}g'V(t-t_v)^2,\qquad
h=\frac{L^2+x^2}{9g'(t-t_v)^2},\qquad u=\frac{2x}{3(t-t_v)}.}
$$

The volume, wall condition and finite front depth can all be checked directly. Choosing another physically appropriate nose Froude number changes the coefficient and profile; the interior equations alone cannot choose it.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
