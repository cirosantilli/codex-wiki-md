<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $s_j=\sin\beta_j$, $c_j=\cos\beta_j$. Inverting the two orthogonal [derivative](../../../../../../derivative.md) systems gives, on the vertical axis,

$$
q_x(0,y)=-s_1h_1(y)-c_1j_1(y),\qquad
q_y(0,y)=c_1h_1(y)-s_1j_1(y),
$$

and, on the horizontal axis,

$$
q_x(x,0)=c_2h_2(x)+s_2j_2(x),\qquad
q_y(x,0)=-s_2h_2(x)+c_2j_2(x).
$$

Using the [Wirtinger derivative](../../../../../../wirtinger-derivatives.md) $q_z=(q_x-iq_y)/2$, these become

$$
q_z(iy)=-\frac{e^{-i\beta_1}}2[j_1(y)+ih_1(y)],\qquad
q_z(x)=\frac{e^{i\beta_2}}2[h_2(x)-ij_2(x)].
$$

Define the appropriate boundary transforms by

$$
\begin{aligned}
H_1(k)&=\int_0^\infty e^{ky}h_1(y)\,dy,&J_1(k)&=\int_0^\infty e^{ky}j_1(y)\,dy,\\
H_2(k)&=\int_0^\infty e^{-ikx}h_2(x)\,dx,&J_2(k)&=\int_0^\infty e^{-ikx}j_2(x)\,dx.
\end{aligned}
$$

The first pair is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) for $\operatorname{Re}k<0$; the second pair consists of [Half-range Fourier transforms](../../../../../../half-range-fourier-transform.md), [holomorphic](../../../../../../complex-differentiability-at-a-point.md) for $\operatorname{Im}k<0$. Parametrizing the vertical boundary by $z=iy$ gives $dz=i\,dy$, which must be retained. Substitution yields the [quarter-plane oblique boundary spectral functions](../../../../../../quarter-plane-oblique-boundary-spectral-functions.md):

$$
\boxed{\widehat q_1(k)=\frac{e^{-i\beta_1}}2[H_1(k)-iJ_1(k)],\qquad
\widehat q_2(k)=-\frac{e^{i\beta_2}}2[H_2(k)-iJ_2(k)].}
$$

Their signs follow from the stated clockwise boundary orientations: upward on the left and inward on the bottom.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 86](../../../paper-86-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
