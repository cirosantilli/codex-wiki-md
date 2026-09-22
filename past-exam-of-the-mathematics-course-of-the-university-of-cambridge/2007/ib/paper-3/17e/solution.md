<h1 id="17e/solution">Solution</h1>

↑ **Parent:** [17E](../17e.md)

Neglect end effects, so the [electrostatic potential](../../../../../electric-potential.md) depends only on the cylindrical radius $r$. The radial [Laplace equation](../../../../../laplace-equation.md) is $(r\phi')'=0$, with general solution $A\log r+B$. Imposing the conductor [boundary conditions](../../../../../boundary-condition.md) gives

$$
\boxed{\phi(r)=\begin{cases}\displaystyle V\frac{\log(r/a)}{\log\lambda},&a<r<\lambda a,\\[6pt]\displaystyle V\frac{\log(2a/r)}{\log(2/\lambda)},&\lambda a<r<2a.\end{cases}}
$$

The radial [electric field](../../../../../electric-field.md) is $E_r=-\phi'$. Just inside the middle cylinder it is $-V/[\lambda a\log\lambda]$, directed towards the inner cylinder; just outside it is $V/[\lambda a\log(2/\lambda)]$, directed towards the outer cylinder. By [Gauss's law](../../../../../gauss-s-law.md), its [charge per unit length](../../../../../linear-charge-density.md) is

$$
q'=2\pi\epsilon_0\lambda a\bigl(E_r(\lambda a+)-E_r(\lambda a-)\bigr)=2\pi\epsilon_0V\left(\frac1{\log\lambda}+\frac1{\log(2/\lambda)}\right).
$$

Hence the [capacitance per unit length](../../../../../capacitance-per-unit-length.md) is

$$
\boxed{C(\lambda)=2\pi\epsilon_0\left(\frac1{\log\lambda}+\frac1{\log(2/\lambda)}\right).}
$$

The two [coaxial cylindrical capacitors](../../../../../coaxial-cylindrical-capacitor.md) contribute in parallel because both connect the middle cylinder to the same grounded potential. This is the [coaxial capacitor with grounded inner and outer cylinders](../../../../../coaxial-capacitor-with-grounded-inner-and-outer-cylinders.md) construction.

For $\lambda=1+\delta$ with $\delta\to0^+$, $\log\lambda=\delta+O(\delta^2)$ while $\log(2/\lambda)\to\log2$. Therefore

$$
\boxed{C(1+\delta)\sim\frac{2\pi\epsilon_0}{\delta}.}
$$

The inner gap has width $a\delta$ and area per unit length approximately $2\pi a$. Its [parallel-plate capacitor](../../../../../parallel-plate-capacitor.md) approximation gives exactly the same leading result; the outer gap contributes only a bounded correction.

For the [extremum](../../../../../maximum-and-minimum.md), set $u=\log\lambda$, $L=\log2$, so $0<u<L$. Then

$$
\frac{C}{2\pi\epsilon_0}=\frac1u+\frac1{L-u},\qquad
\frac{d}{du}\frac{C}{2\pi\epsilon_0}=-\frac1{u^2}+\frac1{(L-u)^2},\qquad
\frac{d^2}{du^2}\frac{C}{2\pi\epsilon_0}=\frac2{u^3}+\frac2{(L-u)^3}>0.
$$

Thus the unique stationary point is $u=L/2$. Strict [convexity](../../../../../convex-function.md) and divergence at both endpoints show it is a global minimum:

$$
\boxed{\lambda=\sqrt2,\qquad C_{\min}=\frac{8\pi\epsilon_0}{\log2}.}
$$

There is no maximum on $1<\lambda<2$.

## ↑ Ancestors (10)

1. [17E](../17e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
