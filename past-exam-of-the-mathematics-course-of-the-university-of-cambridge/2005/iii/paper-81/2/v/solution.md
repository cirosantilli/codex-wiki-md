<h1 id="2/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

In the travelling coordinate $X=x-ct$, [mass conservation](../../../../../../mass-conservation.md) becomes $[\alpha(u-c)]'=0$. Thus the conserved relative flux is $Q$ and

$$
\boxed{u=c+Q/\alpha.}
$$

For a periodic [peristaltic pumping](../../../../../../peristaltic-pumping.md) solution, the neglected-inertia momentum equation is

$$
\widetilde P'(\alpha)\alpha'+\epsilon kP_e\cos kX=-R(\alpha)(c+Q/\alpha).
$$

Take $\alpha_0$ to be the spatial mean area, so $\langle\alpha_1\rangle=\langle\alpha_2\rangle=0$. This normalization, and zero net [pressure](../../../../../../pressure.md) drop over a period, are implicit in the specified periodic forcing. The constant leading state has no [pressure gradient](../../../../../../pressure-gradient.md), giving $Q_0=-\alpha_0c$. Put $B=\widetilde P'_0$ and $d=R_0c/\alpha_0$. At first order,

$$
B\alpha_1'+d\alpha_1=-kP_e\cos kX-R_0Q_1/\alpha_0.
$$

Period averaging gives $Q_1=0$, and the zero-mean solution is

$$
\alpha_1=-\frac{P_e[(d/k)\cos kX+B\sin kX]}{B^2+(d/k)^2},\qquad
\langle\alpha_1^2\rangle=\frac{P_e^2}{2[B^2+(d/k)^2]}.
$$

For the second-order mean balance, expand the [velocity](../../../../../../velocity.md) and friction:

$$
u_1=c\alpha_1/\alpha_0,\qquad
u_2=c\alpha_2/\alpha_0-c\alpha_1^2/\alpha_0^2+Q_2/\alpha_0,\qquad
R_1=-nR_0\alpha_1/\alpha_0.
$$

Averaging the exact [pressure](../../../../../../pressure.md) derivative gives zero, so $\langle R_0u_2+R_1u_1\rangle=0$. Hence the [weak peristaltic pumping of a collapsible tube](../../../../../../weak-peristaltic-pumping-of-a-collapsible-tube.md) result is

$$
\boxed{Q_0=-\alpha_0c,\qquad Q_1=0,\qquad Q_2=\frac{c(n+1)}{2\alpha_0}\frac{P_e^2}{\widetilde P_0'^2+(R_0c/(k\alpha_0))^2}.}
$$

The mean laboratory [volumetric flow rate](../../../../../../volumetric-flow-rate.md) is $c\langle\alpha\rangle+Q=\epsilon^2Q_2+O(\epsilon^3)$, forward with the wave when $c>0$. The negative leading relative flux is therefore consistent with positive mean pumping.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [2](../../2.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
