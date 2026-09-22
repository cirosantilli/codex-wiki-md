<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [geodesic flow](../../../../../../geodesic-flow.md) of a closed negatively curved surface is a topologically transitive [Anosov flow](../../../../../../anosov-flow.md). In particular, its Jacobi-field hyperbolicity and the usual negative-curvature transitivity theorem allow the smooth [Livsic theorem](../../../../../../livsic-theorem.md) to be applied. Set $b(x,v)=\beta_x(v,v)$. The given closed-geodesic integrals are exactly its periodic-orbit obstructions on $SM$. Therefore

$$
\boxed{Xu=b,\qquad u\in C^\infty(SM)}.
$$

We make the differential operators and signs explicit. On the [unit tangent bundle](../../../../../../unit-tangent-bundle.md), let $V$ generate positive fibre rotation, $X$ be the geodesic [vector field](../../../../../../vector-field.md) and $H=[V,X]$. For the [canonical coframe of a surface unit tangent bundle](../../../../../../canonical-coframe-of-a-surface-unit-tangent-bundle.md), write

$$
\alpha(\xi)=\langle v,d\pi\xi\rangle,\qquad
\theta(\xi)=\langle iv,d\pi\xi\rangle,
$$

and let $\omega$ be the [Levi-Civita connection](../../../../../../levi-civita-connection.md) form with $\omega(V)=1$. This uses $\theta$ for a [one-form](../../../../../../one-form.md), keeping $\beta$ for the given tensor. The dual frame is $(X,H,V)$, and the structure equations are

$$
d\alpha=\omega\wedge\theta,\qquad d\theta=\alpha\wedge\omega,
\qquad d\omega=-K\alpha\wedge\theta.
$$

These follow by writing the two horizontal forms as a rotated local orthonormal [coframe](../../../../../../coframe.md) and $\omega=d\vartheta+\omega_0$, with $\omega_0$ its [connection 1-form](../../../../../../connection-1-form-split.md). Equivalently, differentiating the sine and cosine components of $X$ twice in the fibre angle gives

$$
[V,X]=H,\qquad [V,H]=-X.
$$

The curvature equation also gives $[X,H]=KV$. The [Liouville volume of a surface geodesic flow](../../../../../../liouville-volume-of-a-surface-geodesic-flow.md) will be taken positive in the base/positive-fibre orientation, namely $\mu=\alpha\wedge\theta\wedge\omega$.

In an oriented orthonormal frame at $x$, put $v=(\cos\vartheta,\sin\vartheta)$. The [symmetric tensor](../../../../../../symmetric-tensor.md) evaluation is

$$
b(x,v)=\frac{\beta_{11}+\beta_{22}}2
+\frac{\beta_{11}-\beta_{22}}2\cos(2\vartheta)
+\beta_{12}\sin(2\vartheta).
$$

Since $V=\partial_\vartheta$, this proves $(V^3+4V)b=0$.

The [Lie bracket of vector fields](../../../../../../lie-bracket-of-vector-fields.md) identities give an operator identity that supplies the required equation. First,

$$
X V^2=V^2X-2HV+X.
$$

Using $VH=HV-X$ and $XV=VX-H$, differentiate this expression once more to obtain

$$
\begin{aligned}
VX(V^2u+u)
&=V^3Xu-2HV^2u+2XVu+2VXu\\
&=(V^3+4V)Xu-2H(V^2u+u).
\end{aligned}
$$

For $\varphi=V^2u+u$ and $Xu=b$, the first term vanishes by the explicit fibre calculation. Hence

$$
\boxed{VX\varphi=-2H\varphi}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 14](../../../paper-14-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
