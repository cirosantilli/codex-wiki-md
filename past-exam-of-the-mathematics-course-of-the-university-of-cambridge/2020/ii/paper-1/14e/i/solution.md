<h1 id="14e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $y(x)=w(z)$ with $z=\sin^2x$. The [chain rule](../../../../../../chain-rule.md) gives

$$
\left(\frac{dz}{dx}\right)^2=4z(1-z),
\qquad
\frac{d^2z}{dx^2}=2(1-2z),
$$

and hence

$$
\frac{d^2y}{dx^2}
=4z(1-z)\frac{d^2w}{dz^2}
+2(1-2z)\frac{dw}{dz}.
$$

After substitution and division by $4z(1-z)$, the [ordinary differential equation](../../../../../../ordinary-differential-equation.md) becomes

$$
w''+\left(\frac1{2z}+\frac1{2(z-1)}\right)w'
-\frac{k^2/4}{z(z-1)}w=0.
$$

Comparison with the [Gauss hypergeometric equation](../../../../../../gauss-hypergeometric-equation.md) gives, up to interchanging $A$ and $B$,

$$
\boxed{A=\frac{k}{2},\qquad B=-\frac{k}{2},\qquad C=\frac12}.
$$

At $z=0$ and $z=1$, the coefficient of $w'$ has at most a simple pole and that of $w$ has at most a double pole, so both are [regular singular points](../../../../../../regular-singular-point.md). The [regular singular point at infinity](../../../../../../regular-singular-point-at-infinity.md) criterion gives the same conclusion at infinity. The corresponding [Papperitz symbol](../../../../../../papperitz-symbol.md) is

$$
\boxed{
P\!\left\{
\begin{array}{cccc}
0&1&\infty&z\\
0&0&k/2&\\
1/2&1/2&-k/2&
\end{array}
\right\}.}
$$

Indeed, the exponent pairs are $(0,1-C)=(0,1/2)$ at zero, $(0,C-A-B)=(0,1/2)$ at one, and $(A,B)=(k/2,-k/2)$ at infinity; their sum also satisfies the [Fuchs relation](../../../../../../fuchs-relation.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [14E](../../14e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
