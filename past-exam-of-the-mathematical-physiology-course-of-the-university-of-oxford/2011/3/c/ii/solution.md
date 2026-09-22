<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a purely imaginary root $\lambda=i\omega$ with $\omega>0$, separating real and imaginary parts gives

$$
0=-\cos(\omega\tau),\qquad\omega=\sin(\omega\tau).
$$

Thus $\omega=1$ and $\tau=\pi/2+2\pi m$, $m\geq0$. The first crossing is

$$
\boxed{\tau_c=\pi/2,\qquad\lambda=\pm i.}
$$

For $0<\tau<\pi/2$ there is no root with nonnegative real part. Indeed, write $\lambda=a+ib$ with $a\geq0$. The real equation forces $\cos(b\tau)\leq0$, hence $|b|\tau\geq\pi/2$. But the imaginary equation gives $|b|\leq e^{-a\tau}\leq1$, contradicting $\tau<\pi/2$.

Differentiate the characteristic equation along the root:

$$
\frac{d\lambda}{d\tau}=-\frac{\lambda^2}{1+\tau\lambda},\qquad\left.\operatorname{Re}\frac{d\lambda}{d\tau}\right|_{\lambda=i,\tau=\tau_c}=\frac1{1+\tau_c^2}>0.
$$

The imaginary roots are simple because $1+i\tau_c\ne0$, and they cross into the unstable half-plane as delay increases.

One can also check the nonlinear [Hopf bifurcation](../../../../../hopf-bifurcation.md) directly. With $\theta=\omega t$ and small amplitude $a$, substitute

$$
x=a\cos\theta+a^2\left(\frac15\cos2\theta+\frac1{10}\sin2\theta\right)+O(a^3),\qquad\omega=1+\nu a^2+O(a^3),\quad\tau=\tau_c+\mu a^2+O(a^3).
$$

The constant and second harmonics at order $a^2$ give the displayed coefficients. Put $d=\mu+\tau_c\nu$. At order $a^3$, absence of resonant first harmonics requires $d+1/20=0$ and $\nu+3/20=0$. Hence

$$
\boxed{\nu=-\frac3{20},\qquad\mu=\frac{3\pi-2}{40}>0.}
$$

The nonzero coefficient verifies a branch of small periodic solutions for $\tau>\tau_c$, consistent with the transverse [Hopf bifurcation](../../../../../hopf-bifurcation.md) in the delayed logistic equation. This is the [delayed logistic Hopf threshold](../../../../../delayed-logistic-hopf-threshold.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the mathematical physiology course of the University of Oxford](../../../../split.md)
6. [Mathematical physiology course of the University of Oxford](../../../../../mathematical-physiology-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
