<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The first [Piola-Kirchhoff stress tensor](../../../piola-kirchhoff-stress-tensors.md) $T_R$ maps a reference normal to force per reference area. The [Cauchy stress tensor](../../../cauchy-stress-tensor.md) $T$ maps a current normal to force per current area. [Nanson's formula](../../../nanson-s-formula.md) gives $\mathbf n\,da=JF^{-T}\mathbf N\,dA$. Equating the actual surface force in both descriptions gives $T_R=JTF^{-T}$, and therefore

$$
\boxed{T=J^{-1}T_RF^T.}
$$

For [incompressibility](../../../incompressible-flow.md) $\boxed{J=1}$. The strain-energy derivative only fixes the constitutive stress up to a [constraint reaction in hyperelastic stress](../../../constraint-reaction-in-hyperelastic-stress.md): $T_R=DW-p\operatorname{cof}F$, hence $T=DW F^T-pI$. The scalar $p$ is a [Lagrange multiplier](../../../lagrange-multiplier.md) determined by equilibrium and boundary [tractions](../../../traction.md), rather than by the isochoric energy alone.

In [principal stretch](../../../principal-stretch.md) axes, the extra [principal stress](../../../principal-stress.md) is $v_i\partial W/\partial v_i=2\alpha v_i^2-2\beta v_i^{-2}$, up to that arbitrary spherical reaction. With $B=FF^T$, its [eigenvalues](../../../eigenvalue.md) are $v_i^2$, so isotropy yields

$$
\boxed{T^*=2\alpha B-2\beta B^{-1},\qquad T=T^*-pI.}
$$

For the prescribed [simple shear](../../../simple-shear.md),

$$
F=\begin{pmatrix}1&\gamma&0\\0&1&0\\0&0&1\end{pmatrix},\quad
B=\begin{pmatrix}1+\gamma^2&\gamma&0\\\gamma&1&0\\0&0&1\end{pmatrix},\quad
B^{-1}=\begin{pmatrix}1&-\gamma&0\\-\gamma&1+\gamma^2&0\\0&0&1\end{pmatrix}.
$$

The $x_3$ faces retain normal $\pm\mathbf e_3$, and zero [traction](../../../traction.md) there gives $p=2(\alpha-\beta)$. Thus

$$
\boxed{T=2\gamma\begin{pmatrix}\alpha\gamma&\alpha+\beta&0\\\alpha+\beta&-\beta\gamma&0\\0&0&0\end{pmatrix}.}
$$

This constant stress satisfies the interior equilibrium equation, and the remaining face forces maintain the deformation.

To compute the angle, the material face $x_1=1$ becomes the spatial plane $y_1-\gamma y_2=1$. Its outward [unit normal](../../../unit-normal.md) and an in-plane unit tangent are

$$
\mathbf n=\frac{(1,-\gamma,0)}{\sqrt{1+\gamma^2}},\qquad\mathbf m=\frac{(\gamma,1,0)}{\sqrt{1+\gamma^2}}.
$$

Resolve the current [traction](../../../traction.md) $\mathbf t=T\mathbf n$ into these directions:

$$
N=\mathbf n\cdot T\mathbf n=-\frac{2\gamma^2(\alpha+2\beta+\beta\gamma^2)}{1+\gamma^2},\qquad
S=\mathbf m\cdot T\mathbf n=\frac{2\gamma(\alpha+\beta)}{1+\gamma^2}.
$$

Since $N<0$ for nonzero $\gamma$, the angle lies above $\pi/2$, and

$$
\boxed{\theta-\frac\pi2=\arctan\left(\frac{|\gamma|(\alpha+2\beta+\beta\gamma^2)}{\alpha+\beta}\right).}
$$

Using $\arctan z\sim z$ at zero gives

$$
\boxed{\lim_{\gamma\to0}\frac{\theta-\pi/2}{|\gamma|}=\frac{\alpha+2\beta}{\alpha+\beta}.}
$$

Using the undeformed normal $\mathbf e_1$ would give the wrong coefficient. The transformed [unit normal](../../../unit-normal.md) is essential to this [simple-shear traction angle for a Mooney-Rivlin solid](../../../simple-shear-traction-angle-for-a-mooney-rivlin-solid.md).

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2009](../../2009-split.md)
3. [Past exam of the solid mechanics course of the University of Oxford](../../split.md)
4. [Solid mechanics course of the University of Oxford](../../../solid-mechanics-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
