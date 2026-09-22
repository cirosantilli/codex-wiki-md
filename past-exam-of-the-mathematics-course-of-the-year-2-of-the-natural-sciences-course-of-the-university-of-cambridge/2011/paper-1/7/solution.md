<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

The [Cauchy-Riemann equations](../../../../cauchy-riemann-equations.md) are $u_x=v_y$ and $u_y=-v_x$. A [holomorphic function](../../../../holomorphic-function-split.md) is smooth, so equality of mixed [partial derivatives](../../../../partial-derivative.md) gives

$$
\boxed{\Delta u=(v_y)_x-(v_x)_y=0,\qquad\Delta v=-(u_y)_x+(u_x)_y=0.}
$$

Thus its real and imaginary parts are [harmonic functions](../../../../harmonic-function.md).

An [entire function](../../../../entire-function.md) is holomorphic at every finite point of the complex plane. The globally convergent [power series](../../../../power-series.md) for the exponential implies that $e^z$ and $e^{-z}$ are entire. Their difference therefore gives

$$
\sinh z=\frac{e^z-e^{-z}}2,\qquad (\sinh z)'=\cosh z
$$

at every complex $z$, proving that the [hyperbolic sine](../../../../hyperbolic-sine.md) is entire. For powers, the base case $f_1(z)=z$ has derivative one everywhere. If $z^n$ is entire with derivative $nz^{n-1}$, the [product rule](../../../../product-rule.md) gives $(z^{n+1})'=z^n+z\,nz^{n-1}=(n+1)z^n$ everywhere. Induction proves that every positive integer power is entire.

A function has a [pole](../../../../pole.md) of order $n$ at $z_0$ when it is holomorphic in a punctured neighbourhood and $g(z)=(z-z_0)^nf(z)$ extends holomorphically to $z_0$ with $g(z_0)\ne0$. An isolated [essential singularity](../../../../essential-singularity.md) is neither a removable singularity nor a pole; equivalently its [Laurent series](../../../../laurent-series.md) has infinitely many nonzero negative-power terms. In particular

$$
e^{1/z}=\sum_{m=0}^\infty\frac{z^{-m}}{m!},\qquad 0<|z|<\infty,
$$

has an essential singularity at zero.

For $f_N$, the [Laurent series](../../../../laurent-series.md) about infinity is

$$
\boxed{f_N(z)=\sum_{m=0}^\infty\frac{z^{N-m}}{m!}=z^N+z^{N-1}+\frac{z^{N-2}}{2!}+\cdots+\frac1{N!}+\frac{z^{-1}}{(N+1)!}+\cdots.}
$$

To classify the point correctly, use $w=1/z$. Then $f_N(1/w)=w^{-N}e^w$, and $e^w$ is holomorphic with value one at zero. Therefore

$$
\boxed{f_N\text{ has a pole of order }N\text{ at infinity}.}
$$

The [pole at infinity](../../../../pole-at-infinity.md) is compatible with an essential singularity at the finite point zero. Negative powers of $z$ are regular powers of the local coordinate $w$ near infinity, so they do not make that point essential.

## ↑ Ancestors (12)

1. [7](../7.md)
2. [Paper 1](../../paper-1-split.md)
3. [2011](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
