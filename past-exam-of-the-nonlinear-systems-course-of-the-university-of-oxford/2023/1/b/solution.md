<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Adjoin $\dot\mu=0$ and put $w=z+\mu$. The [extended centre manifold](../../../../extended-centre-manifold-for-a-parameter.md) is a graph $w=H(x,y,\mu)$ tangent to $w=0$ at the origin. The equations become

$$
\dot x=y,\qquad \dot y=-x+5\epsilon\mu y-5\epsilon y w,\qquad \dot w=-w+x^2,\qquad \dot\mu=0.
$$

Here $\epsilon>0$ is fixed. The [centre-manifold invariance equation](../../../../centre-manifold-invariance-equation.md), obtained by the [chain rule](../../../../chain-rule.md), is

$$
H_x y+H_y(-x+5\epsilon\mu y-5\epsilon yH)=-H+x^2.
$$

Write $H=H_2+O(\rho^3)$, where $\rho=|x|+|y|+|\mu|$ and $H_2$ is a homogeneous quadratic [polynomial](../../../../polynomial-split.md). To quadratic order the [centre-manifold invariance equation](../../../../centre-manifold-invariance-equation.md) is

$$
y\partial_xH_2-x\partial_yH_2=-H_2+x^2.
$$

The terms $\mu x,\mu y,\mu^2$ have zero [coefficients](../../../../coefficient.md): their equations are homogeneous, and the operator $1+y\partial_x-x\partial_y$ is invertible on these quadratic [polynomials](../../../../polynomial-split.md). For $H_2=ax^2+bxy+cy^2$, comparison of [coefficients](../../../../coefficient.md) gives

$$
-b=1-a,\qquad 2a-2c=-b,\qquad b=-c.
$$

Hence $a=3/5$, $b=-2/5$ and $c=2/5$, giving

$$
\boxed{z=-\mu+\frac35x^2-\frac25xy+\frac25y^2+O(\rho^3).}
$$

Substitution into the $y$ equation gives

$$
\boxed{\dot x=y,\qquad
\dot y=-x+\epsilon(5\mu y-3x^2y+2xy^2-2y^3)+O(\rho^4).}
$$

The constant in the [big O notation](../../../../big-o-notation.md) may depend on fixed $\epsilon$. Thus the equations printed in part (b) are the retained terms of the local [Taylor series](../../../../taylor-series.md), rather than an exact identity for the full reduced [vector field](../../../../vector-field.md).

For the [Hopf bifurcation](../../../../hopf-bifurcation.md) classification in part (a), set $\mu=0$ and use $x=r\cos\theta$, $y=-r\sin\theta$. The radial derivative is $\dot r=(x\dot x+y\dot y)/r$. Its cubic angular mean is

$$
\frac{\epsilon}{r}\left\langle-3x^2y^2+2xy^3-2y^4\right\rangle
=-\epsilon r^3\left(\frac38+\frac68\right)=-\frac{9\epsilon}{8}r^3.
$$

Here $\langle\cdot\rangle$ denotes the mean over one revolution. Removing the oscillatory cubic terms by a [near-identity transformation](../../../../near-identity-transformation.md) gives this same cubic radial coefficient in the [Hopf normal form](../../../../hopf-normal-form.md). The linear radial coefficient is $5\epsilon\mu/2$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the nonlinear systems course of the University of Oxford](../../../split.md)
5. [Nonlinear systems course of the University of Oxford](../../../../nonlinear-systems-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
