<h1 id="2/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The complete [Butcher tableau](../../../../../../butcher-tableau.md) in the PDF supplies

$$
s=\frac{\sqrt3}{6},\qquad
A=\begin{pmatrix}\frac14&\frac14-s\\\frac14+s&\frac14\end{pmatrix},\quad
b=\frac12\begin{pmatrix}1\\1\end{pmatrix},\quad
c=\begin{pmatrix}\frac12-s\\\frac12+s\end{pmatrix}.
$$

These are the two Gauss nodes and the corresponding [Gauss--Legendre Runge-Kutta method](../../../../../../gauss-legendre-method.md). We can verify its order directly rather than infer it from its name. Write $e=(1,1)^T$, $C=\operatorname{diag}(c)$ and let powers of $c$ be componentwise. The [Butcher order conditions](../../../../../../butcher-order-condition.md) through order four are

$$
\begin{aligned}
b^Te&=1,&b^Tc&=\frac12,\\
b^Tc^2&=\frac13,&b^TAc&=\frac16,\\
b^Tc^3&=\frac14,&b^TCAc&=\frac18,\\
b^TAc^2&=\frac1{12},&b^TA^2c&=\frac1{24}.
\end{aligned}
$$

For these coefficients $Ae=c$, $Ac=c^2/2$ and $c^2=c-e/6$. Also $b^Tc^j=1/(j+1)$ for $j=0,1,2,3$, as follows by averaging the two values $1/2\pm s$. These identities give all eight displayed [Butcher order conditions](../../../../../../butcher-order-condition.md); for example $b^TCAc=b^Tc^3/2=1/8$, $b^TAc^2=b^T(c^2/2-c/6)=1/12$, and $b^TA^2c=b^TAc^2/2=1/24$. They establish order at least four for smooth nonlinear [ordinary differential equations](../../../../../../ordinary-differential-equation.md).

To exclude order five, apply the method to the [Dahlquist test equation](../../../../../../dahlquist-test-equation.md). Solving its stage equations gives the [stability function](../../../../../../stability-function.md)

$$
R(z)=1+zb^T(I-zA)^{-1}e
=\frac{1+z/2+z^2/12}{1-z/2+z^2/12}
=1+z+\frac{z^2}{2}+\frac{z^3}{6}+\frac{z^4}{24}+\frac{z^5}{144}+O(z^6).
$$

The exact solution has coefficient $1/120$ at degree five. Hence **the method has order exactly four**; its one-step defect is $O(h^5)$.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2](../../2.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
