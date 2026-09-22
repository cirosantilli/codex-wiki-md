<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $S=\begin{pmatrix}0&-1\\1&0\end{pmatrix}$ and $T=\begin{pmatrix}1&1\\0&1\end{pmatrix}$. The [modular group](../../../../../../modular-group.md) acts on the [complex upper half-plane](../../../../../../upper-half-plane-complex-analysis.md) by fractional linear transformations, and

$$
\operatorname{Im}(\gamma z)=\frac{\operatorname{Im}z}{|cz+d|^2}
\quad\left(\gamma=\begin{pmatrix}a&b\\c&d\end{pmatrix}\right).
$$

For fixed $z=x+iy$, the values $|cz+d|$ with primitive integer pairs $(c,d)$ have a positive minimum: the conditions $|cz+d|\leq R$ bound both $|c|\leq R/y$ and $|d|\leq R+|cx|$, leaving finitely many pairs. By [Bezout identity](../../../../../../bezout-identity.md), a minimizing pair is the bottom row of a matrix in $SL_2(\mathbb Z)$. Applying that matrix gives a point of maximal imaginary part in its orbit.

Translate it by a power of $T$ into $-1/2<x\leq1/2$. It must have modulus at least one, since otherwise $S$ would increase its imaginary part. If it is on the unit circle with negative real part, apply $S$, which there changes $x$ to $-x$. This gives an element of the specified half-open [standard fundamental domain of the modular group](../../../../../../standard-fundamental-domain-of-the-modular-group.md). It proves existence by [reduction to the standard modular region](../../../../../../reduction-to-the-standard-modular-region.md).

For uniqueness, if $z$ lies in the closed standard region then $y\geq\sqrt3/2$ and

$$
|cz+d|\geq1
$$

for every primitive pair. If $c=0$, this follows from $d=\pm1$; if $|c|\geq2$, it follows from $|c|y\geq\sqrt3$. If $|c|=1$, then $d=0$ uses $|z|\geq1$, while $|d|\geq1$ gives

$$
|cz+d|^2=|z|^2+d^2+2cdx\geq1+d^2-|d|\geq1.
$$

If both $z$ and $z'=\gamma z$ lie in the region, applying this inequality to $\gamma$ and $\gamma^{-1}$ forces their imaginary parts to agree, hence $|cz+d|=1$.

The equality cases describe every possible boundary identification. For $c=0$ the map is an integer translation; the half-open vertical strip retains one representative. For $|c|=1,d=0$, equality requires $|z|=1$, and the map is an inversion followed by an integer translation. Inversion exchanges the two halves of the circle, so retaining only the right half removes the duplication; the only translation that returns the exchanged endpoint is the one identifying the two corners. The remaining equality cases have $|c|=|d|=1$, $|z|=1$ and $x=\pm1/2$, and give only those same corner identifications. Our region retains the right corner alone. Therefore $z'=z$, proving

$$
\boxed{\text{every orbit has exactly one representative in }\mathcal D.}
$$

The equality analysis also gives the [elliptic stabilizers of the modular group](../../../../../../elliptic-stabilizers-of-the-modular-group.md). The central matrices $\pm I$ fix every point. The point $i$ is fixed by $S$, with $S^2=-I$, and the retained corner $\rho_+=e^{i\pi/3}$ is fixed by $R=TS$, with $R^3=-I$. There are no other noncentral stabilizers, and the possible bottom rows in the equality cases give exactly

$$
\boxed{\operatorname{Stab}_\Gamma(z)=
\begin{cases}
\langle S\rangle\cong C_4,&z=i,\\
\langle TS\rangle\cong C_6,&z=\rho_+,\\
\{I,-I\},&\text{otherwise}.
\end{cases}}
$$

The corresponding stabilizer orders in $PSL_2(\mathbb Z)$ are two, three and one; the requested group is $SL_2(\mathbb Z)$, so the center must be included.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 137](../../../paper-137-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
