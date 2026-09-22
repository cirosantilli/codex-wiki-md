<h1 id="6a/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the specified unit [vector](../../../../../../vector.md),

$$
A-C=\frac13\begin{pmatrix}
\alpha&\alpha-3&\alpha\\
\alpha&\alpha&\alpha-3\\
\alpha-3&\alpha&\alpha
\end{pmatrix}.
$$

For a cyclic [matrix](../../../../../../matrix.md) with first row $(a,b,c)$, its [determinant](../../../../../../determinant.md) is $a^3+b^3+c^3-3abc$. Here it gives

$$
\det(A-C)=\frac{2\alpha^3+(\alpha-3)^3-3\alpha^2(\alpha-3)}{27}=\alpha-1.
$$

Therefore $Ax=Cx$ has only the zero solution if $\alpha\ne1$. At $\alpha=1$, $A=I$ and $A-C$ has kernel consisting of the equal-coordinate [vectors](../../../../../../vector.md). The complete answer is

$$
\boxed{\alpha\ne1:\ x=0;\qquad \alpha=1:\ x=t(1,1,1),\quad t\in\mathbb R.}
$$

Geometrically, $C^TC=I$, $\det C=1$ and $Cn=n$, so $C$ is a [rotation matrix](../../../../../../rotation-matrix.md) about the $n$ axis. Its [matrix trace](../../../../../../matrix-trace.md) is two, giving $\cos\theta=(\operatorname{tr}C-1)/2=1/2$; its skew part selects angle $-\pi/3$ about the oriented axis $n$. It has no fixed nonzero perpendicular [vector](../../../../../../vector.md). Meanwhile $A$ preserves perpendicular components and scales the axial component by $\alpha$. Comparing these components first forces $x_\perp=0$, and then $(\alpha-1)x_\parallel=0$, exactly matching the [determinant](../../../../../../determinant.md) calculation, including the noninvertible case $\alpha=0$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6A](../../6a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
