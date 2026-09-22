<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

By symmetry, the [centre of mass](../../../../../../center-of-mass.md) is $G=(0,0,\ell/2)$. Choose horizontal axes through $G$ and the vertical symmetry axis as the third axis, writing $Z=z-\ell/2$. With uniform [mass density](../../../../../../density.md) $\rho$, the [inertia tensor](../../../../../../inertia-tensor.md) has entries

$$
I_{ij}=\int\bigl(|\mathbf R|^2\delta_{ij}-R_iR_j\bigr)\,dm,
\qquad \mathbf R=(x,y,Z),\qquad dm=\rho r\,dr\,d\theta\,dz.
$$

Reflection in each coordinate [plane](../../../../../../plane.md) makes all the mixed [integrals](../../../../../../integral-split.md) $\int xy\,dm$, $\int xZ\,dm$, and $\int yZ\,dm$ vanish. Rotational symmetry about the vertical axis gives $I_{11}=I_{22}=A$. Thus these are [principal axes](../../../../../../principal-axis.md) and

$$
\mathbf I_G=\begin{pmatrix}A&0&0\\0&A&0\\0&0&C\end{pmatrix}.
$$

The [axial moment of inertia of a hollow cylinder](../../../../../../axial-moment-of-inertia-of-a-hollow-cylinder.md) is

$$
C=\int(x^2+y^2)\,dm
=2\pi\rho\ell\int_a^b r^3\,dr
=\frac{\pi\rho\ell}{2}(b^4-a^4).
$$

Its [mass](../../../../../../mass.md) is $M=\pi\rho\ell(b^2-a^2)$. Dividing and factoring the difference of squares gives

$$
\boxed{\mathbf I_G=\operatorname{diag}(A,A,C),\qquad C=\frac12M(a^2+b^2).}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [Mathematics IV resit](../../../mathematics-iv-resit-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
