<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The closed [standard fundamental domain of the modular group](../../../../../standard-fundamental-domain-of-the-modular-group.md) is

$$
\boxed{\mathcal F=\{z=x+iy\in\mathbb H:|x|\leq\tfrac12,\ |z|\geq1\}.}
$$

Its vertical sides are paired by $T:z\mapsto z+1$, and its circular sides by $S:z\mapsto-1/z$. It is a fundamental region with boundary identifications. To obtain exactly one representative of each orbit, use $-1/2<x\leq1/2$ and, on $|z|=1$, retain the half with $x\geq0$. We will include both vertices when discussing the closure.

To prove existence of a representative, fix $z\in\mathbb H$. Among primitive integer pairs $(c,d)$ choose one minimizing $|cz+d|$. The minimum exists: below any fixed bound, $|c|y\leq|cz+d|$ bounds $c$, and then the real part bounds $d$, so only finitely many pairs occur. Extend this primitive pair to the bottom row of a determinant-one integer [matrix](../../../../../matrix.md) $\gamma$. Since

$$
\operatorname{Im}(\gamma z)=\frac{y}{|cz+d|^2},
$$

this makes the imaginary part maximal over the orbit. Translate by an integer to put the real part in $[-1/2,1/2]$. If the resulting point had modulus below one, inversion by $S$ would increase its imaginary part, a contradiction. Thus every orbit meets $\mathcal F$.

For uniqueness in the interior, note that $y\geq\sqrt3/2$ throughout $\mathcal F$ and that $|cz+d|\geq1$ for every primitive pair. If $|c|\geq2$, then $|cz+d|\geq|c|y\geq\sqrt3>1$. For $|c|=1$, the minimum over integer $d$ is attained at $d=0$ or, at an endpoint, at a neighboring integer: $|z|\geq1$ and $|z\pm1|^2=|z|^2\pm2x+1\geq1$. All larger $|d|$ give a strict inequality. If $c=0$, primitivity gives $d=\pm1$.

If two points in $\mathcal F$ are equivalent, applying this inequality to the transformation and its inverse shows their imaginary parts are equal. For two interior points equality forces $c=0,d=\pm1$, hence an integer translation. Their real parts lie in an interval of length one, so the translation is zero. The only [matrices](../../../../../matrix.md) acting trivially are $\pm I$. On the boundary, the equality cases give precisely the stated vertical and circular identifications. This establishes the fundamental-domain claim, including its boundary convention.

An [elliptic point of a modular curve](../../../../../elliptic-point-of-a-modular-curve.md) means a fixed point of a nonidentity element of the effective [modular group](../../../../../modular-group.md) $PSL_2(\mathbb Z)$; the central [matrix](../../../../../matrix.md) $-I$ is not counted, since it acts trivially everywhere. The equality cases above show that the only such points in the closed region are

$$
\boxed{i,\qquad \rho=-\tfrac12+\tfrac{\sqrt3}{2}i,\qquad
\rho_+=\tfrac12+\tfrac{\sqrt3}{2}i=\rho+1.}
$$

Their [stabilizer subgroups](../../../../../stabilizer-subgroup.md) in $SL_2(\mathbb Z)$ are

$$
\boxed{\operatorname{Stab}(i)=\langle S\rangle\cong C_4,\quad
\operatorname{Stab}(\rho)=\langle ST\rangle\cong C_6,\quad
\operatorname{Stab}(\rho_+)=\langle TS\rangle\cong C_6,}
$$

where

$$
S=\begin{pmatrix}0&-1\\1&0\end{pmatrix},\quad
ST=\begin{pmatrix}0&-1\\1&1\end{pmatrix},\quad
TS=\begin{pmatrix}1&-1\\1&0\end{pmatrix}.
$$

Indeed $S^2=-I$, $(ST)^3=(TS)^3=-I$, and their fractional-linear fixed-point equations give the listed points. To see that these are the full [stabilizer subgroups](../../../../../stabilizer-subgroup.md), equality in $|cz+d|\geq1$ leaves only bottom rows $(0,\pm1),(\pm1,0)$, with the extra neighboring rows at the vertices. The fixed-point equation then fixes the top row. This yields exactly four [matrices](../../../../../matrix.md) at $i$, six at each vertex, and just $\{\pm I\}$ elsewhere. These are the [elliptic stabilizers of the modular group](../../../../../elliptic-stabilizers-of-the-modular-group.md). After passing to $PSL_2(\mathbb Z)$ their effective orders are two and three. The two vertices represent the same elliptic orbit.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
