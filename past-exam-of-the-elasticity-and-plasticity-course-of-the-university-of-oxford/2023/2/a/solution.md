<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Work to first order in the [slope](../../../../slope.md) $w'$ and take $B$ constant. The [elastic beam](../../../../elastic-beam.md) is slender, its cross-sections remain plane and normal to its centreline, transverse shear deformation is neglected, and the loading is quasi-static. There are no distributed couples. In a non-contact interval the distributed [force](../../../../force-split.md) is $-p\mathbf e_z$ and there is no axial distributed [force](../../../../force-split.md). These are the assumptions of the small-deformation [Euler-Bernoulli beam equation](../../../../euler-bernoulli-beam-equation.md), with an optional prescribed [tension](../../../../tension.md) retained in transverse [force balance](../../../../force-balance.md).

Choose the internal section resultant on the right face of a segment as

$$
\mathbf F=T\mathbf e_x+(Tw'+N)\mathbf e_z,
$$

where $N$ is the [transverse shear force](../../../../transverse-shear-force.md), and take the section [bending moment](../../../../bending-moment.md) as $M\mathbf e_y$. Longitudinal and transverse [force balance](../../../../force-balance.md) on a segment of length $dx$ give $T'=0$ and $(Tw'+N)'=p$. Balancing the [torques](../../../../torque.md) about its left end gives $M'=N$: the [torque](../../../../torque.md) from the transverse section resultant is $-N\,dx\,\mathbf e_y$. Therefore

$$
\boxed{T'=0,\qquad Tw''+N'=p,\qquad M'=N.}
$$

With this positive-$y$ [bending moment](../../../../bending-moment.md) convention, the linear relation between [bending moment](../../../../bending-moment.md) and [curvature](../../../../curvature.md) is $M=-Bw''$. Thus $N=-Bw'''$, and substitution gives

$$
\boxed{Bw''''-Tw''+p=0.}
$$

The [tension](../../../../tension.md) need not be small compared with the transverse restoring terms, but products arising solely from finite deformation, such as the change of axial extension proportional to $(w')^2$, are outside this linear model. A separate axial constitutive constraint would be required to determine an unknown [tension](../../../../tension.md) from fixed end positions.

In an open contact interval, the upward distributed [normal contact force](../../../../normal-contact-force.md) is $R$. At this order the smooth obstacle supplies no axial [force](../../../../force-split.md); its vertical resultant changes the downward load to $p-R$. Hence

$$
\boxed{Bw''''-Tw''+p=R.}
$$

For nonadhesive [unilateral beam contact](../../../../unilateral-beam-contact.md), the obstacle can push but cannot pull, so $R\geq0$. The accompanying constraints are $w\geq f$ and $(w-f)R=0$. A negative $R$ would require adhesion and would invalidate the proposed contact region. If $f$ is four times differentiable, the distributed [normal contact force](../../../../normal-contact-force.md) inside an open contact interval is $R=Bf''''-Tf''+p$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../split.md)
5. [Elasticity and plasticity course of the University of Oxford](../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
