<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Wirtinger derivative](../../../../../../wirtinger-derivatives.md) $q_z=(q_x-iq_y)/2$ and write $z=x+iy$. Since $q$ solves the [Laplace equation](../../../../../../laplace-equation.md), $q_z$ is a [holomorphic function](../../../../../../holomorphic-function.md). The transforms in the question select solutions with sufficient decay at infinity. In this class the solution, when it exists, is unique; hence reflection of the symmetric data about $y=\ell/2$ gives

$$
q(x,\ell-y)=q(x,y),\qquad q(x,\ell)=q(x,0).
$$

For $\gamma>0$, this uniqueness follows directly from [Green's first identity](../../../../../../green-s-first-identity.md): the homogeneous problem has integral $\int|\nabla q|^2+\gamma\int_{y=0,\ell}q^2=0$. For arbitrary real $\gamma$, the decaying-class qualifications are explained in part (c). Without a condition at infinity, symmetry of the data alone would not force symmetry of every solution.

Put $c=q(0,0)$, $f(x)=q(x,0)$, and introduce a known transform

$$
\psi(s)=\frac12\int_0^\infty e^{sx}f(x)dx,\qquad H(k)=\frac12\int_0^\ell e^{ky}g(y)dy.
$$

The bottom [Robin boundary condition](../../../../../../robin-boundary-condition.md) gives $q_y=\gamma f$, while the top one gives $q_y=-\gamma f$. The bottom side is traversed from infinity to zero. [Integration by parts](../../../../../../integration-by-parts.md) therefore gives

$$
G_1=-\frac12\int_0^\infty e^{-ikx}(f'-i\gamma f)dx=\boxed{\frac c2-i(k-\gamma)\psi(-ik)}.
$$

The top side is traversed from $i\ell$ towards infinity, and its exponential supplies $e^{k\ell}$, giving

$$
\boxed{G_3=e^{k\ell}\left[-\frac c2+i(k+\gamma)\psi(-ik)\right].}
$$

On the vertical side, $dz=i\,dy$ and the prescribed [Neumann boundary condition](../../../../../../neumann-boundary-condition.md) is $q_x=g$. Thus

$$
G_2=\frac12\int_0^\ell e^{ky}(q_y+ig)dy=\boxed{\phi(k)+iH(k)}.
$$

Both the side orientations and the factor $1/2$ from the [Wirtinger derivative](../../../../../../wirtinger-derivatives.md) are essential to these signs.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
