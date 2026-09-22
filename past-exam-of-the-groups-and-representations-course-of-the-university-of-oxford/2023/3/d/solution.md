<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $D(z)=\operatorname{diag}(z^{-2}I_3,z^3I_2)$ and partition a [matrix](../../../../matrix.md) $X$ into $3+2$ blocks. The equation $XD(z)=D(z)X$ makes its off-diagonal blocks obey $(z^3-z^{-2})X_{12}=0$ and $(z^{-2}-z^3)X_{21}=0$ for every $z\in U(1)$. Choosing any $z$ with $z^5\ne1$ forces both blocks to vanish. Conversely, every block diagonal [matrix](../../../../matrix.md) commutes with every $D(z)$. Intersecting with the [special unitary group](../../../../special-unitary-group.md) gives the exact [centralizer](../../../../centralizer.md)

$$
\boxed{C_{SU(5)}(U(1))=S(U(3)\times U(2))
=\{\operatorname{diag}(A,B):A\in U(3),\ B\in U(2),\ \det A\det B=1\}.}
$$

Its [Lie algebra](../../../../lie-algebra-split.md) is $\mathfrak{su}(3)\oplus\mathfrak{su}(2)\oplus\mathfrak u(1)$. At the [group](../../../../group-split.md) level there is a finite central identification. The surjective [group homomorphism](../../../../group-homomorphism.md)

$$
F:SU(3)\times SU(2)\times U(1)\longrightarrow S(U(3)\times U(2)),\qquad
F(A,B,z)=\operatorname{diag}(z^{-2}A,z^3B)
$$

has [kernel](../../../../kernel-of-a-linear-map-split.md) $\{(z^2I_3,z^{-3}I_2,z):z^6=1\}\cong\mathbb Z_6$. Surjectivity follows by choosing $z$ with $z^{-6}=\det A'$ for any target pair $(A',B')$, and setting $A=z^2A'$, $B=z^{-3}B'$. Thus

$$
\boxed{C_{SU(5)}(U(1))\cong
\bigl(SU(3)\times SU(2)\times U(1)\bigr)/\mathbb Z_6.}
$$

The six distinct [kernel](../../../../kernel-of-a-linear-map-split.md) elements give a concrete reason the displayed map does not identify the [centralizer](../../../../centralizer.md) with an unquotiented product.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../e/solution.md)
