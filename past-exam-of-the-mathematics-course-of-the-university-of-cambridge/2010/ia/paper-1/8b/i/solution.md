<h1 id="8b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

An [orthogonal matrix](../../../../../../orthogonal-matrix.md) satisfies $R^TR=I$, so it preserves the [Euclidean norm](../../../../../../euclidean-norm.md). For a nonzero real [eigenvector](../../../../../../eigenvector.md) $v$,

$$
\|v\|^2=\|Rv\|^2=\|\lambda v\|^2=\lambda^2\|v\|^2.
$$

Therefore $\boxed{\lambda=\pm1}$. Geometrically, [eigenvalue](../../../../../../eigenvalue.md) $1$ fixes every vector on the [linear span](../../../../../../linear-span.md) of $v$; [eigenvalue](../../../../../../eigenvalue.md) $-1$ reverses every vector on that line. In either case the line is preserved as a set.

For $M$, solving $(M-I)v=0$ gives $y=x$, $z=y$, $x=z$. For $N$, the equations are $-2y-2z=0$ and $-2z=0$, hence $y=z=0$. For $P$, let $a=(1,1,1)^T$ and $J=aa^T$, so that $P=I-\frac23J$. Then $(P-I)v=0$ is equivalent to $x+y+z=0$. The resulting [eigenspaces](../../../../../../eigenspace.md) and their [bases](../../../../../../basis.md) are

$$
\boxed{\begin{aligned}
E_1(M)&=\operatorname{span}\{(1,1,1)^T\},&\dim E_1(M)&=1,\\
E_1(N)&=\operatorname{span}\{(1,0,0)^T\},&\dim E_1(N)&=1,\\
E_1(P)&=\operatorname{span}\{(1,-1,0)^T,(1,0,-1)^T\},&\dim E_1(P)&=2.
\end{aligned}}
$$

Solving all the equations shows that these lists contain the maximum possible numbers of independent [eigenvectors](../../../../../../eigenvector.md) with [eigenvalue](../../../../../../eigenvalue.md) $1$.

The columns of $M$ form an [orthonormal basis](../../../../../../orthonormal-basis.md), so $M$ is an [orthogonal matrix](../../../../../../orthogonal-matrix.md). Also $\det M=1$. Its fixed axis is the line through $a$, and on the perpendicular plane it acts as a two-dimensional rotation. If $\theta$ denotes the rotation angle, its [matrix trace](../../../../../../matrix-trace.md) is $1+2\cos\theta$. Since $\operatorname{tr}M=0$, we obtain $\cos\theta=-1/2$. To fix the orientation relative to $u=a/\sqrt3$, note that $Me_1=e_3$ and

$$
u\cdot(e_1\times Me_1)=u\cdot(e_1\times e_3)=-\frac1{\sqrt3}<0.
$$

The component of $e_1$ perpendicular to $u$ has squared length $2/3$, and this [scalar triple product](../../../../../../scalar-triple-product.md) equals $(2/3)\sin\theta$. Hence $\sin\theta=-\sqrt3/2$. Thus

$$
\boxed{M:\ \text{axis }\mathbb R(1,1,1),\quad
\theta=-\frac{2\pi}{3}\text{ about }\frac{(1,1,1)}{\sqrt3}.}
$$

Equivalently, its unsigned angle is $2\pi/3$, or its positive angle is $2\pi/3$ about the opposite oriented axis.

For $P$, the [reflection in a hyperplane](../../../../../../reflection-in-a-hyperplane.md) formula gives

$$
P=I-2\frac{aa^T}{a^Ta}.
$$

It fixes the plane $a\cdot v=0$ pointwise and maps $a$ to $-a$, so $\boxed{P\text{ reflects in }x+y+z=0}$. These actions also show that $P$ is an [orthogonal matrix](../../../../../../orthogonal-matrix.md). In contrast, the second column of $N$ has squared length $5$, so $N$ is not [orthogonal](../../../../../../orthogonal-vectors.md) and cannot represent either of these Euclidean motions.

A [diagonalizable matrix](../../../../../../diagonalizable-matrix.md) must have a [basis](../../../../../../basis.md) of [eigenvectors](../../../../../../eigenvector.md) over the field in question. For $M$, a direct [determinant](../../../../../../determinant.md) computation gives $\chi_M(t)=1-t^3$. Its [eigenvalues](../../../../../../eigenvalue.md) are $1,\omega,\omega^2$, where $\omega=e^{2\pi i/3}$. Only one is real, with one-dimensional [eigenspace](../../../../../../eigenspace.md), so $M$ is not diagonalizable over $\mathbb R$. Over $\mathbb C$ the three [eigenvalues](../../../../../../eigenvalue.md) are distinct, and the vectors $(1,\lambda,\lambda^2)^T$ for $\lambda=1,\omega,\omega^2$ give an [eigenbasis](../../../../../../eigenbasis.md). The upper triangular [matrix](../../../../../../matrix.md) $N$ has only [eigenvalue](../../../../../../eigenvalue.md) $1$, of [algebraic multiplicity](../../../../../../algebraic-multiplicity.md) $3$, but its [eigenspace](../../../../../../eigenspace.md) has dimension $1$ over either field. Hence $N$ is not diagonalizable over either field. For $P$, the two real plane vectors displayed above, together with $a$, form an [eigenbasis](../../../../../../eigenbasis.md), with [eigenvalues](../../../../../../eigenvalue.md) $1,1,-1$. They remain independent over $\mathbb C$. Therefore

$$
\boxed{\begin{array}{c|cc}
&\mathbb R&\mathbb C\\\hline
M&\text{not diagonalizable}&\text{diagonalizable}\\
N&\text{not diagonalizable}&\text{not diagonalizable}\\
P&\text{diagonalizable}&\text{diagonalizable}
\end{array}}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [8B](../../8b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
