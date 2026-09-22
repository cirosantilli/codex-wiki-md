<h1 id="8e/solution">Solution</h1>

↑ **Parent:** [8E](../8e.md)

In the common sector $0<\arg z<\pi/2$, rotate the positive real contour clockwise to the negative imaginary axis. The large quarter-circle contributes zero because $\operatorname{Re}(z\zeta)>0$ there. The rotated ray passes through the simple pole $\zeta=-i$, whose [residue](../../../../../residue.md) is

$$
R=\operatorname{Res}_{\zeta=-i}\frac{e^{-z\zeta}}{1+\zeta^2}=\frac{e^{iz}}{-2i}.
$$

Take a small semicircular indentation into the right half-plane, excluding the pole from the clockwise contour. The downward ray traverses this semicircle clockwise, contributing $-i\pi R$ in the limit. Thus the deformed downward integral is $\widetilde F-i\pi R$, and it equals the original integral. Consequently

$$
\boxed{F(z)-\widetilde F(z)=-i\pi R=\frac\pi2e^{iz}.}
$$

This half-residue, rather than a full $2\pi i$ residue, results from a pole lying on the rotated integration ray.

Parametrizing $\zeta=-iu$ gives

$$
\widetilde F(z)=-i\,\operatorname{PV}\int_0^\infty\frac{e^{izu}}{1-u^2}\,du.
$$

For $\operatorname{Im}z>0$ its tail decays exponentially. Near $u=1$, subtract the pole coefficient before integrating; the remaining integrand is regular, and the principal-value pole term is explicit. This proves holomorphic dependence on $z$ throughout the upper half-plane, locally uniformly on compact subsets. Agreement in the overlap and the [identity theorem](../../../../../identity-theorem.md) therefore give the requested [analytic continuation](../../../../../analytic-continuation.md):

$$
\boxed{F_{\rm continued}(z)=-i\,\operatorname{PV}\int_0^\infty\frac{e^{izu}}{1-u^2}\,du+\frac\pi2e^{iz},\qquad\frac\pi2\le\arg z<\pi.}
$$

## ↑ Ancestors (10)

1. [8E](../8e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
