<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**The harmonic equation, including critical points.** All derivatives in this argument use the three-dimensional [Levi-Civita connection](../../../../../levi-civita-connection.md) of $\gamma$. Write $U_i=\nabla_iU$, $|\nabla U|^2=\gamma^{ij}U_iU_j$ and $\Delta_\gamma U=\gamma^{ij}\nabla_i\nabla_jU$. The curvature relation for the [static vacuum conformal spatial metric](../../../../../static-vacuum-conformal-spatial-metric.md) gives $R=2|\nabla U|^2$. Substituting it into the [contracted Bianchi identity](../../../../../contracted-bianchi-identity.md) yields

$$
\nabla^iR_{ij}
=2(\Delta_\gamma U)U_j+2U^i\nabla_iU_j
=\frac12\nabla_jR
=2U^i\nabla_jU_i.
$$

The Hessian of a scalar is symmetric, so the last terms cancel:

$$
(\Delta_\gamma U)U_j=0.
$$

Where $\nabla U\ne0$, this implies $\Delta_\gamma U=0$. On the interior of the critical set $\{\nabla U=0\}$, $U$ is locally constant and its Laplacian is also zero. Every other critical point is a limit of noncritical points, so continuity of the Laplacian gives

$$
\boxed{\Delta_\gamma U=0\quad\text{everywhere}.}
$$

This avoids incorrectly dividing by a gradient at its zeros.

**Integration by parts and rigidity.** The usual whole-space energy identity is

$$
0=\int U\Delta_\gamma U\,dV_\gamma
=-\int|\nabla U|^2dV_\gamma+
\lim_{R\to\infty}\int_{S_R}U\,n^i\nabla_iU\,dS_\gamma.
$$

With standard static asymptotic falloff $U=O(R^{-1})$ and $\nabla U=O(R^{-2})$, the last term is $O(R^{-1})$ and vanishes. Positivity of the spatial [Riemannian metric](../../../../../riemannian-metric.md) then makes $U$ constant, and its limiting value fixes that constant to zero.

There is also a direct [integration by parts](../../../../../integration-by-parts.md) proof requiring only the stated vanishing of $U$ at infinity, rather than an assumed flux decay rate. For a regular value $\varepsilon>0$, the region $\Omega_\varepsilon=\{U>\varepsilon\}$ has compact closure. Completeness and the absence of an inner boundary ensure no missing boundary pieces; standard [asymptotic flatness](../../../../../asymptotically-flat-spacetime.md) and $U\to0$ on all ends keep this positive level set away from infinity. Its outward unit normal is $n=-\nabla U/|\nabla U|$. Multiplying the harmonic equation by $U$ and integrating gives

$$
0=-\int_{\Omega_\varepsilon}|\nabla U|^2dV_\gamma
-\varepsilon\int_{\partial\Omega_\varepsilon}|\nabla U|\,dS_\gamma.
$$

Both terms are nonpositive, so both vanish. A nonempty component with $U>\varepsilon$ cannot have zero gradient throughout and boundary value $\varepsilon$. Thus $\Omega_\varepsilon$ is empty. Choose arbitrarily small regular values and apply the same argument to $-U$; it follows that

$$
\boxed{U=0,\qquad R_{ij}(\gamma)=0.}
$$

This is [vanishing harmonic function by level-set integration](../../../../../vanishing-harmonic-function-by-level-set-integration.md). It also makes explicit why an inner boundary would invalidate the conclusion.

**From zero Ricci curvature to Minkowski spacetime.** In dimension three the [Schouten tensor](../../../../../schouten-tensor.md) is $S_{ij}=R_{ij}-R\gamma_{ij}/4$, so it vanishes here. The three-dimensional curvature reconstruction then gives $R_{ijpq}=0$: **$\gamma$ is a [flat Riemannian manifold](../../../../../flat-manifold.md).** This use of [three-dimensional curvature from the Ricci tensor](../../../../../three-dimensional-curvature-from-the-ricci-tensor.md) is essential; zero [Ricci tensor](../../../../../ricci-tensor.md) would not by itself imply flatness in four dimensions.

A complete connected flat spatial manifold has Euclidean universal cover. Standard [asymptotic flatness](../../../../../asymptotically-flat-spacetime.md), with an ordinary Euclidean end, excludes a nontrivial free Euclidean quotient: a nontrivial fixed-point-free Euclidean isometry contains a translational or screw component, and its cyclic quotient has at most quadratic volume growth, incompatible with a three-dimensional Euclidean end. Extra identifications cannot restore cubic growth. Thus the complete spatial metric is globally Euclidean, not just locally flat. With $U=0$ and the standard global time coordinate the four-metric becomes

$$
\boxed{ds^2=-dt^2+dx^2+dy^2+dz^2.}
$$

Therefore [horizonless static vacuum rigidity](../../../../../horizonless-static-vacuum-rigidity.md) gives **[Minkowski spacetime](../../../../../minkowski-spacetime.md) as the sole solution under these hypotheses.**

**Allowing horizons.** A [black hole](../../../../../black-hole.md) exterior can be static and asymptotically flat without being Minkowski. The [Schwarzschild spacetime](../../../../../schwarzschild-spacetime.md) is the basic example. Its [lapse function](../../../../../lapse-function.md) vanishes at the [event horizon](../../../../../event-horizon.md), so $U$ is unbounded below there; the horizon introduces an inner end or boundary in the spatial reduction, and the previous energy argument no longer has its hypotheses. In fact for Schwarzschild,

$$
U=\frac12\log(1-2M/r),\qquad
\gamma=dr^2+r(r-2M)d\Omega^2,
$$

so this conformal quotient terminates at $r=2M$ and is not the complete nonsingular quotient used above.

With the usual regularity, connected-horizon and global hypotheses of the static vacuum [black-hole uniqueness theorem](../../../../../black-hole-uniqueness-theorem.md), the nontrivial black-hole exterior is Schwarzschild. Rotating [Kerr black holes](../../../../../kerr-black-hole.md) are stationary but not static and therefore are not alternatives in this question. This statement concerns a regular domain outside the horizon; the Schwarzschild interior contains a curvature singularity. If “globally static” and “nonsingular everywhere” are retained literally, Schwarzschild does not meet them. Allowing horizons means relaxing the horizonless global hypotheses to the corresponding static exterior problem.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
