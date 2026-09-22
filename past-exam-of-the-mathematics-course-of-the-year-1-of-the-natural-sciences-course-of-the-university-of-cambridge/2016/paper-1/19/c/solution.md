<h1 id="19/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For an independent inversion, use the coordinate relations

$$
W=z,\qquad \theta=\arctan\frac{\sqrt{x^2+y^2}}z,\qquad
\phi=\arctan\frac yx.
$$

The positive-octant domain fixes their angle branches unambiguously. Let $s=\sqrt{x^2+y^2}=W\tan\theta$. Differentiating at fixed Cartesian coordinates gives

$$
\theta_x=\frac{z x}{s(z^2+s^2)}=\frac{\cos^2\theta\cos\phi}{W},\qquad
\theta_y=\frac{\cos^2\theta\sin\phi}{W},\qquad
\theta_z=-\frac{\sin\theta\cos\theta}{W},
$$

and $\phi_x=-y/s^2=-\sin\phi/(W\tan\theta)$, $\phi_y=x/s^2=\cos\phi/(W\tan\theta)$, $\phi_z=0$. Hence the inverse [chain rule](../../../../../chain-rule.md) gives

$$
\boxed{(\partial_x)_{y,z}
=\frac{\cos^2\theta\cos\phi}{W}(\partial_\theta)_{W,\phi}
-\frac{\sin\phi}{W\tan\theta}(\partial_\phi)_{W,\theta},}
$$



$$
\boxed{(\partial_y)_{x,z}
=\frac{\cos^2\theta\sin\phi}{W}(\partial_\theta)_{W,\phi}
+\frac{\cos\phi}{W\tan\theta}(\partial_\phi)_{W,\theta},}
$$

and

$$
\boxed{(\partial_z)_{x,y}=(\partial_W)_{\theta,\phi}
-\frac{\sin\theta\cos\theta}{W}(\partial_\theta)_{W,\phi}.}
$$

Multiplying these coefficients by the forward coefficient matrix gives the identity. The original PDF correctly holds $x,y$ fixed in the final [derivative](../../../../../derivative.md); the transcription's $x,z$ subscript there is a typo.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [19](../../19.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
