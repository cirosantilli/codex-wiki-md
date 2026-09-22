<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $E\to M$ have rank $r$. A [vector bundle covariant derivative](../../../../../connection-vector-bundle.md) is a real-linear operator

$$
\nabla:\Gamma(E)\longrightarrow\Omega^1(M;E),\qquad\boxed{\nabla(fs)=df\otimes s+f\nabla s.}
$$

Pairing its one-form slot with a [vector field](../../../../../vector-field.md) $X$ gives $\nabla_Xs$, with $\nabla_{fX}s=f\nabla_Xs$ and $\nabla_X(fs)=X(f)s+f\nabla_Xs$.

In the horizontal description, a [connection on a vector bundle](../../../../../connection-vector-bundle.md) $A$ is a smooth splitting $T_aE=V_aE\oplus H_aE$, where $V_aE=\ker(d\pi)_a$, and the horizontal choice is compatible with fibre addition and scalar multiplication. This linearity is essential; an arbitrary nonlinear horizontal splitting is not a vector-bundle connection. Identify a vertical vector at $a\in E_x$ with the element of $E_x$ obtained by differentiating the curve $a+tv$. Let $K_A:T_aE\to E_x$ be vertical projection followed by this identification. The induced [vector bundle covariant derivative](../../../../../connection-vector-bundle.md) is

$$
\boxed{\nabla_X^A s=K_A(ds(X)).}
$$

In a local [frame of a vector bundle](../../../../../frame-of-a-vector-bundle.md) $e=(e_1,\ldots,e_r)$, a linear horizontal splitting has the form

$$
H_{(x,v)}E=\{(\xi,-\Gamma_x(\xi)v):\xi\in T_xM\},\qquad K_A(\xi,w)=w+\Gamma_x(\xi)v,
$$

for a matrix-valued [connection one-form](../../../../../connection-one-form.md) $\Gamma$. Thus for $s=e v$, $\nabla^A s=e(dv+\Gamma v)$, which directly verifies the [Leibniz rule](../../../../../leibniz-rule.md).

Conversely, the [Leibniz rule](../../../../../leibniz-rule.md) makes $\nabla$ local: if a section vanishes near a point, multiply it by a [smooth cutoff function](../../../../../smooth-cutoff-function.md) supported in that neighborhood and equal to one near the point to see that its derivative vanishes there too. Local sections can therefore be differentiated by any extension agreeing near the point. Given $\nabla$, define its local [connection one-form](../../../../../connection-one-form.md) by $\nabla e_b=\sum_a e_a\Gamma^a_b$. The [Leibniz rule](../../../../../leibniz-rule.md) gives $\nabla(e v)=e(dv+\Gamma v)$. Under $e'=e g$, $v'=g^{-1}v$, one has

$$
\Gamma'=g^{-1}\Gamma g+g^{-1}dg.
$$

The tangent fibre coordinate transforms by $w'=g^{-1}w-g^{-1}(dg)(\xi)g^{-1}v$, so $w=-\Gamma(\xi)v$ transforms precisely to $w'=-\Gamma'(\xi)v'$. Consequently these local [horizontal subspaces of a vector bundle connection](../../../../../horizontal-subspace-of-a-vector-bundle-connection.md) glue to a smooth linear splitting inducing the given $\nabla$. Its local formula also shows uniqueness. This proves the [horizontal connection associated to a covariant derivative](../../../../../horizontal-connection-associated-to-a-covariant-derivative.md) construction.

A [horizontal lift](../../../../../horizontal-lift.md) $\widetilde\gamma$ of $\gamma$ is a smooth curve in $E$ with $\pi\circ\widetilde\gamma=\gamma$ and $\dot{\widetilde\gamma}(t)\in H_{\widetilde\gamma(t)}E$. In a local frame write $\widetilde\gamma(t)=e(\gamma(t))v(t)$. Horizontality is exactly the [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation.md)

$$
\boxed{\dot v(t)+\Gamma_{\gamma(t)}(\dot\gamma(t))v(t)=0.}
$$

We use existence and uniqueness for an ODE with smooth coefficients, and the continuation theorem that a solution extends across a finite interval when it remains bounded inside the coordinate domain. For a linear system $\dot v=-C(t)v$ with continuous coefficients bounded by $L$ on a compact time interval, the [Gronwall inequality](../../../../../gronwall-inequality.md) bounds $|v(t)|$ by its initial norm times $e^{L|t-t_0|}$, preventing finite-time fibre escape. Cover a compact subinterval of $I$ by finitely many bundle charts and partition it so each piece lies in one chart. Solve successively, changing fibre frames at the partition points. Coordinate invariance of the horizontal equation and uniqueness make the pieces agree. Exhausting $I$ by compact intervals containing $0$ produces **a unique horizontal lift on all of $I$ for every prescribed $a_0$**. This is [global continuation of linear parallel transport](../../../../../global-continuation-of-linear-parallel-transport.md).

The lift equation is linear in its initial value. Hence the endpoint map $P_\gamma:E_{\gamma(0)}\to E_{\gamma(1)}$ is linear. Solving the same equation backwards, or transporting along $t\mapsto\gamma(1-t)$, gives its inverse, so

$$
\boxed{P_\gamma\text{ is a linear isomorphism}.}
$$

This is [parallel transport](../../../../../parallel-transport.md). For two parallel lifts $s_1(t),s_2(t)$, the assumed [metric connection](../../../../../metric-connection.md) identity extends along the embedded curve and becomes

$$
\frac d{dt}\langle s_1(t),s_2(t)\rangle=\langle D_ts_1,s_2\rangle+\langle s_1,D_ts_2\rangle=0.
$$

Here $D_t$ is the [covariant derivative along a curve](../../../../../covariant-derivative-along-a-curve.md). The permitted extension of sections and the tangent vector along the embedded curve justifies applying the bundle identity; equivalently it follows in each local frame. Therefore

$$
\boxed{\langle P_\gamma a,P_\gamma b\rangle_{\gamma(1)}=\langle a,b\rangle_{\gamma(0)},}
$$

so **parallel transport is an isometry**. This is the principle that [parallel transport preserves a fibre metric](../../../../../parallel-transport-preserves-a-fibre-metric.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
