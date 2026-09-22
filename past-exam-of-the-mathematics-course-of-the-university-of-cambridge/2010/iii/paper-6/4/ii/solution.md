<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume the finite-generator identity holds whenever there is no common zero. Let $\varphi\in\Phi_A$. For every finite family $f_1,\ldots,f_n\in\ker\varphi$, their zero sets must have nonempty intersection: otherwise an identity $\sum f_jg_j=1$ would give $0=\varphi(1)=1$. These zero sets are closed in compact $K$. The [finite intersection property](../../../../../../finite-intersection-property.md) therefore supplies $x\in K$ at which every member of $\ker\varphi$ vanishes. For any $f\in A$, the element $f-\varphi(f)1$ is in that kernel, so $f(x)=\varphi(f)$. Thus $\varphi=\delta_x$, proving

$$
\boxed{\text{the finite-generator identity holds}\iff A\text{ is natural}.}
$$

For $C(K)$, the identity is explicit. If the $f_j$ have no common zero, the continuous function $q=\sum_j|f_j|^2$ is strictly positive on compact $K$. Set

$$
g_j=\frac{\overline{f_j}}{q}\in C(K).
$$

Then $\sum f_jg_j=1$. The equivalence just proved shows that **$C(K)$ is natural**.

Next consider the [disc algebra](../../../../../../disk-algebra.md) $A(\overline{\mathbb D})$, the continuous functions on the closed unit disk that are holomorphic in its interior. We show directly that each [algebra character](../../../../../../character-of-an-algebra.md) is evaluation. Polynomials are uniformly dense in this algebra: for $0<r<1$, $f_r(z)=f(rz)$ tends uniformly to $f$ as $r\uparrow1$, by [uniform continuity](../../../../../../uniform-continuity.md). The function $f_r$ is holomorphic on $|z|<1/r$, so its Taylor polynomials converge uniformly on $|z|\leq1$.

Every [algebra character](../../../../../../character-of-an-algebra.md) of a unital [Banach algebra](../../../../../../banach-algebra-split.md) is bounded, with $|\varphi(f)|\leq\|f\|$: if $f-\varphi(f)1$ were invertible, applying $\varphi$ would contradict invertibility, so $\varphi(f)$ belongs to the [spectrum of an element](../../../../../../spectrum-of-an-element.md), which is contained in the disk of radius $\|f\|$ by the [Neumann series](../../../../../../neumann-series.md). For the coordinate function $z$, put $\lambda=\varphi(z)$; then $|\lambda|\leq1$. Multiplicativity gives $\varphi(p)=p(\lambda)$ for every polynomial. By polynomial density and continuity, $\varphi(f)=f(\lambda)$ for every member of the [disc algebra](../../../../../../disk-algebra.md). Hence

$$
\boxed{\Phi_{A(\overline{\mathbb D})}\cong\overline{\mathbb D},\qquad A(\overline{\mathbb D})\text{ is natural}.}
$$

Finally consider the algebra $C$ in the last request. For each $f\in C$, its holomorphic extension $g$ from the boundary is unique by the [maximum modulus principle](../../../../../../maximum-modulus-principle.md). Define $T(f)=g\in A(\overline{\mathbb D})$. This is a surjective unital algebra homomorphism, since it restricts to the identity on the [disc algebra](../../../../../../disk-algebra.md). Also

$$
\|T(f)\|_\infty=\sup_{|z|=1}|f(z)|\leq\|f\|_\infty.
$$

The algebra $C$ is closed: if $f_n\to f$ uniformly, the associated $T(f_n)$ are uniformly Cauchy by this bound, so their limit belongs to the closed [disc algebra](../../../../../../disk-algebra.md) and agrees with $f$ on the boundary. Constants and the coordinate function belong to $C$, so it is itself a [uniform algebra](../../../../../../uniform-algebra.md) on the disk. Its [ideal](../../../../../../ideal.md)

$$
I=\ker T=\{f\in C(\overline{\mathbb D}):f|_{\partial\mathbb D}=0\}
$$

is contained in $C$, and $C/I$ is the [disc algebra](../../../../../../disk-algebra.md).

If a [algebra character](../../../../../../character-of-an-algebra.md) $\chi$ on $C$ vanishes on $I$, it factors through $T$ and the preceding result gives

$$
\chi(f)=T(f)(\lambda)\quad\hbox{for some }\lambda\in\overline{\mathbb D}.
$$

If $\chi$ does not vanish on $I$, choose $h\in I$ with $\chi(h)\ne0$. For $F\in C(\overline{\mathbb D})$, define

$$
\widetilde\chi(F)=\frac{\chi(hF)}{\chi(h)}.
$$

The product $hF$ is in $I$, so this is well defined. It is unital and linear, and

$$
\chi(hF)\chi(hG)=\chi(h^2FG)=\chi(h)\chi(hFG)
$$

shows multiplicativity. Since $C(\overline{\mathbb D})$ is natural, $\widetilde\chi$ is evaluation at a point $x$ of the closed disk. The equality $h(x)=\widetilde\chi(h)=\chi(h)\ne0$ places $x$ in the open disk. On $C$, $\widetilde\chi(f)=\chi(f)$, so $\chi$ itself is evaluation at that interior point.

We therefore obtain two families: actual evaluations $f\mapsto f(x)$ on one closed disk, and analytic-extension evaluations $f\mapsto T(f)(\lambda)$ on a second closed disk. They agree on the boundary. They are distinct at interior points: functions in $I$ distinguish actual interior evaluations from every analytic-extension evaluation, and the coordinate function distinguishes points within each family. Thus

$$
\boxed{\Phi_C\cong\overline{\mathbb D}\ \cup_{\partial\mathbb D}\ \overline{\mathbb D}\cong S^2.}
$$

This is also a topological identification. Each disk family is continuous in the [Gelfand topology](../../../../../../gelfand-topology.md), and they agree along their boundary, giving a continuous [bijection](../../../../../../bijection.md) from the glued disks to $\Phi_C$. The glued disks form a compact space, explicitly homeomorphic to the sphere by sending $(x,y)$ in the two copies to $(x,y,\pm\sqrt{1-x^2-y^2})$. Since the [character space](../../../../../../character-space-of-an-algebra.md) is Hausdorff, the continuous [bijection](../../../../../../bijection.md) is a [homeomorphism](../../../../../../homeomorphism.md). This [boundary-analytic disk algebra with doubled character space](../../../../../../boundary-analytic-disk-algebra-with-doubled-character-space.md) has more [algebra characters](../../../../../../character-of-an-algebra.md) than evaluations on its original disk.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
