<h1 id="14a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Extend the boundary data oddly to the whole real axis. The extended function is precisely the function $f$ from part (a). Taking the [Fourier transform](../../../../../../fourier-transform.md) in $x$, the [Laplace equation](../../../../../../laplace-equation.md) becomes

$$
\partial_y^2\widetilde u-k^2\widetilde u=0.
$$

Decay as $y\to\infty$ selects

$$
\widetilde u(k,y)=\widetilde f(k)e^{-|k|y}.
$$

Part (b), together with the [convolution theorem](../../../../../../convolution-theorem.md), says that the inverse transform is convolution with the [Poisson kernel](../../../../../../poisson-kernel-for-the-upper-half-plane.md)

$$
P_y(s)=\frac{y}{\pi(s^2+y^2)}.
$$

For $x,y>0$ this gives

$$
\begin{aligned}
u(x,y)
&=\frac y\pi\int_0^1\left[
\frac1{(x-v)^2+y^2}-\frac1{(x+v)^2+y^2}
\right]dv\\
&=\boxed{\frac{4xy}{\pi}\int_0^1
\frac{v\,dv}{[(x-v)^2+y^2][(x+v)^2+y^2]}}.
\end{aligned}
$$

The odd extension enforces $u(0,y)=0$, while the [Poisson integral](../../../../../../poisson-integral.md) takes the prescribed boundary values at every continuity point and decays at infinity.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [14A](../../14a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
