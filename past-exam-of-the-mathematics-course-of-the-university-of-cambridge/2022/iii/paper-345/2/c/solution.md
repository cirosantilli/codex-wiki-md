<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use a well-mixed [gravity-current box model](../../../../../../gravity-current-box-model.md) of length $L(t)$ and depth $h(t)=V_0/L(t)$. Its fixed volume requires $w_e=w_d$. The integrated chemical balance and the standard [gravity-current front condition](../../../../../../gravity-current-front-condition.md) are

$$
V_0\dot\phi=-w_dL\phi,
\qquad
\dot L=\operatorname{Fr}\sqrt{g'(\phi)h}
=\operatorname{Fr}\sqrt{\frac{gV_0}{\rho_0L}(R_1\phi+R_2\phi^2)}.
$$

These two [ordinary differential equations](../../../../../../ordinary-differential-equation.md) are the required integral model.

First suppose $R_1>0$ and put

$$
a=\frac{R_2}{R_1},
\qquad
C=\frac{\operatorname{Fr}V_0}{w_d}
\sqrt{\frac{gV_0R_1}{\rho_0}}.
$$

Eliminating time gives

$$
L^{3/2}\frac{dL}{d\phi}
=-C\sqrt{\frac{1+a\phi}{\phi}}.
$$

With

$$
I(f)=\sqrt{f(1+af)}+\frac1{\sqrt a}\operatorname{arsinh}\sqrt{af},
$$

integration from $(L,\phi)=(L_0,1)$ yields

$$
\boxed{L^{5/2}=L_0^{5/2}+\frac52C\,[I(1)-I(\phi)].}
$$

As $t\to\infty$, the [concentration](../../../../../../concentration.md) tends to zero and the [runout length of a gravity current](../../../../../../runout-length-of-a-gravity-current.md) is

$$
\boxed{L_\infty=
\left\{L_0^{5/2}+\frac52C\left[
\sqrt{1+a}+\frac1{\sqrt a}\operatorname{arsinh}\sqrt a
\right]\right\}^{2/5}.}
$$

The formula has a regular $a\to0$ limit. If $R_1=0<R_2$, direct integration instead gives

$$
L^{5/2}=L_0^{5/2}+\frac52\frac{\operatorname{Fr}V_0}{w_d}
\sqrt{\frac{gV_0R_2}{\rho_0}}(1-\phi),
$$

whose value at $\phi=0$ gives $L_\infty$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
