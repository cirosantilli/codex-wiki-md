<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The original cubic vertex gives $g$. At order $g^3$, the one-particle-irreducible correction to the cubic interaction is the triangle diagram: one slow external leg leaves each of three cubic vertices, and three high-mode propagators join the vertices cyclically. Diagrams with a high-momentum bridge carrying only a sum of vanishing external momenta do not contribute to the local zero-momentum coupling; external self-energy diagrams belong to the neglected field rescaling.

The relevant interaction at each vertex is $(g/2)\phi\chi^2$. The third connected cumulant contributes

$$
\frac1{3!}\left(\frac g2\right)^3
\int d^dx,d^dy,d^dz\,\phi(x)\phi(y)\phi(z)
\langle\chi(x)^2\chi(y)^2\chi(z)^2\rangle_c.
$$

Wick's theorem gives $8G_>(x-y)G_>(y-z)G_>(z-x)$. Projecting onto a local interaction therefore gives

$$
\boxed{g_{\rm eff}=g+g^3
\int_{b\Lambda<|q|<\Lambda}\frac{d^dq}{(2\pi)^d}\frac1{(q^2)^3}+O(g^5)}.
$$

For $d=6$, the area of the unit five-sphere is $\Omega_5=\pi^3$, and hence

$$
\int_{b\Lambda}^{\Lambda}\frac{\Omega_5q^5,dq}{(2\pi)^6q^6}
=\frac1{64\pi^3}\log\frac1b.
$$

Thus

$$
\boxed{g_{\rm eff}=g-\frac{g^3}{64\pi^3}\log b+O(g^5)},
\qquad
\boxed{C=-\frac1{64\pi^3}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 304](../../../paper-304-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
