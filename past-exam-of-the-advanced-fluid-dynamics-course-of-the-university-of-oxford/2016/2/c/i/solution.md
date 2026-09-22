<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $g=\dot\gamma$ and use $G_{yx}=g$ for the source's [velocity gradient](../../../../../velocity-gradient.md) convention. Seek the homogeneous stationary [stress](../../../../../stress.md) reached under steady [simple shear flow](../../../../../simple-shear-flow.md). The [material derivative](../../../../../material-derivative.md) of that [stress tensor](../../../../../cauchy-stress-tensor.md) vanishes. In the $xy$ plane,

$$
G=\begin{pmatrix}0&0\\g&0\end{pmatrix},\qquad
E=\frac12\begin{pmatrix}0&g\\g&0\end{pmatrix}.
$$

The $xx$, $yy$ and $zz$ components of the [constitutive equation](../../../../../constitutive-equation.md) give, respectively,

$$
T_{xx}-(2\tau-\alpha)gT_{xy}=0,\qquad
T_{yy}+\alpha gT_{xy}=0,\qquad T_{zz}=0.
$$

Thus, putting $D=1+\alpha(2\tau-\alpha)g^2$ and using the [shear stress](../../../../../shear-stress.md) calculated below,

$$
\boxed{T_{xx}=\frac{\mu(2\tau-\alpha)g^2}{D},\qquad T_{yy}=-\frac{\mu\alpha g^2}{D},\qquad T_{zz}=0.}
$$

The out-of-plane shear components vanish on the homogeneous branch. The two [normal-stress differences](../../../../../normal-stress-difference.md) are

$$
N_1=2\tau gT_{xy}=\frac{2\mu\tau g^2}{D},\qquad
N_2=-\alpha gT_{xy}=-\frac{\mu\alpha g^2}{D},
\qquad \boxed{\frac{N_2}{N_1}=-\frac{\alpha}{2\tau}.}
$$

The ratio is defined at nonzero shear when $N_1\ne0$; at $g=0$ both differences vanish, and the displayed constant is their limiting ratio. An arbitrary isotropic [pressure](../../../../../pressure-split.md) in the total [Cauchy stress tensor](../../../../../cauchy-stress-tensor.md) cancels from both differences; it is not an arbitrary addition to the constitutively defined extra [stress](../../../../../stress.md) $\mathsf T$ itself.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2016](../../../../2016-split.md)
5. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../../split.md)
6. [Advanced fluid dynamics course of the University of Oxford](../../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
