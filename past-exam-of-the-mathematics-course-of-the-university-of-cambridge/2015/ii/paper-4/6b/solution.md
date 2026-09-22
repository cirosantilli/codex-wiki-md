<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

The [Papperitz symbol](../../../../../papperitz-symbol.md) describes a homogeneous second-order [Fuchsian differential equation](../../../../../fuchsian-differential-equation.md) on the [Riemann sphere](../../../../../riemann-sphere.md), with three [regular singular points](../../../../../regular-singular-point.md) and the two [indicial exponents](../../../../../indicial-exponent.md) at each. At a finite point $z_j$, an exponent $r$ corresponds locally to a factor $(z-z_j)^r$; at infinity it corresponds to $z^{-r}$. Repeated or resonant exponents can require logarithms. The six exponents obey the [Fuchs relation](../../../../../fuchs-relation.md) that their sum is one. With three singularities there is no independent [accessory parameter](../../../../../accessory-parameter.md), so these data determine the normalized equation.

A [Möbius transformation of a Papperitz symbol](../../../../../mobius-transformation-of-a-papperitz-symbol.md) moves the singular points without changing their exponents. Multiplication of the dependent variable by a local power shifts the two exponents by that power, using the reciprocal local coordinate at infinity.

Set $w=z/(z-1)$ and $v(w)=F(a,c-b,c;w)$. At $w=0,1,\infty$, the exponent pairs for $v$ are respectively $(0,1-c)$, $(0,b-a)$, and $(a,c-b)$. The [Möbius transformation](../../../../../mobius-transformation.md) sends $z=0,1,\infty$ to $w=0,\infty,1$. Before rescaling, $v(w(z))$ therefore has exponent pairs $(0,1-c)$ at zero, $(a,c-b)$ at one, and $(0,b-a)$ at infinity. Multiplication by $(1-z)^{-a}$ subtracts $a$ at one and adds $a$ at infinity. The resulting pairs are

$$
(0,1-c),\quad(0,c-a-b),\quad(a,b),
$$

exactly those of the original [Gauss hypergeometric equation](../../../../../gauss-hypergeometric-equation.md). Near zero choose the branch with $(1-z)^{-a}=1$ at zero. The resulting solution is analytic there and has value one. Uniqueness of the normalized analytic solution yields

$$
\boxed{F(a,b,c;z)=(1-z)^{-a}F(a,c-b,c;z/(z-1)).}
$$

This is the [Pfaff transformation](../../../../../pfaff-transformation.md). The normalization presupposes the usual admissible parameters, in particular $c\notin\{0,-1,-2,\ldots\}$. Elsewhere the identity holds by [analytic continuation](../../../../../analytic-continuation.md) with compatible branches, or by parameter limits wherever those are defined.

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
