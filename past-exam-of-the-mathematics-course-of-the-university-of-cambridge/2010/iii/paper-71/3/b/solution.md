<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For dilute sediment volume concentration $\phi$, define $G=g(\rho_p-\rho_0)/\rho_0$. Neglecting particle volume in the fluid-volume balance,

$$
\boxed{g'=G\phi,\qquad c=\sqrt{\frac23G\phi h}.}
$$

This applies the [Boussinesq approximation](../../../../../../boussinesq-approximation.md) to the bulk mixture, requiring $G\phi/g\ll1$, and uses a deep ambient layer $h\ll H$. A [gravity-current front condition](../../../../../../gravity-current-front-condition.md) closes the unresolved nose. Write it as $\dot L=F\sqrt{g'h}$, with a prescribed order-one front coefficient $F$. If the chosen [Froude number](../../../../../../froude-number.md) is instead $\operatorname{Fr}=\dot L/c$, then $F=\sqrt{2/3}\operatorname{Fr}$.

Use a [parabolic-channel sediment-current box model](../../../../../../parabolic-channel-sediment-current-box-model.md) for one side of the dam: initially its length is $L_0$, depth $h_0$, and uniform concentration $\phi_0$. Its conserved fluid volume is

$$
V=\frac23h^{3/2}L=\frac23h_0^{3/2}L_0,\qquad
h=h_0(L_0/L)^{2/3}.
$$

For vertical settling onto the channel sides, the projected deposition width is $b(h)=\sqrt h$. Thus the total [particle deposition flux](../../../../../../particle-deposition-flux.md) is $W_s\phi\sqrt h\,L$ and

$$
V\dot\phi=-W_s\phi\sqrt h\,L,\qquad
\boxed{\dot\phi=-\frac{3W_s}{2h}\phi,\qquad
\dot L=F\sqrt{G\phi h}.}
$$

The geometric factor $3/2$ follows from $b(h)/A(h)$; using a rectangular deposition formula would give a different result.

Eliminate time and use $h^{3/2}=h_0^{3/2}L_0/L$:

$$
\frac{d\sqrt\phi}{dL}=-\frac{3W_sL}{4F\sqrt G\,h_0^{3/2}L_0},\qquad
\sqrt\phi=\sqrt{\phi_0}-\frac{3W_s(L^2-L_0^2)}{8F\sqrt G\,h_0^{3/2}L_0}.
$$

The [runout length of a gravity current](../../../../../../runout-length-of-a-gravity-current.md) is the limit where suspended concentration vanishes:

$$
\boxed{L_\infty^2=L_0^2+\frac{8F\sqrt{g'_0}\,h_0^{3/2}L_0}{3W_s},\qquad g'_0=G\phi_0.}
$$

The model approaches this length asymptotically in time. It assumes negligible entrainment, erosion and water loss, and does not resolve the initial release or nose. If the initially disturbed region supplies both sides, apply the formula to each side using its share of the initial volume and length.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
