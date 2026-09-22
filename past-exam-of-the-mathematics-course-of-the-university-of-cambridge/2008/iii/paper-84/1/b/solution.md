<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a concentrated line release, take $V$ to be actual fluid volume per unit source length and allow symmetric spreading to both sides of $x=0$. Put

$$
H=e^{\Omega t}h,
\qquad s=\frac{1-e^{-\Omega t}}{\Omega},
\qquad \frac{ds}{dt}=e^{-\Omega t}.
$$

Substitution in the [porous medium equation](../../../../../../porous-medium-equation.md) gives the [exponential drainage transform for porous-medium diffusion](../../../../../../exponential-drainage-transform-for-porous-medium-diffusion.md):

$$
H_s=D(HH_x)_x.
$$

The [Barenblatt solution](../../../../../../barenblatt-solution.md) has conserved area $\int_{-\infty}^{\infty}H\,dx=V/\phi$. A quadratic cap satisfies this equation:

$$
\boxed{h(x,t)=\frac{e^{-\Omega t}}{6Ds}
\left[R(t)^2-x^2\right]_+,
\qquad R(t)^3=\frac{9DV}{2\phi}s.}
$$

Indeed, inside the current $H_x=-x/(3Ds)$ and $R\propto s^{1/3}$; differentiating verifies $H_s=D(HH_x)_x$. Its area is $\int H\,dx=2R^3/(9Ds)=V/\phi$, fixing the prefactor. The flux vanishes at the two moving noses because $H=0$ there. Hence the remaining physical volume and occupied width are

$$
\boxed{V(t)=Ve^{-\Omega t},\qquad
2R(t)=2\left[\frac{9DV}{2\phi\Omega}(1-e^{-\Omega t})\right]^{1/3}.}
$$

For a one-sided current on a reflecting half-line, replace the $2$ in $R^3$ by $1$ when $V$ denotes the total release into that side. Volume alone does not select this exact solution for an arbitrary finite initial patch; it describes an impulsive line release. Its initial central height is singular, so a finite injection region and the constraint $h\ll w$ regularize the near-source early-time behavior.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 84](../../../paper-84-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
