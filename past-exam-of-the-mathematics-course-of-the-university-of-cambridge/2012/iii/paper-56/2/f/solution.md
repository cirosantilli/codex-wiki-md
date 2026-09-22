<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Differentiate $f=g(S,S)$ twice, use [geodesic deviation](../../../../../../geodesic-deviation.md), and eliminate $g(DS,DS)$ with the conserved $K$:

$$
\ddot f=2g(DS,DS)+2g(S,D^2S)=2K+4\kappa f,\qquad \boxed{\ddot f-\frac R3f=2K.}
$$

The most informative way to interpret this [linear differential equation](../../../../../../linear-differential-equation.md) is to express $S$ in a [parallel-propagated orthonormal frame](../../../../../../parallel-propagated-orthonormal-frame.md) along the [timelike geodesic](../../../../../../timelike-geodesic.md). Its three spatial components satisfy $\ddot S^i=\kappa S^i$.

If $R>0$, put $H=\sqrt{R/12}$. With constant spatial vectors $A,B$ in that frame,

$$
S=Ae^{H\tau}+Be^{-H\tau},\qquad f=|A|^2e^{2H\tau}+2A\cdot B+|B|^2e^{-2H\tau},\qquad K=-4H^2A\cdot B.
$$

Thus **generic deviations grow in length like $e^{H\tau}$**, and their squared separation grows like $e^{2H\tau}$. Initially comoving neighbors, $DS(0)=0$, have $S(\tau)=S(0)\cosh(H\tau)$ and exhibit this growth. The unqualified printed assertion is too strong: the nonzero [Jacobi field](../../../../../../jacobi-field.md) $S=Be^{-H\tau}$ has $K=0$ and shrinks exponentially. Such a [Jacobi field](../../../../../../jacobi-field.md) is realizable by varying initial position and initial unit timelike velocity, with initial relative velocity $DS(0)=-HB$.

If $R<0$, put $\omega=\sqrt{-R/12}$. Then

$$
S=A\cos(\omega\tau)+B\sin(\omega\tau),\qquad \ddot f+4\omega^2f=2K.
$$

**The deviations are bounded and oscillatory, rather than exponentially growing.** The squared separation is periodic with period $\pi/\omega$ or is constant. Initially comoving neighbors have $S(\tau)=S(0)\cos(\omega\tau)$ and focus at $\tau=\pi/(2\omega)$; arbitrary vector initial data need not focus together. For completeness, $R=0$ gives $S=A+B\tau$ and $f=|A+B\tau|^2$. These conclusions concern infinitesimal [geodesic deviation](../../../../../../geodesic-deviation.md) on the domain of the variation, not arbitrarily large finite separations.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Paper 56](../../../paper-56-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
