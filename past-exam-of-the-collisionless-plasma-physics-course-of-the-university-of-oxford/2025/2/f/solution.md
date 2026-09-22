<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Let $J(x)=\int_x^b\kappa(s)\,ds=\eta-I(x)$. The [WKB approximation](../../../../wkb-approximation.md) in the barrier can be rewritten as

$$
E_{\rm II}=\frac{D_R e^{-J}+G_R e^J}{\sqrt\kappa},\qquad
D_R=G e^\eta,\quad G_R=D e^{-\eta}.
$$

The right [Airy turning-point connection formula](../../../../airy-turning-point-connection-formula.md) gives

$$
E_{\rm III}=\frac{2D_R\cos(\Psi-\pi/4)-G_R\sin(\Psi-\pi/4)}{\sqrt{k_3}},
$$

so $A_{\rm t}=D_R+iG_R/2$ and $A_{\rm back}=D_R-iG_R/2$. Impose **no incident [wave](../../../../wave-split.md) from the right**, $A_{\rm back}=0$. Then

$$
D_R=\frac{iG_R}{2},\qquad
G=\frac{iD}{2}e^{-2\eta},\qquad
A_{\rm t}=iD e^{-\eta},\qquad
A_{\rm in}=D\left(1+\frac14e^{-2\eta}\right).
$$

Consequently, within the leading [Airy turning-point connection formula](../../../../airy-turning-point-connection-formula.md) calculation,

$$
t=\frac{A_{\rm t}}{A_{\rm in}}=\frac{i e^{-\eta}}{1+e^{-2\eta}/4},\qquad
r=\frac{A_{\rm r}}{A_{\rm in}}=\frac{1-e^{-2\eta}/4}{1+e^{-2\eta}/4}.
$$

For an opaque barrier, $\eta\gg1$,

$$
\boxed{t\sim i e^{-\eta},\qquad T=|t|^2\simeq e^{-2\eta}.}
$$

The [transmission coefficient](../../../../transmission-coefficient.md) is a ratio of [Poynting fluxes](../../../../poynting-flux.md); the $k^{-1/2}$ normalization already includes their local [wavenumber](../../../../wavenumber.md) factors. The displayed denominator is useful for consistent matching and [Wronskian flux](../../../../wronskian-flux.md) conservation, but does not claim accuracy for subleading terms beyond the [WKB approximation](../../../../wkb-approximation.md), or for merging [wave turning points](../../../../wave-turning-point.md).

## ↑ Ancestors (12)

1. [F](../f.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the collisionless plasma physics course of the University of Oxford](../../../split.md)
5. [Collisionless plasma physics course of the University of Oxford](../../../../collisionless-plasma-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
