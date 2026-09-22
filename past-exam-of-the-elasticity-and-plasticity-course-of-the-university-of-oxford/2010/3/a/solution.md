<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Differentiate the [displacement](../../../../displacement.md) components. The shear strains involving $z$ vanish because $u_z=-w_x$ and $v_z=-w_y$. The full [infinitesimal strain tensor](../../../../infinitesimal-strain-tensor.md) is

$$
\boxed{\mathcal E=z\begin{pmatrix}
-a&-b&0\\-b&-c&0\\0&0&\dfrac{\nu(a+c)}{1-\nu}
\end{pmatrix}.}
$$

In particular $\operatorname{tr}\mathcal E=(2\nu-1)(a+c)z/(1-\nu)$. Substituting the Lamé coefficients into the constitutive law gives

$$
\boxed{\tau=-\frac{Ez}{1-\nu^2}
\begin{pmatrix}a+\nu c&(1-\nu)b&0\\(1-\nu)b&c+\nu a&0\\0&0&0\end{pmatrix}.}
$$

For example $\tau_{zz}=\lambda\operatorname{tr}\mathcal E+2\mu e_{zz}=0$: the thickness-direction strain supplies exactly the plane-stress Poisson correction. Also $\tau_{xy}=-Ebz/(1+\nu)$, confirming the off-diagonal factor.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../split.md)
5. [Elasticity and plasticity course of the University of Oxford](../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
