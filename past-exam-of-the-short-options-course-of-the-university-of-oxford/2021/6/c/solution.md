<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With $H>0$, set

$$
s=\sin(\phi/2),\qquad y^{-1/2}+\lambda=\frac Hs,\qquad c=H^2>0,\qquad b=\frac\lambda H.
$$

Then the [first integral](../../../../first-integral.md) gives $1/\sqrt{1+y'^2}=s$. On the descending and ascending halves of the physical track choose respectively $0<\phi<\pi$ and $\pi<\phi<2\pi$, so that $y'=\cot(\phi/2)$. Solving for $y$ gives

$$
\boxed{y(\phi)=\frac{\sin^2(\phi/2)}{c(1-b\sin(\phi/2))^2}.}
$$

The unsquared equation requires $1-bs>0$. At $s=1$ this says **$b<1$**; it is not permissible to retain other values merely because the displayed formula for $y$ has a squared denominator.

For completeness, the [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) also gives $y''=(A'(y)/A(y))(1+y'^2)<0$. Thus $y'$ decreases through zero exactly once, so the chosen parameter runs through the whole single arch without an extra branch. Differentiating the formula for $y$ and dividing by $y'=\cot(\phi/2)$ gives, continuously also at $\phi=\pi$,

$$
\frac{dx}{d\phi}=\frac{\sin^2(\phi/2)}{c(1-b\sin(\phi/2))^3}.
$$

Using $x(0)=0$ yields

$$
\boxed{x(\phi)=\frac1c\int_0^\phi\frac{\sin^2(u/2)}{(1-b\sin(u/2))^3}\,du.}
$$

Since $\sqrt{1+y'^2}=1/\sin(\phi/2)$, the [arc length](../../../../arc-length.md) is obtained by cancelling one factor of $\sin(\phi/2)$ in $dx/d\phi$. The conditions $x(2\pi)=1$ and $S=L$ become

$$
\boxed{\begin{aligned}
c&=\int_0^{2\pi}\frac{\sin^2(u/2)}{(1-b\sin(u/2))^3}\,du,\\
L&=\frac{\displaystyle\int_0^{2\pi}\frac{\sin(u/2)}{(1-b\sin(u/2))^3}\,du}{\displaystyle\int_0^{2\pi}\frac{\sin^2(u/2)}{(1-b\sin(u/2))^3}\,du}.
\end{aligned}}
$$

These determine a unique parameter pair for each $L>1$. To see uniqueness, regard $L$ as the [expected value](../../../../expected-value-split.md) of $1/s$ under a [probability density function](../../../../probability-density-function.md) proportional to $s^2/(1-bs)^3$ on $0<u<2\pi$. [Differentiation under the integral sign](../../../../differentiation-under-the-integral-sign.md) gives the [covariance](../../../../covariance.md) identity

$$
\frac{dL}{db}=3\operatorname{Cov}\!\left(\frac1s,\frac{s}{1-bs}\right)<0.
$$

The first argument decreases with $s$ and the second increases. The strict sign follows by applying $(f(s)-f(t))(g(s)-g(t))<0$ to two independent unequal values and averaging; the integrable endpoint singularity of $1/s$ causes no problem. As $b\uparrow1$, the weight concentrates at $s=1$, so $L\downarrow1$. As $b=-k\to-\infty$, endpoint estimates give numerator $\sim2/k^2$ and denominator $\sim4\log k/k^3$, so $L\sim k/(2\log k)\to\infty$. Continuity then covers every $L>1$. At $b=0$ one recovers the [cycloid](../../../../cycloid.md) and $L=4/\pi$.

**Smoothness qualification.** Near $\phi=0$,

$$
x\sim\frac{\phi^3}{12c},\qquad y\sim\frac{\phi^2}{4c},\qquad y'\to+\infty,
$$

and the other endpoint has $y'\to-\infty$. These are smooth graphs on $0<x<1$, not $C^1$ graphs on the closed interval. Indeed a finite endpoint slope would make the conserved $H$ diverge as $y\to0$. The [travel time](../../../../travel-time.md) remains finite because

$$
T=\frac1{\sqrt{2gc}}\int_0^{2\pi}\frac{d\phi}{(1-b\sin(\phi/2))^2}<\infty\qquad(b<1).
$$

Thus the printed phrase “smooth solution” must be understood on the interior, with improper endpoint limits. The variational calculation supplies necessary stationary arches; it does not by itself prove global minimality in every larger class of tracks.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
