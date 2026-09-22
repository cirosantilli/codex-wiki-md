<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

For a conservative system near a stable equilibrium, the quadratic [Lagrangian](../../../../lagrangian.md) has the form $L=\frac12\dot q^TM\dot q-\frac12q^TKq$, with symmetric [mass matrix](../../../../mass-matrix.md) $M$ and [stiffness matrix](../../../../stiffness-matrix.md) $K$. A [normal mode](../../../../normal-mode.md) $q=v e^{i\omega t}$ satisfies the [generalized eigenvalue problem for small oscillations](../../../../generalized-eigenvalue-problem-for-small-oscillations.md) $(K-\omega^2M)v=0$, so the frequency equation is $\det(K-\omega^2M)=0$.

To quadratic order, vertical [velocities](../../../../velocity.md) contribute only fourth-order corrections to the [kinetic energy](../../../../kinetic-energy.md), leaving $T=(\dot x^2+\dot y^2+\dot z^2)/2$. A string of length $\ell$ with small horizontal difference $d$ shortens its vertical projection by $d^2/(2\ell)$. The upper segment carries all three masses, the middle segment two, and the lower segment one. Hence their increases in [gravitational potential energy](../../../../gravitational-energy.md) sum to

$$
V=3g\frac{x^2}{2(3a)}+2g\frac{(y-x)^2}{2(2b)}+g\frac{(z-y)^2}{2c}=\frac g2\left[\frac{x^2}{a}+\frac{(x-y)^2}{b}+\frac{(y-z)^2}{c}\right].
$$

Subtracting $V$ from $T$ gives the stated approximate [Lagrangian](../../../../lagrangian.md). Here $M=I$ and

$$
K=g\begin{pmatrix}a^{-1}+b^{-1}&-b^{-1}&0\\-b^{-1}&b^{-1}+c^{-1}&-c^{-1}\\0&-c^{-1}&c^{-1}\end{pmatrix}.
$$

For a mode with middle displacement zero, write $v=(X,0,Z)^T$. The middle row requires $X/b+Z/c=0$, so $Z=-cX/b$. A nonzero mode then has $X,Z\ne0$, and the outer rows require $\omega^2/g=a^{-1}+b^{-1}=c^{-1}$. Therefore the necessary and sufficient condition is

$$
\boxed{\frac1a+\frac1b-\frac1c=0.}
$$

When it holds, the [mode shape](../../../../mode-shape.md) is $(1,0,-c/b)$ with $\omega=\sqrt{g/c}$. This is the force-cancellation mechanism of the [stationary middle mass in a three-mass spring chain](../../../../stationary-middle-mass-in-a-three-mass-spring-chain.md), applied to the equivalent quadratic stiffnesses here.

## ↑ Ancestors (12)

1. [7](../7.md)
2. [Paper 2](../../paper-2-split.md)
3. [2007](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
