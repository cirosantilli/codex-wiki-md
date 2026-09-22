<h1 id="16b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [Möbius transformation](../../../../../../mobius-transformation.md)

$$
w=T(z)=\frac{1+z}{1-z},\qquad z=\frac{w-1}{w+1}.
$$

The lens's boundary intersections are $z=\pm1$. Write $w=u+iv$. Substitution in the inverse gives $\operatorname{Im}z=2v/|w+1|^2$, and

$$
|z+i|^2<2\quad\Longleftrightarrow\quad |(1+i)w+i-1|^2<2|w+1|^2\quad\Longleftrightarrow\quad v<u.
$$

Consequently the two domain inequalities are exactly $0<v<u$, or $0<\arg w<\pi/4$. This algebra proves that $T$ maps the lens bijectively onto the quarter-sector, not merely that its boundary curves go to rays.

The map $w\mapsto w^4$ maps this sector bijectively onto the upper half-plane: the argument increases from $(0,\pi/4)$ to $(0,\pi)$, and the positive modulus map is bijective. Its inverse is the fourth-root branch with argument in $(0,\pi/4)$. Therefore the [quarter-sector mapping of a circular lens](../../../../../../quarter-sector-mapping-of-a-circular-lens.md) is

$$
\boxed{F(z)=\left(\frac{1+z}{1-z}\right)^4:D\cap H\longrightarrow H}.
$$

Its derivative is nonzero in the lens, since $T'(z)=2/(1-z)^2$ and $T(z)\ne0$ there. Finally the Cayley transform $\zeta\mapsto(\zeta-i)/(\zeta+i)$ maps $H$ bijectively to the unit disc, because $|\zeta-i|<|\zeta+i|$ exactly when $\operatorname{Im}\zeta>0$. A required conformal bijection is thus

$$
\boxed{G(z)=\frac{\left(\dfrac{1+z}{1-z}\right)^4-i}{\left(\dfrac{1+z}{1-z}\right)^4+i}}.
$$

All poles and branching endpoints of the construction lie outside the open domain.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [16B](../../16b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
