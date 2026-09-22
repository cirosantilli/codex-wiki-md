<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume the jump is stationary, short compared with the scale of width variation, hydrostatic on either side, and has negligible bed stress integrated over its short length. Treat its width $b_j=\sqrt{32/27}$ as constant. It must occur on the downstream supercritical branch, at $x_j=L\sqrt{b_j-1}>0$. The discharge from the control gives the local unit-width discharge

$$
q_j=\frac Q{b_j},\qquad q_j^2=\frac{g'H^3}{4}.
$$

Before the jump the energy is still $H$. Writing $y=h/H$, its equation is $y+1/(8y^2)=1$. Its positive roots are $1/2$ and $(1+\sqrt5)/4$; the former is supercritical. Thus

$$
h_1=\frac H2,\qquad u_1=\sqrt{g'H},\qquad F_1^2=2.
$$

Mass conservation gives $h_1u_1=h_2u_2=q_j$. The [hydraulic jump](../../../../../../hydraulic-jump.md) momentum balance conserves $q_j^2/h+g'h^2/2$. Factoring out the non-jump solution $h_2=h_1$ gives the conjugate-depth relation

$$
\frac{h_2}{h_1}=\frac{\sqrt{1+8F_1^2}-1}{2}.
$$

Consequently the conditions immediately after the jump are

$$
\boxed{h_2=\frac{\sqrt{17}-1}{4}H,\qquad
u_2=\frac{2\sqrt{g'H}}{\sqrt{17}-1}
=\frac{\sqrt{17}+1}{8}\sqrt{g'H}.}
$$

Its [Froude number](../../../../../../froude-number.md) is below one. The specific-energy loss is

$$
\boxed{E_1-E_2=\frac{(h_2-h_1)^3}{4h_1h_2}>0.}
$$

Selecting the deeper root of the unchanged energy equation would be wrong: that would conserve the energy across a turbulent jump instead of the momentum.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
