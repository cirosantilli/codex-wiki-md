<h1 id="5e/solution">Solution</h1>

↑ **Parent:** [5E](../5e.md)

At a positive spatially homogeneous [equilibrium point](../../../../../equilibrium-point-of-a-dynamical-system.md), $v=u^2$ and $2+u-v=0$. Hence **$(u,v)=(2,4)$**. The reaction [Jacobian matrix](../../../../../jacobian-matrix.md) there is

$$
J=\begin{pmatrix}2&-2\\4a&-a\end{pmatrix},\qquad\operatorname{tr}J=2-a,\quad\det J=6a.
$$

The [two-dimensional Routh-Hurwitz stability criterion](../../../../../two-dimensional-routh-hurwitz-stability-criterion.md) gives **strict linear asymptotic stability for $a>2$**, and instability for $0<a<2$.

For a spatial mode with $s=k^2$, the reaction-diffusion [linearization](../../../../../linearization.md) is $J_s=J-\operatorname{diag}(s,ds)$. When $a>2$, its trace is negative for every $s\geq0$, while

$$
D(s)=\det J_s=ds^2+(a-2d)s+6a.
$$

A growing mode exists precisely when this quadratic is negative at some $s>0$. Its minimum must occur at positive $s$, and must be strictly negative, giving

$$
2d>a,\qquad(2d-a)^2>24ad.
$$

With $z=d/a$, the latter inequality becomes $4z^2-28z+1>0$. Selecting the root compatible with $2d>a$ yields the [Turing instability](../../../../../turing-instability.md) threshold

$$
\boxed{d>\left(\frac72+2\sqrt3\right)a.}
$$

The unstable band is

$$
\frac{2d-a-\sqrt{(2d-a)^2-24ad}}{2d}<k^2<\frac{2d-a+\sqrt{(2d-a)^2-24ad}}{2d}.
$$

On a bounded domain a boundary condition must permit a mode in this band. Equality at the threshold gives a neutral mode, not positive growth.

At $a=2$, the homogeneous [linearization](../../../../../linearization.md) has purely imaginary [eigenvalues](../../../../../eigenvalue.md), so it is not strictly linearly asymptotically stable. If “stable” is read as nonlinear stability, the boundary deserves attention. Put $x=u-2$, $y=(v-4-x)/\sqrt3$, and $x=r\cos\theta$, $y=r\sin\theta$. The exact equations give $\dot r=r^2F(\theta)$, $\dot\theta=\omega+rG(\theta)$, where $\omega=2\sqrt3$,

$$
F=-\frac{\cos^2\theta\sin\theta}{\sqrt3}+\cos\theta\sin^2\theta,\qquad G=\frac{2\cos^3\theta}{\sqrt3}+\cos^2\theta\sin\theta+\sqrt3\cos\theta\sin^2\theta.
$$

Expanding $dr/d\theta$ through cubic order, $\int_0^{2\pi}F=0$ cancels the quadratic displacement. The correction from the quadratic change in $r$ also integrates to zero, because it is proportional to $(\int F)^2$. Since $\int_0^{2\pi}FG=\pi/(2\sqrt3)$, the [Poincaré return map](../../../../../poincare-map.md) is

$$
r\longmapsto r-\frac{\pi}{24\sqrt3}r^3+O(r^4).
$$

This [cubic return-map stability of a weak focus](../../../../../cubic-return-map-stability-of-a-weak-focus.md) shows that $a=2$ is a weak attracting focus. The strict linear range used in the [Turing instability](../../../../../turing-instability.md) calculation is $a>2$; the positive homogeneous equilibrium is also nonlinearly asymptotically stable at the boundary $a=2$. For that boundary, $\operatorname{tr}J_s=-(1+d)s<0$ for every nonzero spatial mode. The same strict [Turing instability](../../../../../turing-instability.md) threshold and unstable band therefore also apply there, with the homogeneous mode understood through nonlinear stability.

## ↑ Ancestors (10)

1. [5E](../5e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
