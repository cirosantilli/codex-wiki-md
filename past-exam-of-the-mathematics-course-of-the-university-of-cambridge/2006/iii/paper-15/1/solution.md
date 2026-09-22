<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the [Levi-Civita connection](../../../../../levi-civita-connection.md) and the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) convention

$$
\mathcal R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z,
\qquad K_M(T,E)=\langle\mathcal R(E,T)T,E\rangle
$$

for orthonormal $T,E$. Thus the round [sphere](../../../../../sphere.md) has positive [sectional curvature](../../../../../sectional-curvature.md). Work on a fixed [compact](../../../../../compact-space.md) parameter interval $[a,b]$ inside the given open interval; this keeps all differentiations and endpoint evaluations well-defined. The base [geodesic](../../../../../geodesic.md) is regular and has constant speed, so a constant rescaling of $t$ makes it unit-speed. Put $T=\partial_t\phi$, $J=\partial_s\phi$, $D_t=\nabla_T$, $D_s=\nabla_J$ and evaluate at $s=0$. The [torsion-free connection](../../../../../torsion-free-connection.md) gives $D_sT=D_tJ$ because the two parameter derivatives commute. The [geodesic](../../../../../geodesic.md) equation is $D_tT=0$.

Differentiating the [length of a curve](../../../../../length-of-a-curve.md) once and twice, using [metric compatibility](../../../../../metric-compatibility.md), gives

$$
L'(0)=\int_a^b\langle D_tJ,T\rangle\,dt
=[\langle J,T\rangle]_a^b,
$$

and

$$
L''(0)=\int_a^b\left(|D_tJ|^2-\langle D_tJ,T\rangle^2+\langle D_sD_tJ,T\rangle\right)dt.
$$

Let $A=D_sJ$. The curvature commutator gives $D_sD_tJ=D_tA+\mathcal R(J,T)J$, and the skew-adjoint curvature symmetry gives $\langle\mathcal R(J,T)J,T\rangle=-\langle\mathcal R(J,T)T,J\rangle$. Integration by parts therefore proves the [moving-endpoint second variation of Riemannian arc length](../../../../../moving-endpoint-second-variation-of-riemannian-arc-length.md):

$$
\boxed{L''(0)=[\langle A,T\rangle]_a^b+
\int_a^b\left(|D_tJ|^2-\langle D_tJ,T\rangle^2-\langle\mathcal R(J,T)T,J\rangle\right)dt.}
$$

Equivalently, with $W=J-\langle J,T\rangle T$, the integral is $I(W,W)$, the [Riemannian index form](../../../../../riemannian-index-form.md). The endpoints of this [geodesic variation](../../../../../geodesic-variation.md) generally move, so the displayed boundary term must be retained. For a base speed $c$ instead of one, the boundary and integral have an overall factor $1/c$, and the subtracted square inside the integral is $\langle D_tJ,T\rangle^2/c^2$. Returning to the original parameter, every ruling has constant speed, so $L_{[a,b]}(s)=(b-a)|\partial_t\phi(0,s)|$ and the full open-interval length is $2\delta|\partial_t\phi(0,s)|$. Consequently

$$
\left.\frac{d^2}{ds^2}L(\gamma_s)\right|_{s=0}=\frac{2\delta}{b-a}L_{[a,b]}''(0).
$$

The preceding curvature formula, with the base-speed factor $1/c$ when necessary, therefore evaluates the original full length derivative using any compact subinterval. No extension to the missing endpoints is required.

Differentiating $D_tT=0$ in $s$ yields the [Jacobi field](../../../../../jacobi-field.md) equation

$$
D_t^2J+\mathcal R(J,T)T=0.
$$

The same ruling [curves](../../../../../curve.md) are [geodesics](../../../../../geodesic.md) of the surface with its [induced metric](../../../../../induced-metric.md), because the tangential part of their ambient acceleration is zero. Write its [second fundamental form](../../../../../second-fundamental-form-split.md) as $II$ and its induced [Levi-Civita connection](../../../../../levi-civita-connection.md) as $D^N$. In particular $II(T,T)=0$. The scalar $f=\langle J,T\rangle$ satisfies $f''=0$, by the [Jacobi field](../../../../../jacobi-field.md) equation, so $W=J-fT$ is a [Jacobi field](../../../../../jacobi-field.md) both intrinsically and in the ambient manifold. In a regular surface chart $h=|W|>0$, and $E=W/h$ is the perpendicular unit tangent. Along a two-dimensional [geodesic](../../../../../geodesic.md), $D_t^NE=0$: its derivative is orthogonal to both $E$ and the parallel field $T$. The intrinsic [Jacobi field](../../../../../jacobi-field.md) equation consequently gives

$$
h''=-K_Nh.
$$

For the ambient derivative, the [Gauss formula](../../../../../gauss-formula.md) gives $D_tW=h'E+h\,II(T,E)$. Applying the same norm differentiation used above to $h=|W|$ gives

$$
hh''=|D_tW|^2-(h')^2-\langle\mathcal R(W,T)T,W\rangle
=h^2\bigl(\|II(T,E)\|^2-K_M(T,E)\bigr).
$$

Comparing these identities proves the [curvature comparison for a geodesically ruled surface](../../../../../curvature-comparison-for-a-geodesically-ruled-surface.md):

$$
\boxed{K_N=K_M(T,E)-\|II(T,E)\|^2\le K_M(T_pN).}
$$

This is also the [Gauss equation in a curved ambient manifold](../../../../../gauss-equation-in-a-curved-ambient-manifold.md) with $II(T,T)=0$. It applies locally to each regular patch of the surface.

For strict inequality, take the Euclidean [embedded submanifold](../../../../../embedded-submanifold.md) parametrized by $\phi(t,s)=(t,s,ts)$. Each $t$-curve is a straight-line [geodesic](../../../../../geodesic.md). Its [first fundamental form](../../../../../first-fundamental-form.md) has coefficients $E_0=1+s^2$, $F_0=st$, $G_0=1+t^2$; the normal $(-s,-t,1)/\sqrt{1+t^2+s^2}$ gives [second fundamental form](../../../../../second-fundamental-form-split.md) coefficients $e=0$, $f_0=1/\sqrt{1+t^2+s^2}$, $g_0=0$. Hence

$$
\boxed{K_N(t,s)=-\frac1{(1+t^2+s^2)^2}<0=K_{\mathbb R^3}.}
$$

Thus equality can fail everywhere, although every ruling is an ambient [geodesic](../../../../../geodesic.md).

The length differentiation requires a nonconstant base ruling; a regular parametrized surface patch guarantees this. If “image of a smooth map” is read literally without a rank assumption, a degenerate member can fail even to have a first length derivative. For example, in the flat cylinder $\mathbb R\times S^1$, the map $\phi(t,s)=(st,e^{is})$ for $|t|<\delta$, $|s|<4\pi$ has [geodesic](../../../../../geodesic.md) rulings and a two-dimensional open image: every nonzero-$s$ point has full-rank parametrization, and the sole zero-$s$ image point also has a full-rank preimage at $s=2\pi,t=0$. Yet $L(\gamma_s)=2\delta|s|$ is not differentiable at zero. The variation formula therefore applies to nonconstant members, as usual. The curvature inequality still holds on the whole image: regular values are dense by [Sard theorem](../../../../../sard-s-theorem.md), and both curvatures extend continuously to the remaining points.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
