<h1 id="3c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\mathbf E=E\widehat{\mathbf x}$ and $\mathbf B=B\widehat{\mathbf y}$, and choose $\widehat{\mathbf z}=\widehat{\mathbf x}\times\widehat{\mathbf y}$. Part (a) gives $y=0$. With the origin at $\mathbf x_0$, the remaining Cartesian components are

$$
\ddot x=\frac{qE}{m}-\omega\dot z,
\qquad
\ddot z=\omega\dot x,
\qquad
\omega=\frac{qB}{m}.
$$

The initial conditions are $x=z=\dot x=\dot z=0$. Integrating the second equation gives $\dot z=\omega x$, so

$$
\ddot x+\omega^2x=\frac{qE}{m}.
$$

Solving this [forced harmonic oscillator](../../../../../../forced-harmonic-oscillator.md) and then integrating $\dot z=\omega x$ yields

$$
\boxed{
\begin{aligned}
x(t)&=\frac{mE}{qB^2}\bigl(1-\cos\omega t\bigr),\\
y(t)&=0,\\
z(t)&=\frac EB\left(t-\frac{\sin\omega t}{\omega}\right).
\end{aligned}}
$$

**Thus the position vector is $\mathbf x_0+x(t)\widehat{\mathbf x}+z(t)\widehat{\mathbf z}$. The oscillation occurs at the signed [cyclotron frequency](../../../../../../cyclotron-frequency.md), superposed on the usual [E-cross-B drift](../../../../../../e-cross-b-drift.md).**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3C](../../3c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
