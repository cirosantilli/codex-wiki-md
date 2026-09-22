<h1 id="17b/solution">Solution</h1>

↑ **Parent:** [17B](../17b.md)

The total [angular momentum operator](../../../../../angular-momentum-operator.md) is

$$
\mathbf L^2=L_x^2+L_y^2+L_z^2.
$$

Using the cyclic [orbital angular momentum commutation relations](../../../../../orbital-angular-momentum-commutation-relations.md),

$$
[L_z,L_x^2]=i\hbar(L_yL_x+L_xL_y),
\qquad
[L_z,L_y^2]=-i\hbar(L_xL_y+L_yL_x),
$$

while $[L_z,L_z^2]=0$; hence $\boxed{[L_z,\mathbf L^2]=0}$. In Cartesian coordinates,

$$
\boxed{L_z=-i\hbar\left(x\frac{\partial}{\partial y}-y\frac{\partial}{\partial x}\right)}.
$$

Because $L_z(x+iy)=\hbar(x+iy)$ and it annihilates $z$ and every radial function,

$$
L_z[(x+iy)^mz^nf(r)]=m\hbar(x+iy)^mz^nf(r).
$$

Replacing $i$ by $-i$ gives eigenvalue $-m\hbar$.

The six-dimensional space splits into the five trace-free quadratic [spherical harmonics](../../../../../spherical-harmonic.md) with $\ell=2$ and one radial state with $\ell=0$. A simultaneous eigenbasis for $L_z$ and $\mathbf L^2$ is

$$
\begin{array}{c|c|c}
\text{state}&L_z&\mathbf L^2\\ \hline
(x+iy)^2f(r)&2\hbar&6\hbar^2\\
(x+iy)zf(r)&\hbar&6\hbar^2\\
(2z^2-x^2-y^2)f(r)&0&6\hbar^2\\
(x-iy)zf(r)&-\hbar&6\hbar^2\\
(x-iy)^2f(r)&-2\hbar&6\hbar^2\\
(r^2-3)f(r)&0&0
\end{array}
$$

where the eigenvalue $\ell(\ell+1)\hbar^2$ of $\mathbf L^2$ was used. Every displayed state is a complex [linear combination](../../../../../linear-combination.md) of the original six energy eigenstates, so it is still an energy eigenstate at the same level.

## ↑ Ancestors (10)

1. [17B](../17b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
