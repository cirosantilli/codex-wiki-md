<h1 id="38b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write

$$
C=\frac{g\sin\alpha}{3\nu}.
$$

Conservation of the two-dimensional volume $V=\int h\,dx$ suggests

$$
h=t^{-1/3}H(\eta),
\qquad
\eta=xt^{-1/3}.
$$

Substitution into the [scalar conservation law](../../../../../../scalar-conservation-law.md) $h_t+(Ch^3)_x=0$ gives

$$
-\frac13(H+\eta H')+C(H^3)'=0.
$$

The integration constant is zero at the dry rear, so

$$
CH^3-\frac13\eta H=0,
\qquad
H(\eta)=\sqrt{\frac{\eta}{3C}}.
$$

Thus

$$
h(x,t)=\sqrt{\frac{x}{3Ct}},
\qquad 0<x<x_N(t).
$$

The jump from $h_N$ to the dry region is a shock. Its [Rankine-Hugoniot condition](../../../../../../rankine-hugoniot-conditions.md) gives $\dot x_N=Ch_N^2$, which is also satisfied by the similarity profile.

Volume conservation determines the front:

$$
V=\int_0^{x_N}\sqrt{\frac{x}{3Ct}}\,dx
=\frac{2x_N^{3/2}}{3\sqrt{3Ct}}.
$$

Therefore the [finite-volume gravity-driven thin-film current](../../../../../../finite-volume-gravity-driven-thin-film-current.md) has

$$
\boxed{
x_N(t)
=\left(\frac{9gV^2\sin\alpha}{4\nu}t\right)^{1/3}
},
$$

and its head height is

$$
\boxed{
h_N(t)
=\left(\frac{3\nu V}{2g\sin\alpha}\right)^{1/3}t^{-1/3}
}.
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [38B](../../38b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
