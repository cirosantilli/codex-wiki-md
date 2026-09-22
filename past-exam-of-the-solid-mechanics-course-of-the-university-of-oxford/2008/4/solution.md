<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

On each half-space the [deformation](../../../deformation-mechanics.md) is affine. Continuity on the separating [plane](../../../plane.md) makes the two affine constants equal and gives $(A-B)t=0$ for every [tangent vector](../../../tangent-vector-split.md) $t\perp N$. Decomposing any $x$ into its tangential part and $(x\cdot N)N$ gives

$$
(A-B)x=[(A-B)N](N\cdot x),\qquad\boxed{A-B=a\otimes N,\quad a=(A-B)N.}
$$

This is the [Hadamard jump condition](../../../hadamard-jump-condition.md). Since $B=A-a\otimes N=A(I-A^{-1}a\otimes N)$, the [matrix determinant lemma](../../../matrix-determinant-lemma.md) gives

$$
\det B=\det A(1-N\cdot A^{-1}a).
$$

Both [determinants](../../../determinant.md) are positive, hence $\boxed{A^{-1}a\cdot N<1}$.

Write $a_1=\eta_1$, $a_2=\eta_2$, $S=a_1^2+a_2^2$ and $\Delta=a_2^2-a_1^2\ne0$. The two proposed angles have $c=2a_1a_2/S$ and $s=\kappa\Delta/S$, and $c^2+s^2=1$. Therefore the displayed [rotations](../../../rotation-mathematics.md) lie in $SO(3)$. Direct multiplication gives

$$
RU_2-U_1=\frac\Delta S\begin{pmatrix}-a_2&-\kappa a_2&0\\\kappa a_1&a_1&0\\0&0&0\end{pmatrix}
=\boxed{\frac\Delta S(-a_2,\kappa a_1,0)\otimes(1,\kappa,0).}
$$

This is a [rank-one connection](../../../rank-one-connection.md) for each sign. With a unit normal one may choose $N=(1,\kappa,0)/\sqrt2$ and jump vector $a=\sqrt2\Delta(-a_2,\kappa a_1,0)/S$. The two [rotations](../../../rotation-mathematics.md) are distinct because $\Delta\ne0$; the permitted at-most-two result therefore proves these are all solutions. Flipping both $a$ and $N$ changes no connection.

It remains to test the material [plane](../../../plane.md). Because $y(0)=0$, the affine constants vanish. Let $t=(-p_2,p_1,0)$, so the [plane](../../../plane.md) is spanned by $t$ and $e_3$. Both [deformation gradients](../../../deformation-gradient.md) send $e_3$ to $a_1e_3$. If the [plane](../../../plane.md) is not the [twin plane](../../../twin-plane.md), it cuts the two half-spaces; its two image halves are coplanar exactly when the in-[plane](../../../plane.md) vectors $Bt$ and $At$ are [parallel](../../../linear-dependence.md). Put $d=(-a_2,\kappa a_1)$ and $n=(1,\kappa)$ in their two-dimensional sections. Then

$$
\begin{aligned}
\det_2(Bt,At)
&=\frac\Delta S\det_2(Bt,d)(n\cdot t)\\
&=\boxed{\frac{\kappa a_1a_2\Delta}{S}(p_1-\kappa p_2)^2}.
\end{aligned}
$$

Its prefactor is nonzero, so [coplanarity](../../../coplanarity.md) requires $p_1=\kappa p_2$, precisely $p\parallel(1,\kappa,0)\parallel N$. Conversely, on that [twin plane](../../../twin-plane.md) $(A-B)x=0$, so the two [affine maps](../../../affine-map.md) agree and its image is a [plane](../../../plane.md). Thus $\boxed{\Pi\text{ remains plane}\iff p\parallel N}$. All other allowed [planes](../../../plane.md) acquire a kink along their intersection with the twin. This is the [planarity test across a cubic-to-tetragonal twin](../../../planarity-test-across-a-cubic-to-tetragonal-twin.md).

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2008](../../2008-split.md)
3. [Past exam of the solid mechanics course of the University of Oxford](../../split.md)
4. [Solid mechanics course of the University of Oxford](../../../solid-mechanics-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
