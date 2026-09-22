<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $a(X)=k_0(X)^{-2}$, $F(y,X)=\cos(n\pi y/R(X))$, and $N(X)=\int_{-R}^{R}F^2dy$. At the next order of the [WKB approximation](../../../../../../../wkb-approximation.md), the transverse operator $L=a\partial_y^2+1-ak^2$ gives

$$
LP_1=i\bigl[(ak)_XAF+2ak(A_XF+AF_X)\bigr].
$$

The moving-wall [Neumann boundary condition](../../../../../../../neumann-boundary-condition.md) gives $P_{1,y}(R)=-ikR_XAF(R)$ and $P_{1,y}(-R)=+ikR_XAF(-R)$. Multiply by $F$ and integrate across the duct. Since $LF=0$ and $F_y=0$ at both walls, [integration by parts](../../../../../../../integration-by-parts.md) gives

$$
\int_{-R}^{R}FLP_1dy=a[FP_{1,y}]_{-R}^{R}=-2iakR_XA.
$$

Also $N_X=2\int FF_Xdy+2R_X$, because $F^2=1$ at both walls. Substituting these identities in the next-order equation produces the transport equation for the [variable-sound-speed WKB duct amplitude](../../../../../../../variable-sound-speed-wkb-duct-amplitude.md):

$$
2akN A_X+(akN)_XA=0.
$$

Consequently $A\sqrt{akN}$ is a complex constant, including a constant phase. For $n\ge1$, $N=R$; for $n=0$, $N=2R$, with the factor two absorbed into the mode's arbitrary constant. Thus

$$
\boxed{A(X)=C\frac{k_0(X)}{\sqrt{k(X)R(X)}}.}
$$

Equivalently,

$$
\frac{A(X)}{A(X_*)}=\frac{k_0(X)}{k_0(X_*)}
\sqrt{\frac{k(X_*)R(X_*)}{k(X)R(X)}}.
$$

There is an independent flux check. The real-coefficient [Helmholtz equation](../../../../../../../helmholtz-equation.md) implies $\nabla\cdot\operatorname{Im}(p^*a\nabla p)=0$, and the wall condition gives zero normal flux. Hence the integrated longitudinal current is constant; at leading order it is $-ak|A|^2N$. This agrees with the transport equation. The factor $k_0$ must be retained: using only $(kR)^{-1/2}$ would ignore the variable coefficient in the given divergence-form equation.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 82](../../../../paper-82-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
