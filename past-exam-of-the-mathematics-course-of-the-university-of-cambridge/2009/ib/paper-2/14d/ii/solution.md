<h1 id="14d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Here

$$
F'(z)=\frac\pi b\sinh\frac{\pi z}{b}.
$$

This entire function vanishes exactly at $z=inb$, $n\in\mathbb Z$, and those points map to $\zeta=(-1)^n$. The second [derivative](../../../../../../derivative.md) there is $(\pi/b)^2(-1)^n\ne0$, so each is a simple critical point of the [conformal map](../../../../../../conformal-map.md):

$$
\boxed{z=inb\ (n\in\mathbb Z),\qquad\text{critical values }\zeta=\pm1.}
$$

Take the half-strip

$$
\boxed{D=\{z:\operatorname{Re}z>0,\ 0<\operatorname{Im}z<b\}.}
$$

Writing $\pi z/b=u+iv$, its imaginary part maps to $\sinh u\sin v>0$. More precisely, $w=e^{\pi z/b}$ maps $D$ bijectively onto $\{w:\operatorname{Im}w>0,\ |w|>1\}$, with inverse $z=(b/\pi)\log w$ using arguments in $(0,\pi)$. Then

$$
F(z)=\frac12\left(w+\frac1w\right).
$$

Part (i) with $b=1$, followed by positive real scaling, proves that this second map is a conformal bijection onto the upper half-plane. Their composition proves the required result and gives the [half-strip conformal map by hyperbolic cosine](../../../../../../half-strip-conformal-map-by-hyperbolic-cosine.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [14D](../../14d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
