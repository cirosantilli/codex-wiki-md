<h1 id="14f/solution">Solution</h1>

↑ **Parent:** [14F](../14f.md)

First obtain the [hyperbolic circle in the upper half-plane](../../../../../hyperbolic-circle-in-the-upper-half-plane.md). For centre $w=u+iv$, the fractional-linear map $\zeta=(z-w)/(z-\overline w)$ takes the [Poincaré half-plane model](../../../../../poincare-half-plane-model.md) isometrically to the [Poincare disc model](../../../../../poincare-disk-model.md), sending $w$ to zero. Direct differentiation transforms the metric to $4|d\zeta|^2/(1-|\zeta|^2)^2$. A radial segment from zero to modulus $\rho$ has length $2\operatorname{artanh}\rho$. Any path to that modulus has at least this length, by $|d\zeta|\ge|d\rho|$; thus it is the [hyperbolic distance](../../../../../hyperbolic-distance.md).

A circle of hyperbolic radius $R$ therefore satisfies

$$
\left|\frac{z-w}{z-\overline w}\right|=\tanh(R/2).
$$

Squaring and rearranging gives

$$
\boxed{(x-u)^2+(y-v\cosh R)^2=v^2\sinh^2R.}
$$

Hence it is a [circle](../../../../../circle.md) in [Euclidean geometry](../../../../../euclidean-geometry.md), with Euclidean centre $u+iv\cosh R$ and radius $v\sinh R$. Its lowest point has height $ve^{-R}>0$, so it stays entirely in the upper half-plane. **The centres differ whenever $R>0$**: for example, the hyperbolic circle centred at $i$ has Euclidean centre $i\cosh R$, rather than $i$.

For [hyperbolic side-side-side congruence](../../../../../hyperbolic-side-side-side-congruence.md), use the standard fact that hyperbolic isometries act transitively on ordered point pairs with the same positive separation, and that reflection in a hyperbolic line is an isometry. Map $A,B$ to $A',B'$. The image of $C$ has prescribed distances $b$ from $A'$ and $a$ from $B'$, just as $C'$ does. There are at most two such points, interchanged by reflection in the line $A'B'$.

For completeness, normalize $A',B'$ to points on the positive imaginary axis. Their distance circles are Euclidean circles with centres on that axis by the formula above. Subtracting their equations determines one height $y$, and then the abscissa is determined up to its sign. Reflection $z\mapsto-\overline z$ interchanges these choices. Therefore either the chosen isometry or its composition with that reflection maps all three labelled vertices correctly. **Equal three side lengths imply a hyperbolic isometry between the triangles.**

**Two sides and an unspecified equal angle do not suffice.** Here is an explicit [hyperbolic side-side-angle ambiguity](../../../../../hyperbolic-side-side-angle-ambiguity.md). Fix the angle at $A$ to be $\pi/6$, let $\cosh a=3/2$ and $\cosh b=2$, and choose

$$
c_-=\ln(3-\sqrt2),\qquad c_+=\ln(3+\sqrt2).
$$

Both are positive and distinct. The [hyperbolic cosine rule](../../../../../hyperbolic-law-of-cosines.md) at $A$ becomes

$$
\cosh a=\cosh b\cosh c-\sinh b\sinh c\cos A
=2\cosh c-\frac32\sinh c.
$$

Setting $u=e^c$, the condition is $u^2-6u+7=0$, whose two roots are $3\pm\sqrt2$. Construct each triangle from sides $b,c_\pm$ meeting at angle $\pi/6$; its opposite side is the same $a$ by the cosine rule. The triangles therefore share $a,b,A$ but have different third sides and cannot be isometric. If the common angle is specifically the included angle between the two given sides, the cosine rule determines the third side and side-side-side congruence does apply.

## ↑ Ancestors (10)

1. [14F](../14f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
