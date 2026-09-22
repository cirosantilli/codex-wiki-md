<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

At a fixed time, the complete spatial derivative is

$$
\boxed{\frac{dS}{dx}=\left(\frac{\partial S}{\partial x}\right)_h+\frac{\partial S}{\partial h}h_x.}
$$

The first term describes geometric variation along the channel at a fixed surface elevation. The second describes the extra wetted area produced by a varying water level; $S_h$ is the surface width.

Assume a fixed channel, negligible lateral inflow, uniform cross-sectional velocity, incompressible water and the hydrostatic long-wave approximation. Integrating [volume conservation](../../../../../../volume-conservation.md) over a short channel segment gives

$$
\boxed{S_t+(Su)_x=0,\qquad
S_h(h_t+uh_x)+Su_x+uS_x=0.}
$$

Inviscid horizontal momentum, with $h$ measured from the fixed datum, is $u_t+uu_x+gh_x=0$. The coefficient matrix acting on $(h_x,u_x)$ has eigenvalues

$$
\boxed{\frac{dx}{dt}=u\pm c,\qquad c^2=\frac{gS}{S_h}.}
$$

These are the [variable-section channel characteristics](../../../../../../variable-section-channel-characteristics.md). Put $D_\pm=\partial_t+(u\pm c)\partial_x$. Adding the corresponding linear combinations of the two equations gives

$$
\boxed{\frac gcD_\pm h\pm D_\pm u=-\frac{uc}{S}S_x.}
$$

The opposite signs in the two combinations cancel both derivative terms in the source calculation.

If $c=c(h)$, then $D_\pm c=c_hD_\pm h$ and $dc^2/dh=2cc_h$. Taking $\xi=t$ along a characteristic gives the requested form

$$
\boxed{\frac{2g}{dc^2/dh}\frac{dc}{d\xi}\pm\frac{du}{d\xi}
=-\frac{uc}{S}\left(\frac{\partial S}{\partial x}\right)_h.}
$$

A sufficient geometry assumption is $S(x,h)=b(x)A(h)$, for which $S/S_h=A/A'$ is independent of $x$ at fixed height.

For a completely general $S(x,h)$, the printed form omits an explicit wave-speed geometry term. The correct conversion is instead

$$
\frac{2g}{\partial_h(c^2)}\left[D_\pm c-(u\pm c)(\partial_xc)_h\right]\pm D_\pm u
=-\frac{uc}{S}S_x.
$$

For example, a lake at rest with constant $h$ but position-dependent $c$ has $D_\pm c=\pm c c_x$. The printed left side is then nonzero while its right side is zero. The $h$-based compatibility equation remains valid, including when $\partial_h(c^2)=0$ makes the speed-based expression singular.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
