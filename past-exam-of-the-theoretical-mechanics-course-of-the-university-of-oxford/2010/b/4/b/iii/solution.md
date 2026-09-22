<h1 id="b/4/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use $\phi=F(r)\Theta(\theta)Z(z)e^{-i\omega t}$. Periodicity gives $\Theta=\cos m\theta$ or $\sin m\theta$, $m\geq0$, with only the cosine branch for $m=0$. The end-wall conditions give $Z=\cos(\ell\pi z/h)$, $\ell\geq0$. With radial separation constant $\kappa^2$, the remaining equation is

$$
F''+\frac1rF'+\left(\kappa^2-\frac{m^2}{r^2}\right)F=0,
\qquad\omega^2=c_0^2\left(\kappa^2+\frac{\ell^2\pi^2}{h^2}\right).
$$

For $\kappa>0$, boundedness on the axis selects $F=J_m(\kappa r)$. The cylindrical wall then requires $J_m'(\kappa a)=0$. Thus the modes are real and imaginary parts of

$$
\boxed{J_m(k_{m,n}r/a)\{\cos m\theta,\sin m\theta\}
\cos(\ell\pi z/h)e^{-i\omega t},\qquad
\omega^2=c_0^2\left(\frac{k_{m,n}^2}{a^2}+\frac{\ell^2\pi^2}{h^2}\right).}
$$

Here take the positive derivative zeros and include the separate constant radial mode $m=0$, $k=0$. For zero radial separation constant, regularity gives $r^m$ when $m>0$, which fails the wall condition, and a constant for $m=0$. This avoids counting a formal derivative zero at the origin that would make $J_m(0\,r)$ identically zero. The completely constant mode has zero frequency and no [velocity](../../../../../../velocity.md); the remaining modes are acoustic oscillations. The self-adjoint [Neumann Laplacian](../../../../../../neumann-laplacian.md) has these separated modes as a complete system, so no additional nonzero natural frequencies occur.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [B](../../../../b.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the theoretical mechanics course of the University of Oxford](../../../../../split.md)
7. [Theoretical mechanics course of the University of Oxford](../../../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
