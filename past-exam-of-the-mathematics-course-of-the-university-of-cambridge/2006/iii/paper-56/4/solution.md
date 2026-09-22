<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

On [complexified Minkowski spacetime](../../../../../complexified-minkowski-spacetime.md), use the [twistor incidence relation](../../../../../twistor-incidence-relation.md)

$$
\boxed{\omega^A=ix^{AA'}\pi_{A'},\qquad \pi\ne0.}
$$

The harmless factor $i$ is a conventional choice; omitting it corresponds to rescaling the complexified coordinates. For fixed $x$, projectivizing the nonzero [two-component spinors](../../../../../two-component-spinor.md) $\pi$ gives a [twistor line](../../../../../twistor-line.md) $L_x\simeq\mathbb{CP}^1$. The two stated patches cover all these incidence lines; they describe the affine-space-time twistor domain with the line $\pi=0$ removed from full [projective twistor space](../../../../../projective-twistor-space.md).

Since $E|_{L_x}$ is holomorphically trivial, choose a global [bundle frame](../../../../../frame-of-a-vector-bundle.md) on that line. Comparing its columns with the [bundle frames](../../../../../frame-of-a-vector-bundle.md) in the two patch trivializations gives invertible [matrices](../../../../../matrix.md) $H(x,\pi)$ and $\widetilde H(x,\pi)$, holomorphic on their respective patches, with

$$
\boxed{F(ix\pi,\pi)=\widetilde H(x,\pi)H(x,\pi)^{-1}.}
$$

This is the [holomorphic splitting of a twistor patching matrix](../../../../../holomorphic-splitting-of-a-twistor-patching-matrix.md). It follows directly from existence of the global [bundle frame](../../../../../frame-of-a-vector-bundle.md), rather than from an arbitrary factorization of an arbitrary [matrix](../../../../../matrix.md): nontrivial line bundles would obstruct such a nonsingular splitting.

The factors can be chosen holomorphically in $x$ near any given $x_0$. An explicit local argument is useful. Normalize the known splitting at $x_0$ and set $Q(x,\lambda)=\widetilde H(x_0,\lambda)^{-1}F(x,\lambda)H(x_0,\lambda)$ on a fixed circular contour in the overlap. It is close to the identity when $x$ is close to $x_0$. Let $P_+$ select strictly positive Laurent powers, and seek $q=1+$ positive powers satisfying

$$
q=1-P_+[(Q-1)q].
$$

In a holomorphic contour-function norm the operator has norm below one for sufficiently small variation, so its [Neumann series](../../../../../neumann-series.md) converges and is holomorphic in $x$. Then $Qq=\widetilde q$ has only nonpositive powers and is holomorphic on the exterior patch including infinity. Both factors are close to the identity and invertible. They extend over their full patches through $Q$ and its inverse. Taking $H=H(x_0)q$ and $\widetilde H=\widetilde H(x_0)\widetilde q$ gives the required local family. This is also the elementary [Laurent series](../../../../../laurent-series.md) reason that $H^1(\mathbb{CP}^1,\mathcal O)=0$ leaves no infinitesimal obstruction.

Raise primed [two-component spinor](../../../../../two-component-spinor.md) indices with the antisymmetric [two-component spinor](../../../../../two-component-spinor.md) form and define $V_A=\pi^{A'}\partial_{AA'}$, holding $\pi$ fixed. Incidence gives

$$
V_A\omega^B=i\delta_A^B\pi^{A'}\pi_{A'}=0,\qquad V_A\pi_{B'}=0.
$$

Thus $V_AF=0$ for a pulled-back [function](../../../../../function-split.md) depending only on twistor coordinates. Differentiating the splitting and multiplying by the inverse factors gives

$$
H^{-1}V_AH=\widetilde H^{-1}V_A\widetilde H.
$$

The left expression is holomorphic on one [two-component spinor](../../../../../two-component-spinor.md) patch, the right on the other, and each is homogeneous of degree one in $\pi$. They therefore glue to a global matrix-valued section of $\mathcal O(1)$ on the line.

Such a section is linear in its homogeneous coordinates. To see this explicitly, set $\lambda=\pi_{0'}/\pi_{1'}$ on $U$. The normalized expression is an entire [matrix](../../../../../matrix.md) [function](../../../../../function-split.md) of $\lambda$; on the other patch its quotient by $\lambda$ is holomorphic at infinity. Hence it has at most linear growth. [Cauchy estimates](../../../../../cauchy-estimate.md) force all its [derivatives](../../../../../derivative.md) of order at least two to vanish. Entry by entry it is $a_A(x)+\lambda b_A(x)$, or invariantly

$$
\boxed{\pi^{A'}\Phi_{AA'}(x)=H^{-1}\pi^{A'}\partial_{AA'}H.}
$$

The coefficients are holomorphic in $x$. This proves existence of the desired space-time one-form, with no remaining dependence on $\pi$ in its coefficients.

A second splitting must differ by right multiplication $H\mapsto Hg(x)$ and $\widetilde H\mapsto\widetilde Hg(x)$. Indeed the comparison [matrix](../../../../../matrix.md) is holomorphic on both patches of a compact [complex projective line](../../../../../complex-projective-line.md) and therefore constant along the line. The resulting transformation is

$$
\Phi\longmapsto g^{-1}\Phi g+g^{-1}dg,
$$

the [gauge connection](../../../../../connection-vector-bundle.md) transformation law. Local coefficient [matrices](../../../../../matrix.md) consequently glue to a holomorphic [gauge connection](../../../../../connection-vector-bundle.md) on the bundle whose fiber at $x$ is the space of [holomorphic sections](../../../../../holomorphic-section.md) of $E|_{L_x}$. If a single global matrix-valued one-form is wanted on all $M_{\mathbb C}\simeq\mathbb C^4$, choose a basis at the origin and parallel-transport it along the straight radial paths to each $x$. Linear transport exists on every finite path and varies holomorphically with $x$; this gives a global holomorphic [bundle frame](../../../../../frame-of-a-vector-bundle.md). The assertion does not require [flat connection](../../../../../flat-connection.md) in all four directions, only a fixed choice of paths for a trivialization. On more general space-time domains the intrinsic object is a [gauge connection](../../../../../connection-vector-bundle.md) with these gauge-related local one-forms.

Finally put $D_{AA'}=\partial_{AA'}+\Phi_{AA'}$ and $\mathcal D_A(\pi)=\pi^{A'}D_{AA'}$. From the defining identity,

$$
\mathcal D_A(\pi)H^{-1}
=-H^{-1}(V_AH)H^{-1}+(H^{-1}V_AH)H^{-1}=0.
$$

Thus the columns of $H^{-1}$ are an invertible parallel [bundle frame](../../../../../frame-of-a-vector-bundle.md) in the two [alpha-plane](../../../../../alpha-plane.md) directions. Their [matrix commutator](../../../../../commutator.md) must annihilate that [bundle frame](../../../../../frame-of-a-vector-bundle.md), so

$$
\pi^{A'}\pi^{B'}F_{AA'BB'}=0\qquad\text{for every }\pi.
$$

Use the [spinor decomposition of gauge curvature](../../../../../spinor-decomposition-of-gauge-curvature.md)

$$
F_{AA'BB'}=\epsilon_{AB}\varphi_{A'B'}+\epsilon_{A'B'}\varphi_{AB},
$$

where both [gauge curvature](../../../../../gauge-field-strength.md) [two-component spinors](../../../../../two-component-spinor.md) are symmetric. The second term vanishes under contraction with $\pi^{A'}\pi^{B'}$. The first is a quadratic polynomial in the two [two-component spinor](../../../../../two-component-spinor.md) components; vanishing for every [two-component spinor](../../../../../two-component-spinor.md) forces each of its coefficients to vanish. Therefore

$$
\boxed{\varphi_{A'B'}=0,}
$$

which is precisely the [ASDYM](../../../../../anti-self-dual-yang-mills-equations.md) equation in the convention where the primed symmetric [two-component spinor](../../../../../two-component-spinor.md) is the self-dual part. Equivalently, the [gauge connection](../../../../../connection-vector-bundle.md) is flat when restricted to every [alpha-plane](../../../../../alpha-plane.md). This completes the forward [Penrose-Ward correspondence](../../../../../penrose-ward-correspondence.md), including both the existence of the [gauge connection](../../../../../connection-vector-bundle.md) and its [anti-self-duality of gauge curvature](../../../../../anti-self-duality-of-gauge-curvature.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
