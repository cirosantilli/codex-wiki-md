<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Put $n=x/R$ and $q=r(R)/R$. Differentiating $y=qx$ uses $\nabla R=n$ and $\nabla q=(r'-q)n/R$. Hence

$$
\boxed{F=qI+(r'-q)n\otimes n.}
$$

Its [radial eigenvalue](../../../eigenvalue.md) is $r'$ and its two tangential [eigenvalues](../../../eigenvalue.md) are $q$. They are positive by hypothesis, so they are also the principal stretches:

$$
\boxed{v_1=r',\qquad v_2=v_3=q.}
$$

For an [isotropic](../../../isotropy.md) [stored energy](../../../strain-energy-density.md) the [nominal stress](../../../nominal-stress-tensor.md) has the same radial/tangential [projectors](../../../projection-linear-algebra.md),

$$
P=DW(F)=\Phi_1 n\otimes n+\Phi_2(I-n\otimes n),
$$

where symmetry of $\Phi$ gives equal tangential derivatives. Since $\operatorname{Div}(n\otimes n)=2n/R$ and the scalar coefficients depend only on $R$,

$$
\operatorname{Div}P=\left[\frac{d\Phi_1}{dR}+\frac2R(\Phi_1-\Phi_2)\right]n.
$$

Thus [equilibrium](../../../equilibrium-point-of-a-dynamical-system.md) is exactly $\boxed{d\Phi_1/dR=2(\Phi_2-\Phi_1)/R}$.

For the particular energy define $\delta=r'q^2=\det F>0$. Its two derivatives are

$$
\Phi_1=\mu+h'(\delta)q^2,\qquad\Phi_2=\mu+h'(\delta)r'q.
$$

Also $q'=(r'-q)/R$. Differentiating the first formula and substituting the [equilibrium](../../../equilibrium-point-of-a-dynamical-system.md) equation gives

$$
h''(\delta)\delta'q^2+2h'(\delta)qq'=2h'(\delta)q(r'-q)/R=2h'(\delta)qq'.
$$

The last terms cancel. Strict positivity of $h''$ and $q$ yields $\boxed{\delta'=0}$, so $r^2r'=D R^2$ for one positive constant $D$. Integration gives $r^3=DR^3+C$.

The displacement data mean $r(1)=\lambda_1$ and $r(2)=2\lambda_2$, not $r(2)=\lambda_2$. Solving the two scalar equations gives

$$
\boxed{D=\frac{8\lambda_2^3-\lambda_1^3}{7},\qquad C=\frac{8(\lambda_1^3-\lambda_2^3)}7,\qquad r=(DR^3+C)^{1/3}.}
$$

The given inequality makes $D>0$. Since $r^3$ increases from $\lambda_1^3>0$ to $8\lambda_2^3$, it is positive on the whole shell, and $r'=DR^2/r^2>0$. Thus the formula is [smooth](../../../smooth-function.md) and [admissible](../../../admissible-representation-of-a-locally-profinite-group.md) and satisfies [equilibrium](../../../equilibrium-point-of-a-dynamical-system.md). Conversely every [admissible](../../../admissible-representation-of-a-locally-profinite-group.md) radial [equilibrium](../../../equilibrium-point-of-a-dynamical-system.md) had to have this constant [determinant](../../../determinant.md) and these two integration constants, proving [uniqueness](../../../uniqueness.md). This is a [constant-Jacobian radial equilibrium for a stretch-sum energy](../../../constant-jacobian-radial-equilibrium-for-a-stretch-sum-energy.md).

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2008](../../2008-split.md)
3. [Past exam of the solid mechanics course of the University of Oxford](../../split.md)
4. [Solid mechanics course of the University of Oxford](../../../solid-mechanics-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
