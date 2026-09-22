<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $u=(a,b)^T$. The [Pauli matrices](../../../../pauli-matrices.md) give

$$
U^0=\frac{|a|^2+|b|^2}{2},\quad
U^1=\operatorname{Re}(a^*b),\quad
U^2=\operatorname{Im}(a^*b),\quad
U^3=\frac{|a|^2-|b|^2}{2}.
$$

Hence

$$
(U^1)^2+(U^2)^2+(U^3)^2
=|a|^2|b|^2+\frac{(|a|^2-|b|^2)^2}{4}
=\frac{(|a|^2+|b|^2)^2}{4}=(U^0)^2.
$$

Therefore $\boxed{U_\mu U^\mu=0}$, with $U^0>0$ for $u\ne0$: the bilinear is a future null [Lorentz four-vector](../../../../four-vector.md), and $u=0$ gives the zero vector.

For $S=e^{\rho\sigma_z/2}=\operatorname{diag}(e^{\rho/2},e^{-\rho/2})$, the transformed components are $a'=e^{\rho/2}a$ and $b'=e^{-\rho/2}b$. Thus $a'^*b'=a^*b$, while the two squared magnitudes acquire factors $e^{\rho}$ and $e^{-\rho}$. Substitution gives

$$
\boxed{\begin{pmatrix}U'^0\\U'^1\\U'^2\\U'^3\end{pmatrix}
=\begin{pmatrix}
\cosh\rho&0&0&\sinh\rho\\
0&1&0&0\\0&0&1&0\\
\sinh\rho&0&0&\cosh\rho
\end{pmatrix}
\begin{pmatrix}U^0\\U^1\\U^2\\U^3\end{pmatrix}.}
$$

The matrix preserves the [Minkowski metric](../../../../minkowski-metric.md) and is an active boost along $+z$ of [rapidity](../../../../rapidity.md) $\rho$, with velocity $c\tanh\rho$. Relative to the passive standard-boost convention of part [i](../../1/d/i.md), its velocity parameter has the opposite sign.

For $S=e^{i\theta\sigma_z}$, $a'=e^{i\theta}a$ and $b'=e^{-i\theta}b$, so $a'^*b'=e^{-2i\theta}a^*b$. Consequently

$$
\boxed{U'^0=U^0,\quad U'^3=U^3,\quad
\begin{pmatrix}U'^1\\U'^2\end{pmatrix}
=\begin{pmatrix}\cos2\theta&\sin2\theta\\-\sin2\theta&\cos2\theta\end{pmatrix}
\begin{pmatrix}U^1\\U^2\end{pmatrix}.}
$$

This is an active right-handed spatial rotation through $-2\theta$ about $z$. The minus sign follows from the specified positive $i\theta\sigma_z$ exponent; the familiar positive-angle spin rotation uses $e^{-i\varphi\sigma_z/2}$. The doubled angle exhibits the [Lorentz spinor double cover](../../../../lorentz-spinor-double-cover.md): $u$ and $-u$ give the same four-vector.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the symmetry and relativity course of the University of Oxford](../../../split.md)
5. [Symmetry and relativity course of the University of Oxford](../../../../symmetry-and-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
