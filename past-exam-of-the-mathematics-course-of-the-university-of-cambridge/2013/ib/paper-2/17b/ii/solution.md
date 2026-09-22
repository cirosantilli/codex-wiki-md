<h1 id="17b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $p=\sqrt{2mE}/\hbar$ and $\gamma=mk/\hbar^2$. Integrating the [Schrödinger equation](../../../../../../schrodinger-equation.md) across the [delta potential](../../../../../../delta-potential.md) gives continuity of $\psi$ and

$$
\psi'(0+)-\psi'(0-)=2\gamma\psi(0).
$$

For incidence from the left, write $\psi=e^{ipx}+r e^{-ipx}$ on $x<0$ and $\psi=t e^{ipx}$ on $x>0$. Matching gives $t=1+r$ and $ip(t-1+r)=2\gamma t$, hence

$$
r=-\frac{i\gamma}{p+i\gamma},\qquad t=\frac p{p+i\gamma}.
$$

The incident and transmitted [probability currents](../../../../../../probability-current.md) have the same velocity factor, so the [reflection coefficient](../../../../../../reflection-coefficient.md) and [transmission coefficient](../../../../../../transmission-coefficient.md) are

$$
\boxed{R=\frac{\gamma^2}{p^2+\gamma^2},\qquad T=\frac{p^2}{p^2+\gamma^2},\qquad R+T=1.}
$$

For $k<0$, an even [bound state](../../../../../../bound-state.md) has $\psi=Ae^{-\kappa|x|}$, $\kappa=\sqrt{-2mE}/\hbar$. The [derivative](../../../../../../derivative.md) jump now gives $-2\kappa A=2\gamma A$, so $\kappa=-\gamma>0$ and

$$
\boxed{E=-\frac{mk^2}{2\hbar^2}.}
$$

There is exactly one positive value of $\kappa$, hence exactly one even [bound state](../../../../../../bound-state.md). Its normalized amplitude is $A=\sqrt\kappa$. An odd decaying solution would have to vanish at zero and is therefore trivial.

In the shrinking [finite square well](../../../../../../finite-square-well.md), its integrated potential is $k=-2Ul$, not $-Ul$: the full width is $2l$. With $Ul$ fixed and $l\to0$, $0\leq(\alpha l)^2\leq2mUl^2/\hbar^2\to0$. The matching condition then bounds $\beta$ by $(2mUl/\hbar^2)(1+o(1))$, so $E$ remains bounded. Consequently $El\to0$, and the previous matching condition gives

$$
\beta=\alpha\tan(\alpha l)\sim\alpha^2l=\frac{2m(U+E)l}{\hbar^2}\longrightarrow-\frac{mk}{\hbar^2}.
$$

Using $E=-\hbar^2\beta^2/(2m)$ recovers the same bound-state energy. All other even levels disappear as the width shrinks.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [17B](../../17b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
