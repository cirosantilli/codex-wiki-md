<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take two time derivatives at fixed reference position $\mathbf X$:

$$
\ddot{\mathbf x}=\ddot{\mathbf F}\mathbf X+\ddot{\mathbf c}.
$$

The constraint $\det\mathbf F=1$ ensures that the [deformation gradient](../../../../../deformation-gradient.md) is invertible, so $\mathbf X=\mathbf F^{-1}(\mathbf x-\mathbf c)$. Thus the spatial [material acceleration](../../../../../material-acceleration.md) is the affine [vector field](../../../../../vector-field.md)

$$
\ddot{\mathbf x}=\mathbf A(t)(\mathbf x-\mathbf c(t))+\ddot{\mathbf c}(t),
\qquad \mathbf A=\ddot{\mathbf F}\mathbf F^{-1}.
$$

Its spatial [gradient](../../../../../gradient.md) is $\mathbf A$, and its [curl](../../../../../curl.md) is

$$
\nabla\times\ddot{\mathbf x}
=(A_{32}-A_{23},\ A_{13}-A_{31},\ A_{21}-A_{12}).
$$

Part (b)(iii) therefore requires

$$
\boxed{\ddot{\mathbf F}\mathbf F^{-1}
=\left(\ddot{\mathbf F}\mathbf F^{-1}\right)^T.}
$$

Equivalently, multiplying on the left by $\mathbf F^T$ and on the right by $\mathbf F$ gives

$$
\boxed{\mathbf F^T\ddot{\mathbf F}=\ddot{\mathbf F}^{\,T}\mathbf F.}
$$

The translation $\mathbf c(t)$ contributes no spatial [curl](../../../../../curl.md) and is unrestricted by this condition. A useful equivalent first integral is

$$
\frac d{dt}\left(\mathbf F^T\dot{\mathbf F}-\dot{\mathbf F}^{\,T}\mathbf F\right)=\mathbf0:
$$

the antisymmetric [matrix](../../../../../matrix.md) in parentheses must be constant, and need not vanish. The separate constraint $\det\mathbf F=1$ is still required; differentiating it also gives $\operatorname{tr}(\dot{\mathbf F}\mathbf F^{-1})=0$.

The condition is understood in the setting of part (b), where a static family already exists under the prescribed [body force](../../../../../body-force.md). For a homogeneous elastic [deformation gradient](../../../../../deformation-gradient.md), the elastic [stress](../../../../../stress.md) $\mathbf S(\mathbf F)$ is spatially constant. Static [balance of linear momentum](../../../../../balance-of-linear-momentum.md) consequently gives $\nabla p_0=\rho\mathbf b$, ensuring that $\mathbf b$ has a [scalar potential](../../../../../scalar-potential.md). If the static-family assumption were dropped and an arbitrary time-independent [body force](../../../../../body-force.md) allowed, the general necessary condition would instead be $\nabla\times\ddot{\mathbf x}=\nabla\times\mathbf b$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the solid mechanics course of the University of Oxford](../../../../split.md)
6. [Solid mechanics course of the University of Oxford](../../../../../solid-mechanics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
