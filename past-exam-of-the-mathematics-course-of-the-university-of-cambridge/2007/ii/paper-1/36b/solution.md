<h1 id="36b/solution">Solution</h1>

↑ **Parent:** [36B](../36b.md)

For [lubrication theory](../../../../../lubrication-theory.md), take layer thickness $H$, horizontal length $L$ and speed $U$. Require aspect ratio $\varepsilon=H/L\ll1$, small surface slopes, inertial ratio $UH^2/(\nu L)\ll1$, and slow evolution $H^2/(\nu T)\ll1$. The longitudinal viscous term then dominates the longitudinal derivative term, while transverse momentum is hydrostatic.

Here $\varepsilon\sim\alpha$ and $U\sim gH^2\alpha/\nu$, so sufficient conditions are $\alpha\ll1$ and $gH^3\alpha^2/\nu^2\ll1$, together with the slow-time condition. With atmospheric pressure at the surface, $p=p_{\rm atm}+\rho g\cos\alpha(h-y)$. No slip at the wall and zero surface shear give

$$
u=\frac g\nu(\sin\alpha-\cos\alpha\,h_x)(hy-y^2/2),\qquad
q=\frac{gh^3}{3\nu}(\sin\alpha-\cos\alpha\,h_x).
$$

Depth-integrated [mass conservation](../../../../../mass-conservation.md), $h_t+q_x=0$, therefore gives the stated equation with

$$
\boxed{A=\frac{g\sin\alpha}{3\nu}\sim\frac{g\alpha}{3\nu},\qquad B=\frac{g\cos\alpha}{3\nu}\sim\frac g{3\nu}.}
$$

A steady linear profile with $h_x=A/B=\tan\alpha$ has zero flux: its free surface is horizontal in laboratory coordinates, so the hydrostatic gradient balances downslope gravity. A constant-depth profile also gives steady through-flow.

For the [travelling front of a gravity-driven thin film](../../../../../travelling-front-of-a-gravity-driven-thin-film.md), set $h=F(\xi)$, $\xi=x-ct$. Integrating and using the dry tip gives $-cF=-AF^3+BF^3F'$. The state $F\to h_0$, $F'\to0$ behind the front fixes $\boxed{c=Ah_0^2}$. Consequently $F'=(A/B)(1-h_0^2/F^2)$, and integration with $F(0)=0$ yields

$$
\boxed{\xi=\frac BA\left[F+\frac{h_0}{2}\log\frac{h_0-F}{h_0+F}\right].}
$$

This tends to $-\infty$ as $F\uparrow h_0$. Expanding at zero gives $\xi\sim-BF^3/(3Ah_0^2)$, so $\boxed{F\sim(-3c\xi/B)^{1/3}.}$ The divergent slope at the formal tip violates the small-slope approximation sufficiently close to the [contact line](../../../../../contact-line.md); the interior profile is the lubrication result.

## ↑ Ancestors (10)

1. [36B](../36b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
