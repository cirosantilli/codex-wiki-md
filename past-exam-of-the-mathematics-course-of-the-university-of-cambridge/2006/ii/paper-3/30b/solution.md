<h1 id="30b/solution">Solution</h1>

↑ **Parent:** [30B](../30b.md)

Put $t=\sqrt z\,\tau$ and $L=z^{3/2}$. The [steepest descent](../../../../../method-of-steepest-descent.md) phase is $F(\tau)=-\tau^3/3+\tau$, with saddles at $\pm1$. The specified contour can be deformed through the negative saddle, where $F(-1)=-2/3$; the positive saddle would produce the growing exponential and is not the saddle for this contour.

An explicit descending contour is $\tau=u+iv$, where $u=-\sqrt{1+v^2/3}$ and $v$ increases from negative to positive infinity. Its imaginary phase is $v(1-u^2+v^2/3)=0$, and its ends approach the prescribed rays $4\pi/3$ and $2\pi/3$. The real part of the phase has a strict maximum at $v=0$, with quadratic term $-v^2$. Since the integrand is entire and decays in the connecting sectors, contour deformation introduces no residue.

Near the saddle, write $\tau=-1+is+O(s^2)$. Then $F(\tau)=-2/3-s^2+O(s^3)$ and $d\tau=i(1+O(s))ds$. The [Gaussian](../../../../../normal-distribution.md) saddle contribution is therefore

$$
\operatorname{Ai}(z)\sim\frac{\sqrt z}{2\pi i}i e^{-2L/3}\int_{-\infty}^{\infty}e^{-Ls^2}ds=\boxed{\frac{e^{-2z^{3/2}/3}}{2\sqrt\pi\,z^{1/4}}}.
$$

The remainder of the descending contour has smaller real phase, so does not alter this leading term.

## ↑ Ancestors (10)

1. [30B](../30b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
