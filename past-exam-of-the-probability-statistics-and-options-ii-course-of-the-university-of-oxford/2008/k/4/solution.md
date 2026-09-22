<h1 id="k/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Take source strength $Q$ to mean total two-dimensional flux, so an isolated source has potential $Q\log(z-a)/(2\pi)$. Let $a=1+i$, $b=1/\bar a=(1+i)/2$, and put $c_Q=Q/(2\pi)$. The [circle](../../../../circle.md) theorem gives, up to an additive constant,

$$
w(z)=c_Q[\log(z-a)+\log(z-b)-\log z],\qquad q(z)=w'(z)=c_Q\left[\frac1{z-a}+\frac1{z-b}-\frac1z\right].
$$

The [derivative](../../../../derivative.md) is single valued, which is what the force integrals require. With a positively oriented contour around the [cylinder](../../../../cylinder-geometry.md), the force form of Blasius' theorem is

$$
F_x-iF_y=\frac{i\rho}{2}\oint_C q(z)^2\,dz.
$$

Only the poles at zero and $b$ are enclosed; the physical source at $a$ lies outside. The [residues](../../../../residue.md) of $q^2/c_Q^2$ are $2(1/a+1/b)$ at zero and $2[1/(b-a)-1/b]$ at $b$. Their sum is $2[1/a+1/(b-a)]=-2/a=-(1-i)$. Therefore

$$
\boxed{F_x-iF_y=\frac{\rho Q^2}{4\pi}(1-i),\qquad F_x=F_y=\frac{\rho Q^2}{4\pi}.}
$$

For the second integral, the [residue](../../../../residue.md) of $zq^2/c_Q^2$ at zero is one. At $b$ it is $1+2b[1/(b-a)-1/b]=-3$. Their sum is $-2$. Using precisely the supplied complex-moment convention gives

$$
M-iN=-\frac\rho2(2\pi i)(-2c_Q^2)=\frac{i\rho Q^2}{2\pi},\qquad\boxed{M=0,\quad N=-\frac{\rho Q^2}{2\pi}.}
$$

The vanishing physical moment $M$ is also consistent with [pressure](../../../../pressure-split.md) acting normally to a [circle](../../../../circle.md), hence radially about its centre. If strength is instead defined as the coefficient of $\log(z-a)$, replace $c_Q$ by that strength throughout; stating the flux convention fixes all factors of $2\pi$.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [K](../../k.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
