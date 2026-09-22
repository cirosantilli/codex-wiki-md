<h1 id="31a/solution">Solution</h1>

↑ **Parent:** [31A](../31a.md)

Put $w=1/z$ and $Y(w)=y(1/w)$. The equation becomes

$$
Y''+\frac2wY'-w^{-n-4}Y=0.
$$

At $w=0$ the regular-singular criterion requires $w(2/w)$ and $w^2(-w^{-n-4})$ to be analytic. This holds precisely for $n\le-2$. Thus the singularity at infinity is irregular, corresponding to essential exponential behaviour of solutions, **exactly for $\boxed{n\ge-1}$**. For $n\le-2$ it is regular singular, with powers and possibly logarithms rather than such essential exponentials.

For $y''=z^3y$, the [Liouville–Green approximation](../../../../../wkb-approximation.md) uses $Q=z^3$, amplitude $Q^{-1/4}$ and phase integral $\int\sqrt Q\,dz=2z^{5/2}/5$. On a consistently chosen branch, the two leading solutions are

$$
\boxed{y_\pm(z)\sim z^{-3/4}\exp\!\left(\pm\frac25z^{5/2}\right).}
$$

The derivative correction is smaller by order $z^{-5/2}$, and the two exponential signs give independent solutions.

Using the convention that [Stokes lines](../../../../../stokes-line.md) have equal exponential phase, $\operatorname{Im}(z^{5/2})=0$, their rays are $\arg z=2\pi k/5$. The equal-magnitude, oscillatory rays, often called [anti-Stokes lines](../../../../../anti-stokes-line.md), satisfy $\operatorname{Re}(z^{5/2})=0$, giving $\arg z=(2k+1)\pi/5$. If the alternative naming convention is used, these two names interchange; the stated equations specify the rays unambiguously.

To give the sector precisely, the solution recessive on the positive axis can be represented by

$$
y_0(z)=\frac2{\sqrt{5\pi}}\sqrt z\,K_{1/5}\!\left(\frac25z^{5/2}\right),
$$

where $K_\nu$ is the [Modified Bessel function of the second kind](../../../../../modified-bessel-function-of-the-second-kind.md). Substitution verifies the differential equation. Its asymptotic $K_\nu(w)\sim\sqrt{\pi/(2w)}e^{-w}$ is valid on closed subsectors of $|\arg w|<3\pi/2$ on the continued branch. Consequently

$$
\boxed{y_0(z)\sim z^{-3/4}e^{-2z^{5/2}/5}\quad\text{for }|\arg z|<3\pi/5.}
$$

Actual exponential decay occurs in the narrower sector $|\arg z|<\pi/5$; in the adjacent portions of the larger asymptotic sector the same continued exponential grows. This distinguishes the validity of the approximation to the positive-axis recessive solution from the directions where its modulus decays.

## ↑ Ancestors (10)

1. [31A](../31a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
