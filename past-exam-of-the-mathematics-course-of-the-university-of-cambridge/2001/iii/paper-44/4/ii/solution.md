<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For constant [porosity](../../../../../../porosity.md) and permeability, the equation is $h_T+h_X=\nabla_{X,Y}\cdot(h\nabla_{X,Y}h)$. Under $\tau=T$, $\xi=X-T$, $\eta=Y$, the chain rule gives $h_T=h_\tau-h_\xi$ and $h_X=h_\xi$. Thus the moving-frame [porous medium equation](../../../../../../porous-medium-equation.md) is

$$
\boxed{h_\tau=\nabla_{\xi,\eta}\cdot(h\nabla_{\xi,\eta}h)
=\tfrac12\nabla_{\xi,\eta}^2(h^2).}
$$

Its conserved mass is $M=\iint h\,d\xi\,d\eta$.

There is a source inconsistency in the printed volume formula. Actual liquid volume is $V=P\iint h\,dx\,dy$. The stated coordinates have [Jacobian determinant](../../../../../../jacobian-determinant.md)

$$
dx\,dy=\frac{dX\,dY}{\tan^2\theta}
=\frac{d\xi\,d\eta}{\tan^2\theta},
$$

so the [volume Jacobian for downslope stretched coordinates](../../../../../../volume-jacobian-for-downslope-stretched-coordinates.md) requires

$$
\boxed{V=P\cot^2\theta\iint h\,d\xi\,d\eta,
\qquad M=\frac{V\tan^2\theta}{P}.}
$$

The printed factor $\tan^2\theta$ in the first expression is its reciprocal and cannot be proved with these coordinates. For example, at $\theta=\pi/6$ an integral equal to one corresponds to actual volume $3P$, whereas the printed formula gives $P/3$. The physical-volume normalization below uses the corrected Jacobian.

Let $r=\sqrt{\xi^2+\eta^2}$. For the source-type axisymmetric [similarity solution](../../../../../../similarity-solution.md), put

$$
h=\tau^{-a}f(s),\qquad s=r\tau^{-b}.
$$

Mass conservation imposes $a=2b$, and balancing $h_\tau$ against $\nabla\cdot(h\nabla h)$ gives $a+1=2a+2b$. Hence $a=1/2$ and $b=1/4$. The profile equation is

$$
-\tfrac12f-\tfrac14sf'
=\frac1s(sf f')'.
$$

Multiplying by $s$, the left side is $-\tfrac14(s^2f)'$. Integration and regularity at the origin give

$$
sff'=-\tfrac14s^2f.
$$

Where $f>0$, divide by $sf$ to obtain $f'=-s/4$, so

$$
f(s)=C-\frac{s^2}{8},\qquad 0\le s\le\sqrt{8C}.
$$

Set the profile to zero beyond this front. The mass normalization is

$$
M=2\pi\int_0^{\sqrt{8C}}\left(C-\frac{s^2}{8}\right)s\,ds
=4\pi C^2.
$$

Therefore the [two-dimensional Barenblatt profile for quadratic porous-medium diffusion](../../../../../../two-dimensional-barenblatt-profile-for-quadratic-porous-medium-diffusion.md) is

$$
\boxed{h(r,\tau)=\left[
\sqrt{\frac{M}{4\pi\tau}}-\frac{r^2}{8\tau}\right]_+,
\qquad M=\frac{V\tan^2\theta}{P},}
$$

where $[q]_+=\max(q,0)$. Its radius and central thickness are

$$
\boxed{r_N(\tau)=\left(\frac{16M\tau}{\pi}\right)^{1/4},\qquad
h(0,\tau)=\sqrt{\frac{M}{4\pi\tau}}.}
$$

The profile is regular at the center, its flux $-hh_r$ vanishes at the dry edge, and the front speed $r_N'=r_N/(4\tau)$ equals the limiting advective speed $-h_r$ there. Its support shrinks to the release point as $\tau\downarrow0$ while its mass stays $M$, giving the concentrated initial release in the weak sense.

In physical coordinates its center travels at

$$
x_c(t)=\frac{\rho gK\sin\theta}{\mu P}t,
$$

and $r=\tan\theta\sqrt{(x-x_c)^2+y^2}$ with $\tau=\rho gK\sin\theta\tan\theta\,t/(\mu P)$. If the printed volume expression were instead adopted merely as a definition of a formal parameter $\widetilde V$, the same profile would use $M=\widetilde V/(P\tan^2\theta)$; that parameter would equal $V\tan^4\theta$, not the actual released fluid volume.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
