<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The paper uses $T_{\mu\nu}{}^\lambda=\Gamma_{\nu\mu}{}^\lambda-\Gamma_{\mu\nu}{}^\lambda$, the negative of a common [torsion tensor](../../../torsion-tensor.md) convention. Keep that sign throughout. Also, $\nabla_\mu\nabla_\nu\varphi$ denotes the covariant [Hessian](../../../hessian-matrix.md), so the second derivative acts on the lower index $\nu$ of the [covector](../../../covector.md) $\nabla_\nu\varphi$; it is not just a composition of two directional derivatives on a scalar.

Since the [covariant derivative](../../../covariant-derivative.md) of a [scalar field](../../../scalar-field.md) is its ordinary derivative,

$$
\nabla_\mu\nabla_\nu\varphi
=\partial_\mu\partial_\nu\varphi-\Gamma_{\mu\nu}{}^\lambda\partial_\lambda\varphi.
$$

Commuting the ordinary partial derivatives therefore gives

$$
\boxed{(\nabla_\mu\nabla_\nu-\nabla_\nu\nabla_\mu)\varphi
=T_{\mu\nu}{}^\lambda\nabla_\lambda\varphi.}
$$

For a [vector field](../../../vector-field.md), write $D_\nu X^\lambda=\partial_\nu X^\lambda+\Gamma_{\nu\rho}{}^\lambda X^\rho$. This is a [tensor](../../../tensor.md) with one covariant and one contravariant index. Hence

$$
\nabla_\mu\nabla_\nu X^\lambda
=\partial_\mu(D_\nu X^\lambda)+\Gamma_{\mu\sigma}{}^\lambda D_\nu X^\sigma
-\Gamma_{\mu\nu}{}^\sigma D_\sigma X^\lambda.
$$

Subtracting the expression with $\mu,\nu$ exchanged, the first two terms combine to

$$
\left(\partial_\mu\Gamma_{\nu\rho}{}^\lambda
-\partial_\nu\Gamma_{\mu\rho}{}^\lambda
+\Gamma_{\mu\sigma}{}^\lambda\Gamma_{\nu\rho}{}^\sigma
-\Gamma_{\nu\sigma}{}^\lambda\Gamma_{\mu\rho}{}^\sigma\right)X^\rho.
$$

The coefficients of first derivatives of $X$ in those two terms cancel. The last terms give $(\Gamma_{\nu\mu}{}^\sigma-\Gamma_{\mu\nu}{}^\sigma)D_\sigma X^\lambda$. Identifying the [curvature](../../../curvature.md) coefficient yields

$$
\boxed{[\nabla_\mu,\nabla_\nu]X^\lambda
=R_{\mu\nu\rho}{}^\lambda X^\rho
+T_{\mu\nu}{}^\rho\nabla_\rho X^\lambda.}
$$

Here the bracket denotes antisymmetrization of the [tensorial](../../../tensoriality.md) second [covariant derivative](../../../covariant-derivative.md), consistently with the preceding calculation.

To check tensoriality directly, antisymmetrize the supplied transformation law of the [connection coefficients](../../../connection-components.md) in the two lower indices. The inhomogeneous term vanishes because mixed coordinate second derivatives are symmetric. The remaining transformation law is

$$
T_{\nu\lambda}{}^\mu
=\frac{\partial x^\mu}{\partial x^{\mu'}}
\frac{\partial x^{\nu'}}{\partial x^\nu}
\frac{\partial x^{\lambda'}}{\partial x^\lambda}
T_{\nu'\lambda'}{}^{\mu'},
$$

which is precisely that of a $(1,2)$ [tensor](../../../tensor.md). Intrinsically, with the paper's sign,

$$
\boxed{T(X,Y)=\nabla_YX-\nabla_XY+[X,Y].}
$$

The derivative terms involving the components of $X,Y$ cancel against their [Lie bracket](../../../lie-bracket.md), leaving $(\Gamma_{\nu\mu}{}^\lambda-\Gamma_{\mu\nu}{}^\lambda)X^\mu Y^\nu$. This also shows that the expression is linear over smooth functions in each argument.

Finally take the [torsion-free connection](../../../torsion-free-connection.md) and the commuting parameter fields $Y,Z$ along the [geodesic](../../../geodesic.md) family. Vanishing torsion gives $\nabla_YZ=\nabla_ZY$, while affine [geodesic](../../../geodesic.md) parametrization gives $\nabla_YY=0$. The [curvature](../../../curvature.md) operator in the specified convention is

$$
R(Y,Z)W=\nabla_Y\nabla_ZW-\nabla_Z\nabla_YW-\nabla_{[Y,Z]}W.
$$

Therefore

$$
\nabla_Y\nabla_YZ
=\nabla_Y\nabla_ZY
=R(Y,Z)Y+\nabla_Z\nabla_YY+\nabla_{[Y,Z]}Y
=R(Y,Z)Y.
$$

In components this is the [geodesic deviation](../../../geodesic-deviation.md) equation

$$
\boxed{\frac{D^2Z^\mu}{d\tau^2}
=R_{\nu\lambda\rho}{}^\mu Y^\nu Z^\lambda Y^\rho.}
$$

The connecting field represents infinitesimal separation within the family, so this is a linear equation for relative free-fall acceleration, rather than an exact coordinate difference for widely separated worldlines.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2011](../../2011-split.md)
3. [Past exam of the general relativity course of the University of Oxford](../../split.md)
4. [General relativity course of the University of Oxford](../../../general-relativity-course-of-the-university-of-oxford.md)
5. [Year 3 of the physics course of the University of Oxford](../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
