<h1 id="14e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Set $\Theta=e^{-ikx+ik^2t}$. Expanding the proposed [local relation](../../../../../../local-relation.md) gives

$$
(\Theta q)_t-[\Theta(-kq+iq_x)]_x=\Theta(q_t-iq_{xx}).
$$

Thus its vanishing is exactly $iq_t+q_{xx}=0$. Integrating over $x>0$, using decay at infinity, yields

$$
\frac d{dt}\left(e^{ik^2t}\widehat q(k,t)\right)=e^{ik^2t}[kq(0,t)-iq_x(0,t)].
$$

Integrate in time and use the initial data to obtain the [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md)

$$
\boxed{\widehat q(k,t)=e^{-ik^2t}\left[\widehat q_0(k)+k\widetilde g_0(k^2,t)-i\widetilde g_1(k^2,t)\right],\quad\operatorname{Im}k\leq0.}
$$

Here $\widetilde g_j(z,t)=\int_0^te^{iz\tau}g_j(\tau)\,d\tau$, with $g_0=q(0,\cdot)$ and $g_1=q_x(0,\cdot)$. In particular these finite-time transforms are entire in $z$.

Write $F(k)=e^{ikx-ik^2t}$ and $B_\pm(k)=k\widetilde g_0(k^2,t)\pm i\widetilde g_1(k^2,t)$. Substitution into part (i), including replacing $k$ by $-k$ in the reflected transform, gives

$$
q(x,t)=\frac1{2\pi}\left\{\int_{\mathbb R}F\widehat q_0(k)\,dk+c\int_LF\widehat q_0(-k)\,dk+\int_{\mathbb R}FB_-\,dk-c\int_LFB_+\,dk\right\}.
$$

For the boundary integrands, rotate the negative real ray to the positive imaginary ray through the second quadrant. There are no singularities, and for $k=a+ib$ with $a\leq0,b\geq0$,

$$
\left|e^{ikx-ik^2(t-\tau)}\right|=e^{-bx+2ab(t-\tau)}\leq e^{-bx},\qquad0\leq\tau\leq t.
$$

After writing $FB_+$ as its finite time integral, this estimate and the usual smooth-data arc bounds justify the rotation. The positive real ray stays fixed and the new imaginary ray is directed downwards, giving

$$
\boxed{\int_{\mathbb R}FB_+\,dk=\int_LFB_+\,dk.}
$$

The same argument applies separately to the $\widetilde g_0$ and $\widetilde g_1$ terms. Thus the net boundary integral in the inversion formula is

$$
\int_LF\left[(1-c)k\widetilde g_0-i(1+c)\widetilde g_1\right]dk.
$$

For [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md) choose $c=-1$, eliminating the unknown normal derivative. For [Neumann boundary conditions](../../../../../../neumann-boundary-condition.md) choose $c=+1$, eliminating the unknown boundary value. The resulting [unified transform](../../../../../../fokas-method.md) representations are

$$
\boxed{q_D(x,t)=\frac1{2\pi}\int_{\mathbb R}F\widehat q_0(k)\,dk+\frac1{2\pi}\int_LF[-\widehat q_0(-k)+2k\widetilde g_0(k^2,t)]\,dk,}
$$



$$
\boxed{q_N(x,t)=\frac1{2\pi}\int_{\mathbb R}F\widehat q_0(k)\,dk+\frac1{2\pi}\int_LF[\widehat q_0(-k)-2i\widetilde g_1(k^2,t)]\,dk.}
$$

Each contains only the initial transform and the prescribed boundary transform. The signs depend on the PDF's orientation of $L$, checked above.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [14E](../../14e.md)
3. [Section II](../../section-ii.md)
4. [Paper 1](../../../paper-1-split.md)
5. [Ii](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
