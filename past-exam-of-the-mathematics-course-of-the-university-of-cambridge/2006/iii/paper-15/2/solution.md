<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [Riemannian isometry](../../../../../riemannian-isometry.md) $F:(M,g)\to(N,h)$ is a [diffeomorphism](../../../../../diffeomorphism.md) satisfying $F^*h=g$. A [local isometry](../../../../../local-isometry.md) is a [local diffeomorphism](../../../../../local-diffeomorphism.md) with the same pullback identity; equivalently $dF_p$ is an isometric [linear isomorphism](../../../../../linear-isomorphism.md) for every $p$. An [isometric immersion](../../../../../isometric-immersion.md) into a higher-dimensional manifold does not satisfy this local-diffeomorphism requirement.

Let $\phi_t$ be the [local flow](../../../../../local-flow.md) of the generating [vector field](../../../../../vector-field.md) $K$. The identity $\phi_t^*g=g$ differentiates to $\mathcal L_Kg=0$, where $\mathcal L$ is the [Lie derivative of a tensor field](../../../../../lie-derivative-of-a-tensor-field.md). For arbitrary [vector fields](../../../../../vector-field.md) $X,Y$, [metric compatibility](../../../../../metric-compatibility.md) and the [torsion-free connection](../../../../../torsion-free-connection.md) give

$$
\begin{aligned}
(\mathcal L_Kg)(X,Y)
&=K\langle X,Y\rangle-\langle[K,X],Y\rangle-\langle X,[K,Y]\rangle\\
&=\langle\nabla_XK,Y\rangle+\langle\nabla_YK,X\rangle.
\end{aligned}
$$

This proves the [Killing equation](../../../../../killing-equation.md). Conversely, a smooth [Killing field](../../../../../killing-vector-field.md) has a [local flow](../../../../../local-flow.md), and

$$
\frac{d}{dt}\phi_t^*g=\phi_t^*(\mathcal L_Kg)=0.
$$

Since $\phi_0$ is the identity, $\phi_t^*g=g$ wherever the flow is defined. Its inverse is $\phi_{-t}$ locally, so **the [local flow](../../../../../local-flow.md) consists of [local isometries](../../../../../local-isometry.md)**. Neither direction assumes that $K$ is complete.

Put $H(X,Y)=\nabla_X(\nabla_YK)-\nabla_{\nabla_XY}K$ and $B(X,Y,Z)=\langle H(X,Y),Z\rangle$. These expressions are tensorial in $X,Y,Z$. Take the [covariant derivative](../../../../../covariant-derivative.md) in direction $X$ of the [Killing equation](../../../../../killing-equation.md), subtracting the terms from differentiating $Y$ and $Z$. It follows that

$$
\boxed{B(X,Y,Z)+B(X,Z,Y)=0.}
$$

With the curvature convention $\mathcal R$ of Solution 1, the [torsion-free connection](../../../../../torsion-free-connection.md) also gives

$$
H(X,Y)-H(Y,X)=\mathcal R(X,Y)K.
$$

Define $C(X,Y,Z)=\langle\mathcal R(X,K)Y,Z\rangle$. It is skew in $Y,Z$ by skew-adjointness of the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md). The [first Bianchi identity](../../../../../first-bianchi-identity.md) gives

$$
\mathcal R(X,K)Y-\mathcal R(Y,K)X=\mathcal R(X,Y)K,
$$

so $C$ has the same antisymmetrization in $X,Y$ as $B$. Consequently $D=B-C$ is symmetric in its first two slots and skew in its last two. These symmetries force it to vanish:

$$
D(X,Y,Z)=D(Y,X,Z)=-D(Y,Z,X)=-D(Z,Y,X)
=D(Z,X,Y)=D(X,Z,Y)=-D(X,Y,Z).
$$

We have proved the [second covariant derivative of a Killing vector](../../../../../second-covariant-derivative-of-a-killing-vector.md) identity, including its sign:

$$
\boxed{\nabla^2_{X,Y}K=\mathcal R(X,K)Y.}
$$

The printed identity uses the opposite [curvature-sign convention in Killing derivative identities](../../../../../curvature-sign-convention-in-killing-derivative-identities.md). If $R=-\mathcal R$, namely $R(X,Y)Z=\nabla_Y\nabla_XZ-\nabla_X\nabla_YZ+\nabla_{[X,Y]}Z$, the same result reads **$\nabla^2_{X,Y}K=R(K,X)Y$**, exactly as printed. The convention must change with the sign; under $\mathcal R$, writing $\mathcal R(K,X)Y$ would be incorrect.

Finally let $H_0=K-\widetilde K$ have zero value and zero first [covariant derivative](../../../../../covariant-derivative.md) at $p$. Along any [geodesic](../../../../../geodesic.md) issuing from $p$, the identity just proved says

$$
D_t^2H_0=\mathcal R(T,H_0)T=-\mathcal R(H_0,T)T.
$$

Thus $H_0$ is a [Jacobi field](../../../../../jacobi-field.md) with zero initial value and derivative. Uniqueness for this linear [ordinary differential equation](../../../../../ordinary-differential-equation.md) implies $H_0=0$ on each such [geodesic](../../../../../geodesic.md), hence on a [convex normal neighborhood](../../../../../convex-normal-neighbourhood.md) of $p$. Consider the set of points where both $H_0$ and $\nabla H_0$ vanish. It is closed by continuity and open by this same local argument; on the resulting neighborhood $H_0$ vanishes identically, so its derivative does too. It is nonempty, and $M$ is [connected](../../../../../connected-space.md), therefore it is all of $M$. This proves **$K=\widetilde K$ everywhere** and the general statement that a [Killing field is determined by its value and first covariant derivative](../../../../../killing-field-is-determined-by-its-value-and-first-covariant-derivative.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
