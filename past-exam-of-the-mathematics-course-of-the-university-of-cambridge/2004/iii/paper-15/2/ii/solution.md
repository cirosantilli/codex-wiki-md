<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Weierstrass elliptic function](../../../../../../weierstrass-elliptic-function.md) and its derivative give the map

$$
\boxed{z\longmapsto[\wp(z):\wp'(z):1],\qquad O\longmapsto[0:1:0],}
$$

onto the [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md) $Y^2Z=4X^3-g_2XZ^2-g_3Z^3$. Near zero, multiplying these coordinates by $z^3$ gives $[z+O(z^5):-2+O(z^4):z^3]$, so the map extends holomorphically and is an immersion at the origin.

The meromorphic map $\wp:E\to\mathbb P^1$ has degree two, since its only pole on the torus has order two. Its evenness implies $\wp(u)=\wp(v)$ exactly when $u\equiv v$ or $u\equiv-v$. Oddness of $\wp'$ distinguishes these two alternatives unless they are the same point class. At each nonzero half-period, $\wp'=0$. These three points exhaust its zeros, since its only pole has order three. The three half-period values are distinct: equality of two of them would give two distinct zeros each of order at least two for $\wp-e$, contradicting its total pole order two. They are roots of $4X^3-g_2X-g_3$, so the polynomial has distinct roots and the cubic is smooth. At a half-period $h$ with value $e$, $\wp''(h)=2\prod_{e'\ne e}(e-e')\ne0$. Elsewhere $\wp'$ is nonzero. The coordinate pair therefore has nonzero derivative at every finite point, and the map is injective. Compactness and the smooth cubic equation then identify it as an embedding onto the cubic.

The hyperplane section at infinity has divisor $3[O]$. Thus the intersection divisor $D_\ell$ of any line with this cubic is linearly equivalent to $3[O]$. Applying the [principality criterion on a complex elliptic curve](../../../../../../principality-criterion-on-a-complex-elliptic-curve.md) to $D_\ell-3[O]$ shows that its three points, **counted with intersection multiplicity**, have sum zero in $E$.

Conversely, if the degree-three divisor $D=[u]+[v]+[w]$ has point sum zero, Question 1 gives a meromorphic function with divisor $D-3[O]$. A meromorphic function with no poles away from $O$ and pole order at most three lies in

$$
L(3[O])=\operatorname{span}_{\mathbb C}\{1,\wp,\wp'\}.
$$

To prove this description, subtract multiples of $\wp'$ and $\wp$ to cancel the cubic and quadratic Laurent principal parts. The remaining possible simple-pole coefficient is a residue, which must be zero because it is the only pole on a compact torus. The remaining holomorphic elliptic function is constant. Thus the constructed function is a linear form in the projective coordinates, and its line has intersection divisor exactly $D$. This proves **the chord-and-tangent collinearity criterion is $u+v+w=0$ in $E$**, with multiplicities understood.

For three pairwise distinct point classes away from $O$, ordinary collinearity is equivalent to linear dependence of the coordinate columns, so

$$
\boxed{\det\begin{pmatrix}1&1&1\\\wp(u)&\wp(v)&\wp(w)\\\wp'(u)&\wp'(v)&\wp'(w)\end{pmatrix}=0
\iff u+v+w\in\Lambda.}
$$

The original PDF has this three-column determinant; the TeX's extra copied column is a transcription defect.

There is also a genuine implicit distinctness condition in the printed determinant assertion. If $u=v=\omega_1/10$ and $w=\omega_1/5$, all entries are finite and the determinant is zero because two columns coincide, but $u+v+w=2\omega_1/5\notin\Lambda$. Thus the unrestricted literal equivalence is false. To specify repeated intersections, use the [confluent elliptic collinearity determinant](../../../../../../confluent-elliptic-collinearity-determinant.md): for a double point at $u$ replace the second column by $c'(u)$, where $c(z)=(1,\wp(z),\wp'(z))^t$; for a triple point use $c(u),c'(u),c''(u)$. These impose tangency or inflection, and recover the correct conditions $2u+w\in\Lambda$ or $3u\in\Lambda$. If a point is $O$, use the homogeneous coordinates or a local homogeneous lift, since the displayed affine entries have poles there.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
