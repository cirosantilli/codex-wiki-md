<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [gravity-current front condition](../../../../../../gravity-current-front-condition.md) $\dot L=\operatorname{Fr}\sqrt{d\phi h}$, with a specified order-one front [Froude number](../../../../../../froude-number.md). In a [triangular-channel gravity-current box model](../../../../../../triangular-channel-gravity-current-box-model.md), the depth and concentration are uniform over $0<x<L(t)$. The volume is

$$
V=\frac\lambda2h^2L^2=\frac\lambda2H^2L_0^2,
\qquad \boxed{hL=HL_0=:K.}
$$

The horizontal projected deposition area is $\int_0^LT\,dx=\lambda hL^2$. Consequently the integral model is

$$
\boxed{\dot L=\operatorname{Fr}\sqrt{\frac{dK\phi}{L}},\qquad
\dot\phi=-\frac{2W_sL}{K}\phi,\qquad h=\frac KL,\qquad
L(0)=L_0,\quad\phi(0)=\phi_0.}
$$

This front speed is a closure for the integral model, rather than the assertion that its uniform interior is an exact solution of the spatially varying [shallow water equations](../../../../../../shallow-water-equations.md).

Eliminating time and integrating gives

$$
\frac{d\sqrt\phi}{dL}=-\frac{W_sL^{3/2}}{\operatorname{Fr}\sqrt d\,K^{3/2}},\qquad
\sqrt{\phi(L)}=\sqrt{\phi_0}-\frac{2W_s}{5\operatorname{Fr}\sqrt d\,K^{3/2}}(L^{5/2}-L_0^{5/2}).
$$

The limiting [runout length of a gravity current](../../../../../../runout-length-of-a-gravity-current.md) is therefore

$$
\boxed{L_\infty=\left[L_0^{5/2}+\frac{5\operatorname{Fr}\sqrt{g'_0}\,(HL_0)^{3/2}}{2W_s}\right]^{2/5},\qquad g'_0=d\phi_0.}
$$

The additional distance beyond the release gate is $L_\infty-L_0$. The limit is approached asymptotically as $\phi\to0$ and $\dot L\to0$; the idealized box model does not predict a finite-time stop. Its numerical runout depends on the adopted front [Froude number](../../../../../../froude-number.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
