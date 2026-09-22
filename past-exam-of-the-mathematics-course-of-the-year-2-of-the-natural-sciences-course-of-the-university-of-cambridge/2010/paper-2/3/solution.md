<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [outgoing Green function for the three-dimensional Helmholtz equation](../../../../outgoing-green-function-for-the-three-dimensional-helmholtz-equation.md) satisfies

$$
(\Delta_y+\omega^2)G_F(x,y)=-\delta^{(3)}(y-x).
$$

Its normalization follows by integrating over a small ball about $x$: $G_F\sim1/(4\pi|y-x|)$, so its outward derivative has flux $-1$. Apply [Green's second identity](../../../../green-second-identity.md) in the $y$ variables:

$$
\begin{aligned}
\int_{\partial V}(\Psi\nabla_yG_F-G_F\nabla_y\Psi)\cdot n\,dS
&=\int_V(\Psi\Delta_yG_F-G_F\Delta_y\Psi)dV_y\\
&=-\int_V\Psi(y)\delta^{(3)}(y-x)dV_y.
\end{aligned}
$$

The $\omega^2$ terms cancel. Thus the surface integral equals $-\Psi(x)$ for $x\in V$, and zero for $x$ outside the closed volume. Equivalently, remove a small source ball and evaluate its flux before taking its radius to zero. A source on the boundary would require a different limiting formula and is not part of this calculation.

For the upper half-space, take a half-ball of radius $\rho$. Interpret the first far-field condition as $\Psi=O(\rho^{-1})$, and the radiation limit in its usual direction-uniform sense, namely the [Sommerfeld radiation condition](../../../../sommerfeld-radiation-condition.md)

$$
(\partial_\rho-i\omega)\Psi=o(\rho^{-1}).
$$

This is the finite-bound interpretation of the PDF's first condition. For fixed $x$ and real $\omega$,

$$
G_F=O(\rho^{-1}),\qquad(\partial_\rho-i\omega)G_F=O(\rho^{-2}).
$$

Indeed $|y-x|=\rho-\widehat y\cdot x+O(\rho^{-1})$, and its radial derivative is $1+O(\rho^{-2})$. On the large hemisphere the integrand can therefore be rewritten as

$$
\Psi(\partial_\rho-i\omega)G_F-G_F(\partial_\rho-i\omega)\Psi
=O(\rho^{-3})+o(\rho^{-2}).
$$

Its area is $2\pi\rho^2$, so its integral tends to zero. The planar integral, taken over expanding disks if needed, consequently equals $-\Psi(x)$ for $x_3>0$ and zero for $x_3<0$.

The outward [unit normal vector](../../../../unit-normal.md) on the bottom plane is $-e_3$. Denote this planar integral by

$$
I(x)=\int_{\mathbb R^2}\left[-\Psi(y',0)\partial_{y_3}G_F(x,(y',0))+G_F(x,(y',0))\partial_3\Psi(y',0)\right]d^2y'.
$$

For $x_3>0$ reflect the source point to $x^*=(x_1,x_2,-x_3)$. On the plane,

$$
G_F(x^*,y)=G_F(x,y),\qquad \partial_{y_3}G_F(x^*,y)=-\partial_{y_3}G_F(x,y).
$$

Adding $I(x)=-\Psi(x)$ and $I(x^*)=0$ cancels the boundary values of $\Psi$ and gives $2\int G_F\partial_3\Psi=-\Psi(x)$. Thus the [Neumann representation for a radiating Helmholtz half-space](../../../../neumann-representation-for-a-radiating-helmholtz-half-space.md) is

$$
\boxed{\Psi(x)=-\frac1{2\pi}\int_{\mathbb R^2}\partial_3\Psi(y',0)\frac{e^{i\omega\sqrt{|x'-y'|^2+x_3^2}}}{\sqrt{|x'-y'|^2+x_3^2}}\,d^2y',\qquad x_3>0.}
$$

The negative sign is consistent with using the upward derivative $\partial_3\Psi$ rather than the outward [normal derivative](../../../../normal-derivative.md). If that upward derivative is zero everywhere on the plane, the integral is zero. Hence **$\Psi=0$ throughout the upper half-space** in the specified radiating class; taking a difference also gives uniqueness for prescribed [Neumann boundary data](../../../../neumann-boundary-data.md).

## ↑ Ancestors (12)

1. [3](../3.md)
2. [Paper 2](../../paper-2-split.md)
3. [2010](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
