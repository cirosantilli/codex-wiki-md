<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

The [Papperitz symbol](../../../../../papperitz-symbol.md)

$$
P\left\{
\begin{array}{ccccc}
0&1&\infty&&\\
0&0&a&z&\\
1-c&c-a-b&b&&
\end{array}\right\}
$$

specifies a second-order [Fuchsian differential equation](../../../../../fuchsian-differential-equation.md). The first row lists its three distinct regular singular points $0,1,\infty$; $z$ is the independent variable. The two entries below each singular point are its [characteristic exponents](../../../../../characteristic-exponent-at-a-regular-singular-point.md). Thus local solutions have leading behaviors

$$
1,\ z^{1-c}\quad(z\to0),
$$



$$
1,\ (1-z)^{c-a-b}\quad(z\to1),
$$

and, with the usual convention at infinity,

$$
z^{-a},\ z^{-b}\quad(z\to\infty).
$$

When an exponent difference is an integer, a logarithmic second solution may replace the naive second Frobenius power. The entries obey the [Fuchs relation](../../../../../fuchs-relation.md)

$$
0+(1-c)+0+(c-a-b)+a+b=1.
$$

For a second-order equation with exactly three regular singular points, these exponent data determine the equation up to multiplication by a nonzero function; there is no accessory parameter. The symbol is therefore the one for the [Gauss hypergeometric equation](../../../../../gauss-hypergeometric-equation.md). Its distinguished solution $F(a,b;c;z)$ is the exponent-zero solution analytic at zero and normalized to one there. For the ordinary power-series definition one assumes $c\notin\{0,-1,-2,\ldots\}$, with exceptional parameter values handled separately or by continuation.

Now put

$$
u=\frac{z}{z-1},
\qquad
Y(z)=F(a,c-b;c;u).
$$

The hypergeometric equation in $u$ has exponent pairs

$$
(0,1-c)\text{ at }u=0,\qquad
(0,b-a)\text{ at }u=1,\qquad
(a,c-b)\text{ at }u=\infty.
$$

The [Möbius transformation of a Papperitz symbol](../../../../../mobius-transformation-of-a-papperitz-symbol.md) sends

$$
u=0,1,\infty
\quad\longleftarrow\quad
z=0,\infty,1,
$$

so $Y$ has symbol

$$
P\left\{
\begin{array}{ccccc}
0&1&\infty&&\\
0&a&0&z&\\
1-c&c-b&b-a&&
\end{array}\right\}.
$$

On the other hand, $F(a,b;c;z)$ has exponent pairs

$$
(0,1-c),\qquad(0,c-a-b),\qquad(a,b)
$$

at $0,1,\infty$. Multiplication by $(1-z)^a$ applies the [dependent-variable rescaling of a Papperitz symbol](../../../../../dependent-variable-rescaling-of-a-papperitz-symbol.md): it adds $a$ to both exponents at $z=1$ and subtracts $a$ from both at infinity. Hence

$$
(1-z)^aF(a,b;c;z)
$$

has exactly the same three exponent pairs as $Y$.

Both functions are analytic near $z=0$ and equal one at $z=0$, so uniqueness of the normalized exponent-zero hypergeometric solution gives the [Pfaff transformation](../../../../../pfaff-transformation.md)

$$
\boxed{
F\left(a,c-b;c;\frac{z}{z-1}\right)
=(1-z)^aF(a,b;c;z).}
$$

The identity first holds near zero with the branch of $(1-z)^a$ equal to one there, and then extends by [analytic continuation](../../../../../analytic-continuation.md) on any domain where compatible branches are chosen.

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
