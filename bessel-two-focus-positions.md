# Bessel two focus positions

↑ **Parent:** [Bessel lens displacement method](bessel-lens-displacement-method.md)

Place a converging [thin lens](thin-lens.md) at coordinate $x$ between the object at $0$ and the screen at $L$. In air and the [paraxial approximation](paraxial-approximation.md), the required object and image distances are $u=x$ and $v=L-x$. The [thin lens](thin-lens.md) equation gives a [quadratic equation](quadratic-equation.md):

$$
\frac1f=\frac1x+\frac1{L-x}=\frac{L}{x(L-x)},\qquad x^2-Lx+Lf=0.
$$

Its [discriminant](discriminant.md) is $L^2-4Lf$. For $L>4f>0$, the two roots and their separation are

$$
x_\pm=\frac{L\pm d}{2},\qquad d=x_+-x_-=\sqrt{L^2-4Lf},\qquad x_-+x_+=L.
$$

Both roots lie inside $(0,L)$, and both object and image distances exceed $f$. The two roots therefore describe finite [real images](real-image.md) on the screen. Exchanging the roots exchanges $u,v$; from [transverse magnification](transverse-magnification.md) $m=-v/u$,

$$
m_-=-\frac{L+d}{L-d},\qquad m_+=-\frac{L-d}{L+d},\qquad m_-m_+=1.
$$

The image-height ratio between the enlarged and reduced settings is $|m_-|/|m_+|=|m_-|^2$, rather than $|m_-|$.

At $L=4f$, the roots coincide: $d=0$, $x=L/2=2f$, $u=v=2f$ and $m=-1$. There is one setting, not two separately measurable settings. For $0<L<4f$ the [discriminant](discriminant.md) is negative, so no position between the fixed object and screen gives a sharp [real image](real-image.md) there. This does not forbid a [real image](real-image.md) elsewhere if the screen is moved. Another short proof observes that $x(L-x)$ has maximum $L^2/4$ at $x=L/2$; the focusing requirement $x(L-x)=Lf$ is possible exactly when $L\ge4f$.

## ↑ Ancestors (8)

1. [Bessel lens displacement method](bessel-lens-displacement-method.md)
2. [Thin lens](thin-lens.md)
3. [Lens (optics)](lens-optics.md)
4. [Geometrical optics](geometrical-optics-split.md)
5. [Optics](optics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
