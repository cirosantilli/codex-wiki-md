<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

The [Papperitz symbol](../../../../../papperitz-symbol.md)

$$
P\left\{
\begin{array}{ccc}
z_1&z_2&z_3\\
\alpha_1&\alpha_2&\alpha_3\\
\beta_1&\beta_2&\beta_3
\end{array}
\right\}
$$

describes the two-dimensional solution space of a second-order homogeneous [Fuchsian differential equation](../../../../../fuchsian-differential-equation.md) on the Riemann sphere with exactly three [regular singular points](../../../../../regular-singular-point-criterion-for-a-second-order-equation.md) $z_1,z_2,z_3$. Near $z_i$, its two independent Frobenius behaviours are locally

$$
(z-z_i)^{\alpha_i}
\quad\text{and}\quad
(z-z_i)^{\beta_i},
$$

subject to logarithmic modifications in resonant cases. The six [characteristic exponents](../../../../../characteristic-exponent-at-a-regular-singular-point.md) obey the [Fuchs relation](../../../../../fuchs-relation.md)

$$
\sum_{i=1}^3(\alpha_i+\beta_i)=1.
$$

For the [Gauss hypergeometric equation](../../../../../gauss-hypergeometric-equation.md), the exponents at infinity are $a$ and $b$. Put $w=z^{-1}$. Transforming the Papperitz symbol from $z$ to $w$ shows that

$$
y_a(z)
=z^{-a}F(a,1+a-c;1+a-b;z^{-1})
$$

and

$$
y_b(z)
=z^{-b}F(b,1+b-c;1+b-a;z^{-1})
$$

are local solutions near $z=\infty$, with respective leading behaviours $z^{-a}$ and $z^{-b}$. When $a-b\notin\mathbb Z$, these behaviours are distinct and the two solutions are linearly independent. They therefore form a basis of the solution space on any simply connected common domain with compatible branch choices.

The solution $F(a,b;c;z)$ normalized at zero can be analytically continued into that domain. Since it solves the same second-order equation, it must be a constant linear combination of the basis at infinity:

$$
\boxed{
F(a,b;c;z)
=Az^{-a}F(a,1+a-c;1+a-b;z^{-1})
+Bz^{-b}F(b,1+b-c;1+b-a;z^{-1})
}.
$$

The constants depend on $a,b,c$ and the branch convention, but not on $z$. This is the [hypergeometric connection formula at infinity](../../../../../hypergeometric-connection-formula-at-infinity.md).

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
