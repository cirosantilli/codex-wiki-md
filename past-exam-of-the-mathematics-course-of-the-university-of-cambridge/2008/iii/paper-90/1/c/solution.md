<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Model the specified drag by a prescribed head loss, $(E+H)_x=-\gamma$. A modified conserved head is consequently

$$
\boxed{\mathcal E_\gamma=H+h+\frac{Q^2}{2gb^2h^2}+\gamma x,}
$$

with an arbitrary reference constant absorbed into $\mathcal E_\gamma$. More generally the last term is $\int_0^x\gamma(s)\,ds$. The effective bed elevation for the [shallow-water specific energy](../../../../../../shallow-water-specific-energy.md) calculation is $H+\gamma x$. The critical momentum equation becomes

$$
(1-F^2)h_x=F^2h\frac{b_x}b-H_x-\gamma.
$$

This is the [head-loss correction to hydraulic control](../../../../../../head-loss-correction-to-hydraulic-control.md).

When $\beta=0$, $b=1$, and regularity at $F=1$ gives $-2\eta x_c+\gamma=0$. Therefore, for $\eta,\gamma>0$,

$$
\boxed{x_c=\frac{\gamma}{2\eta}.}
$$

The effective bed $-\eta x^2+\gamma x$ has a strict maximum there, with elevation increment $\Delta=\gamma^2/(4\eta)$ relative to $x=0$.

Let $d=h(0)$ and require $h_c=2d$. At the control $Q^2=g h_c^3=8gd^3$. At $x=0$ the [shallow-water specific energy](../../../../../../shallow-water-specific-energy.md) is $d+Q^2/(2gd^2)=5d$, while at the control it is $3h_c/2=3d$. Equality of the modified head gives $5d=3d+\Delta$. Hence

$$
\boxed{h(0)=\frac{\gamma^2}{8\eta},\qquad h_c=\frac{\gamma^2}{4\eta},\qquad
Q=\sqrt g\left(\frac{\gamma^2}{4\eta}\right)^{3/2}=\frac{\sqrt g\,\gamma^3}{8\eta^{3/2}}.}
$$

The inlet has $F(0)^2=8$ and is [supercritical flow](../../../../../../supercritical-flow.md); the branch whose depth increases into the control makes the required smooth transition. At the control the increasing branch has slope $h_x=\sqrt{2\eta h_c/3}$, as follows by expanding the modified head to second order.

The numerical discharge uses a constant loss rate on the entire segment from $0$ to $x_c$. The wording specifies that rate only near the control, which is sufficient to locate $x_c$ but does not by itself determine the inlet-to-control head loss. If the loss elsewhere is unspecified, write $\Lambda_c=\int_0^{x_c}\gamma(s)\,ds$. The same calculation gives $h_c=H(x_c)-H(0)+\Lambda_c$ and $Q=\sqrt g\,h_c^{3/2}$; the boxed value is the constant-loss specialization.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 90](../../../paper-90-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
