<h1 id="31a/solution">Solution</h1>

↑ **Parent:** [31A](../31a.md)

At a simple [saddle point](../../../../../saddle-point.md), $\phi'(z_0)=0$ and $\phi''(z_0)\ne0$. On a [method of steepest descent](../../../../../method-of-steepest-descent.md) ray leaving the saddle, choose the oriented local coordinate

$$
z-z_0=\frac{i s}{\sqrt{\phi''(z_0)}},\qquad s\geq0,
$$

with the square-root branch determined by that ray. Then $\phi(z)=\phi(z_0)-s^2/2+O(s^3)$ and $dz=i\,ds/\sqrt{\phi''(z_0)}$ to leading order. For large positive $x$, the effective range is $s=O(x^{-1/2})$. The half-Gaussian integral gives

$$
I_0\sim\frac{i e^{x\phi(z_0)}}{\sqrt{\phi''(z_0)}}\int_0^\infty e^{-xs^2/2}\,ds,
\qquad\boxed{I_0\sim i\sqrt{\frac\pi{2\phi''(z_0)x}}e^{x\phi(z_0)}.}
$$

As usual this saddle contribution presumes the remaining contour is lower in real phase and integrable. Reversing the contour orientation reverses the sign; the square-root convention encodes the chosen outgoing ray.

For the second integral set $t=\sqrt n\,z$. Using the specified logarithm branch,

$$
I=\sqrt n\,n^{-n}\int e^{n\phi(z)}\,dz,\qquad \phi(z)=-z^2-2\log z.
$$

The saddles are $z=\pm i$, and only $z_0=i$ is in the upper half-plane. Here

$$
\phi(i)=1-i\pi,\qquad\phi''(i)=-4.
$$

The contour can be deformed to the horizontal line through $i$, oriented from left to right, without crossing the pole at zero. Along $z=s+i$,

$$
\operatorname{Re}\phi(s+i)=1-s^2-\log(1+s^2),
$$

which has a unique strict maximum at $s=0$ and decays at infinity. This explicitly verifies saddle dominance. Locally $\phi(i+s)=1-i\pi-2s^2+O(s^3)$. Both sides of the saddle contribute a full Gaussian, so

$$
I\sim\sqrt n\,n^{-n}e^{n(1-i\pi)}\int_{-\infty}^\infty e^{-2ns^2}\,ds.
$$

For integer $n$, $e^{-i\pi n}=(-1)^n$, and hence

$$
\boxed{I\sim(-1)^n\sqrt{\frac\pi2}\left(\frac en\right)^n.}
$$

There is no extra factor of two from another saddle: the full Gaussian already accounts for the incoming and outgoing parts at the upper saddle.

## ↑ Ancestors (10)

1. [31A](../31a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
