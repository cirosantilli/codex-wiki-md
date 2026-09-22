<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In a parabolic conduction valley, $\mathbf v=\hbar M^{-1}\mathbf k$. The [Lorentz force](../../../../lorentz-force.md) on an [electron](../../../../electron.md) gives $M\dot{\mathbf v}=-e\mathbf v\times\mathbf B=e\mathbf B\times\mathbf v$. In the principal axes of the stated [effective-mass tensor](../../../../effective-mass-tensor.md),

$$
\begin{pmatrix}\dot v_x\\\dot v_y\\\dot v_z\end{pmatrix}
=e\begin{pmatrix}0&-B_z/m_1&B_y/m_1\\B_z/m_1&0&-B_x/m_1\\-B_y/m_2&B_x/m_2&0\end{pmatrix}
\begin{pmatrix}v_x\\v_y\\v_z\end{pmatrix}.
$$

Call the matrix on the right $A$. Its characteristic polynomial is

$$
\det(\lambda I-A)=\lambda\left[\lambda^2+e^2\left(\frac{B_z^2}{m_1^2}+\frac{B_x^2+B_y^2}{m_1m_2}\right)\right].
$$

One mode has zero frequency, corresponding to constant drift along the field; the other two have eigenvalues $\pm i\omega$. Thus

$$
\omega^2=e^2\frac{m_1(B_x^2+B_y^2)+m_2B_z^2}{m_1^2m_2},
\qquad
\boxed{\omega=\frac{e|\mathbf B|}{m_{\mathrm{cr}}},\quad m_{\mathrm{cr}}=|\mathbf B|\sqrt{\frac{m_1^2m_2}{m_1B_x^2+m_1B_y^2+m_2B_z^2}}.}
$$

More generally the [ellipsoidal cyclotron mass](../../../../ellipsoidal-cyclotron-mass.md) is $m_{\mathrm{cr}}^2=\det M/(\widehat{\mathbf B}^TM\widehat{\mathbf B})$. The tensor axes must be rotated for the differently oriented valleys.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the condensed matter physics major option course of the University of Oxford](../../../split.md)
5. [Condensed matter physics major option course of the University of Oxford](../../../../condensed-matter-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
