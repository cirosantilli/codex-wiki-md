# Paper 68

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper68.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper68.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 68](paper-68.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

An [affine connection](../../../fiber-bundle.md#affine-connection) on the [tangent bundle](../../../fiber-bundle.md#tangent-bundle) of a [smooth manifold](../../../differential-geometry.md#smooth-manifold) assigns a [vector field](../../../calculus.md#vector-field) $\nabla_XY$ to two [vector fields](../../../calculus.md#vector-field), is $\mathbb R$-bilinear, and satisfies

$$
\nabla_{fX}Y=f\nabla_XY,\qquad
\nabla_X(fY)=X(f)Y+f\nabla_XY.
$$

Thus its first slot is [tensorial](../../../fiber-bundle.md#tensoriality) and its second obeys the [Leibniz rule](../../../calculus.md#leibniz-rule). Its action on [covectors](../../../linear-algebra.md#covector) is defined by differentiating the pairing, and this extends it to [tensor fields](../../../fiber-bundle.md#tensor-field). A [torsion-free connection](../../../fiber-bundle.md#torsion-free-connection) has $\nabla_XY-\nabla_YX=[X,Y]$.

Assume that $g$ is a smooth [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form) [metric tensor](../../../general-relativity.md#metric-tensor). [Metric compatibility](../../../fiber-bundle.md#metric-compatibility) and a vanishing [torsion tensor](../../../fiber-bundle.md#torsion-tensor) imply the [Koszul formula](../../../fiber-bundle.md#koszul-formula),

$$
2g(\nabla_XY,Z)=Xg(Y,Z)+Yg(Z,X)-Zg(X,Y)
-g(X,[Y,Z])+g(Y,[Z,X])+g(Z,[X,Y]).
$$

The right-hand side is determined by $g$ and the [Lie bracket of vector fields](../../../differential-geometry.md#lie-bracket-of-vector-fields). Nondegeneracy determines $\nabla_XY$ uniquely; conversely this formula defines an [affine connection](../../../fiber-bundle.md#affine-connection) with both required properties, proving existence as well as uniqueness. In a [coordinate frame](../../../differential-geometry.md#coordinate-basis) the brackets vanish. Combining the three differentiated [metric tensor](../../../general-relativity.md#metric-tensor) identities gives

$$
\boxed{\Gamma^a{}_{bc}
=\frac12g^{ad}(\partial_bg_{dc}+\partial_cg_{db}-\partial_dg_{bc}).}
$$

This is the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection). Positive definiteness is unnecessary: the argument also works for a [pseudo-Riemannian metric](../../../differential-geometry.md#pseudo-riemannian-metric).

For the other [affine connection](../../../fiber-bundle.md#affine-connection) define $S(X,Y)=\bar\nabla_XY-\nabla_XY$. The [derivative](../../../calculus.md#derivative) of $f$ cancels between the two [Leibniz rules](../../../calculus.md#leibniz-rule), so $S$ is $C^\infty$-linear in both slots. The [difference of affine connections is a tensor](../../../fiber-bundle.md#difference-of-affine-connections-is-a-tensor): here $S$ is a section of $TM\otimes T^*M\otimes T^*M$ with components $\bar\Gamma^a{}_{bc}-\Gamma^a{}_{bc}$. Both [affine connections](../../../fiber-bundle.md#affine-connection) are [torsion-free](../../../fiber-bundle.md#torsion-free-connection), so $S(X,Y)=S(Y,X)$.

Agreement of [geodesics](../../../riemannian-geometry.md#geodesic) means agreement of their unparametrized curves; different [affine parameters](../../../riemannian-geometry.md#affine-parameter) are allowed. For every nonzero tangent vector $v$, existence of a [geodesic](../../../riemannian-geometry.md#geodesic) with that initial velocity implies that $S(v,v)$ is parallel to $v$. The [symmetric bilinear diagonal-parallel lemma](../../../linear-algebra.md#symmetric-bilinear-diagonal-parallel-lemma) now determines $S$. Choose a [basis](../../../vector-space.md#basis) $e_i$ and write $S(e_i,e_i)=\alpha_i e_i$. Applying the parallelism condition to $e_i+e_j$ and $e_i-e_j$ gives

$$
S(e_i,e_j)=\frac12\alpha_j e_i+\frac12\alpha_i e_j.
$$

With $V(e_i)=\alpha_i/2$, [bilinearity](../../../linear-algebra.md#bilinearity) yields

$$
\boxed{S^a{}_{bc}=\delta^a_bV_c+\delta^a_cV_b
=2\delta^a{}_{(b}V_{c)},\qquad
V_c=\frac{S^a{}_{ac}}{n+1},\quad n=\dim M.}
$$

This is [projective equivalence of affine connections](../../../fiber-bundle.md#projective-equivalence-of-affine-connections). It also covers dimension one. For two [Levi-Civita connections](../../../general-relativity.md#levi-civita-connection), the [projective covector from metric volume densities](../../../fiber-bundle.md#projective-covector-from-metric-volume-densities) gives the explicit answer

$$
\boxed{V_c=\frac{1}{2(n+1)}
\partial_c\log\left|\frac{\det\bar g}{\det g}\right|.}
$$

Indeed $\Gamma^a{}_{ac}=\partial_c\log\sqrt{|\det g|}$. The [determinant](../../../linear-algebra.md#determinant) ratio is a [scalar](../../../vector-space.md#scalar), so this expression is a genuine [covector](../../../linear-algebra.md#covector), although either [determinant](../../../linear-algebra.md#determinant) alone is coordinate-dependent. This [determinant](../../../linear-algebra.md#determinant) expression requires nondegeneracy of $\bar g$; the difference-tensor and earlier [trace](../../../linear-algebra.md#matrix-trace) formula require only the two torsion-free [affine connections](../../../fiber-bundle.md#affine-connection).

Conversely, the displayed [tensor](../../../linear-algebra.md#tensor) gives $\bar\nabla_{\dot\gamma}\dot\gamma=2V(\dot\gamma)\dot\gamma$ along an affinely parametrized $\nabla$-[geodesic](../../../riemannian-geometry.md#geodesic). Choosing a new parameter $t(\tau)$ satisfying $t''/t'=2V(\dot\gamma)$ removes that tangential acceleration. This [geodesic reparametrization under projective equivalence](../../../fiber-bundle.md#geodesic-reparametrization-under-projective-equivalence) proves sufficiency. If agreement were required with the very same [affine parameter](../../../riemannian-geometry.md#affine-parameter), polarization would instead force $S=0$ and $V=0$.

## 2

↑ **Parent:** [Paper 68](paper-68.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Use $c=1$, background [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime) [metric tensor](../../../general-relativity.md#metric-tensor) $\eta_{ab}=\operatorname{diag}(1,-1,-1,-1)$, and $g_{ab}=\eta_{ab}+h_{ab}$ with small [metric perturbation](../../../general-relativity.md#linearized-gravity). All indices and [derivatives](../../../calculus.md#derivative) in this [linear](../../../vector-space.md#linearity) approximation use $\eta$. The [linearized inverse metric](../../../general-relativity.md#linearized-inverse-metric) is $\eta^{ab}-h^{ab}$, and the [linearized Levi-Civita connection](../../../general-relativity.md#linearized-levi-civita-connection) is

$$
\Gamma^a{}_{bc}=\frac12\eta^{ad}
(\partial_bh_{cd}+\partial_ch_{bd}-\partial_dh_{bc}).
$$

Define the [trace-reversed metric perturbation](../../../general-relativity.md#trace-reversed-metric-perturbation) $\bar h_{ab}=h_{ab}-\eta_{ab}h/2$, with $h=\eta^{ab}h_{ab}$.

An infinitesimal coordinate change $x'^a=x^a+\xi^a$ gives the [linearized coordinate gauge transformation](../../../general-relativity.md#linearized-coordinate-gauge-transformation)

$$
h'_{ab}=h_{ab}-\partial_a\xi_b-\partial_b\xi_a,\qquad
\bar h'_{ab}=\bar h_{ab}-\partial_a\xi_b-\partial_b\xi_a
+\eta_{ab}\partial_c\xi^c.
$$

The [metric perturbation](../../../general-relativity.md#linearized-gravity) therefore has redundant components. The [gauge invariance of the linearized Riemann tensor](../../../general-relativity.md#gauge-invariance-of-the-linearized-riemann-tensor) follows because its change contains third [derivatives](../../../calculus.md#derivative) of $\xi$ cancelling by commutation of [partial derivatives](../../../calculus.md#partial-derivative). Conversely, [flat linearized metric perturbations are locally pure gauge](../../../general-relativity.md#flat-linearized-metric-perturbations-are-locally-pure-gauge) on a [contractible](../../../algebraic-topology.md#contractible-space) patch. Thus linearized [curvature](../../../differential-geometry.md#curvature), rather than a particular coordinate value of $h$, detects the physical disturbance. Gauge freedom can also be restricted by global [topology](../../../topology.md) or [boundary conditions](../../../differential-equation.md#boundary-condition).

Keeping the paper's [curvature sign convention](../../../general-relativity.md#curvature-sign-convention), its [linearized Ricci tensor and scalar](../../../general-relativity.md#linearized-ricci-tensor-and-scalar) are

$$
R^{(1)}_{ab}=\frac12\left[
\Box h_{ab}+\partial_a\partial_bh
-\partial_a\partial^ch_{bc}-\partial_b\partial^ch_{ac}\right],
\qquad R^{(1)}=\Box h-\partial_a\partial_bh^{ab}.
$$

These are the negatives of the alternative frequently used [curvature](../../../differential-geometry.md#curvature) convention. Put $v_b=\partial^a\bar h_{ab}$. The [Linearized Einstein equations](../../../general-relativity.md#linearized-einstein-equations) in vacuum are

$$
G^{(1)}_{ab}=\frac12\left[
\Box\bar h_{ab}-\partial_av_b-\partial_bv_a
+\eta_{ab}\partial^cv_c\right]=0,\qquad
\Box=\partial_t^2-\nabla^2.
$$

Under a gauge change $v_b\mapsto v_b-\Box\xi_b$, so solving $\Box\xi_b=v_b$ imposes the [Lorenz gauge in linearized gravity](../../../general-relativity.md#lorenz-gauge-in-linearized-gravity). The field equations then become $\Box\bar h_{ab}=0$. The remaining [residual gauge symmetry of linearized gravity](../../../general-relativity.md#residual-gauge-symmetry-of-linearized-gravity) has $\Box\xi_b=0$; Lorenz gauge does not exhaust the coordinate freedom.

A [Fourier mode](../../../fourier-analysis.md#fourier-mode) $\bar h_{ab}=A_{ab}e^{ik_cx^c}$ obeys $k^ak_a=0$ and $k^aA_{ab}=0$. Hence the [plane gravitational waves in linearized gravity](../../../general-relativity.md#plane-gravitational-wave-in-linearized-gravity) propagate on the background [light cones](../../../special-relativity.md#light-cone). Four transversality conditions and four residual gauge amplitudes leave $10-4-4=2$ physical degrees of freedom. The [explicit plane-wave reduction to transverse-traceless gauge](../../../general-relativity.md#explicit-plane-wave-reduction-to-transverse-traceless-gauge) can set $h_{0a}=0$, spatial [trace](../../../linear-algebra.md#matrix-trace) zero and $k^ih_{ij}=0$. For a wave in the $z$ direction, write its physical spatial strain as $H_{ij}=-h_{ij}$, so the spatial [metric tensor](../../../general-relativity.md#metric-tensor) is $-(\delta_{ij}+H_{ij})$:

$$
H_{ij}(t-z)=
\begin{pmatrix}
H_+&H_\times&0\\
H_\times&-H_+&0\\
0&0&0
\end{pmatrix}.
$$

There are **two [gravitational wave polarizations](../../../general-relativity.md#gravitational-wave-polarization)**, [plus polarization](../../../general-relativity.md#plus-polarization) and [cross polarization](../../../general-relativity.md#cross-polarization). Rotating transverse axes through $\theta$ rotates their amplitude pair through $2\theta$. Nonconstant profiles with nonzero second [derivative](../../../calculus.md#derivative) have nonzero linearized [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) and cannot be removed as pure gauge.

The [TT coordinate separation and measured separation](../../../general-relativity.md#tt-coordinate-separation-and-measured-separation) distinction explains a detector's response. Freely falling particles initially at rest can keep fixed TT coordinates, since $\Gamma^a{}_{00}=0$, while their proper separation changes. For a short arm along a unit vector $n$,

$$
\frac{\delta L}{L}=\frac12H_{ij}n^in^j,\qquad
\frac{d^2\delta L}{dt^2}=\frac12\ddot H_{ij}n^in^jL.
$$

This is the tidal response described by [geodesic deviation](../../../general-relativity.md#geodesic-deviation); coordinate motion by itself is not the measured signal.

Finally, gravitational-wave energy is second order in the perturbation, so it is absent from a first-order vacuum equation. In a short-wavelength averaging regime the [averaged stress-energy of transverse gravitational waves](../../../general-relativity.md#averaged-stress-energy-of-transverse-gravitational-waves) is

$$
t^{\rm GW}_{ab}=\frac{1}{32\pi G}
\left\langle\partial_aH_{ij}\partial_bH_{ij}\right\rangle.
$$

For a plane wave its [energy flux](../../../physics.md#energy-flux) is $(16\pi G)^{-1}\langle\dot H_+^2+\dot H_\times^2\rangle$. The averaging scale and weak-field assumptions matter: this does not assign a coordinate-independent local gravitational [energy density](../../../statistical-physics.md#energy-density) to an arbitrary first-order perturbation.

## 3

↑ **Parent:** [Paper 68](paper-68.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The [Brans-Dicke theory](../../../general-relativity.md#brans-dicke-theory) couples a [scalar field](../../../quantum-field-theory.md#scalar-field) $\Phi$ to the [Ricci scalar](../../../general-relativity.md#ricci-scalar). Assume $\Phi\ne0$, constant $\omega$, matter independent of $\Phi$, and variations of compact support so [boundary terms](../../../calculus.md#boundary-term) may be discarded. Use the paper's [curvature sign convention](../../../general-relativity.md#curvature-sign-convention) and signature $(+---)$. Set $X=g^{ab}\partial_a\Phi\,\partial_b\Phi$ and $\Box\Phi=\nabla_a\nabla^a\Phi$. Define the [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor) consistently by

$$
\delta S_m=\frac12\int\sqrt{-g}\,T_{ab}\,\delta g^{ab}\,d^4x
=-\frac12\int\sqrt{-g}\,T^{ab}\,\delta g_{ab}\,d^4x.
$$

This convention fixes the sign of the matter term.

Vary with respect to $g^{ab}$. The [variation of metric volume density](../../../general-relativity.md#variation-of-metric-volume-density) contributes $-g_{ab}/2$ times each [scalar](../../../vector-space.md#scalar) Lagrangian, while $\delta R=R_{ab}\delta g^{ab}+g^{ab}\delta R_{ab}$. Applying the [Palatini identity](../../../general-relativity.md#palatini-identity) followed by two rounds of [integration by parts](../../../calculus.md#integration-by-parts) gives the [metric variation of a scalar-curvature coupling](../../../general-relativity.md#metric-variation-of-a-scalar-curvature-coupling),

$$
\delta\int\sqrt{-g}\,\Phi R\,d^4x
=\int\sqrt{-g}\left[
\Phi G_{ab}+\nabla_a\nabla_b\Phi-g_{ab}\Box\Phi
\right]\delta g^{ab}\,d^4x.
$$

The differentiated $\Phi$ terms remain because the [curvature](../../../differential-geometry.md#curvature) multiplier is not constant. Varying the kinetic term at fixed $\Phi$ gives

$$
\delta\int\sqrt{-g}\,\omega\Phi^{-1}X\,d^4x
=\int\sqrt{-g}\,\omega\Phi^{-1}
\left(\partial_a\Phi\,\partial_b\Phi-\frac12g_{ab}X\right)
\delta g^{ab}\,d^4x.
$$

Combining these terms with the matter variation, the [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) is

$$
\boxed{\Phi G_{ab}+\nabla_a\nabla_b\Phi-g_{ab}\Box\Phi
+\omega\Phi^{-1}
\left(\partial_a\Phi\,\partial_b\Phi-\frac12g_{ab}X\right)
=-8\pi G T_{ab}.}
$$

Raising both free indices reproduces the contravariant form, because $\nabla_ag_{bc}=0$.

The independent [scalar](../../../vector-space.md#scalar) variation gives

$$
R-\omega\Phi^{-2}X
-2\omega\nabla_a(\Phi^{-1}\nabla^a\Phi)=0,
$$

or $R+\omega\Phi^{-2}X-2\omega\Phi^{-1}\Box\Phi=0$. The [trace](../../../linear-algebra.md#matrix-trace) of the [metric tensor](../../../general-relativity.md#metric-tensor) equation in four dimensions is

$$
-\Phi R-3\Box\Phi-\omega\Phi^{-1}X=-8\pi G T,
\qquad T=g^{ab}T_{ab}.
$$

Multiplying the [scalar](../../../vector-space.md#scalar) equation by $\Phi$ eliminates the same combination $\Phi R+\omega\Phi^{-1}X$. Thus the [scalar equation of Brans-Dicke theory](../../../general-relativity.md#scalar-equation-of-brans-dicke-theory) is

$$
\boxed{(3+2\omega)\Box\Phi=8\pi G T,\qquad
\Box\Phi=\frac{8\pi G}{3+2\omega}\,g_{ab}T^{ab}
\quad(\omega\ne-3/2).}
$$

At the [degenerate coupling of Brans-Dicke theory](../../../general-relativity.md#degenerate-coupling-of-brans-dicke-theory), $\omega=-3/2$, the combined equations impose $T=0$ instead; division by $3+2\omega$ is unavailable. If matter depended directly on $\Phi$, its [scalar](../../../vector-space.md#scalar) variation would add a source and the displayed [scalar](../../../vector-space.md#scalar) equation would change.

The following lettered sections justify the supplied variation identities; they are supporting identities in the PDF, rather than three independent field-equation problems.

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Differentiate $g^{ac}g_{cb}=\delta^a_b$ while holding the coordinate system fixed. The [variation of inverse metric](../../../general-relativity.md#variation-of-inverse-metric) obeys

$$
(\delta g^{ac})g_{cb}+g^{ac}\delta g_{cb}=0.
$$

Multiplication by the inverse [metric tensor](../../../general-relativity.md#metric-tensor) gives

$$
\boxed{\delta g^{cd}=-g^{ca}g^{db}\delta g_{ab}.}
$$

This is the [matrix](../../../vector-space.md#matrix) inverse [derivative](../../../calculus.md#derivative) written with [tensor](../../../linear-algebra.md#tensor) indices. A variation of the [metric tensor](../../../general-relativity.md#metric-tensor) is symmetric, so the right-hand side is symmetric in $c,d$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Write $g=\det(g_{ab})$. The [Jacobi formula](../../../linear-algebra.md#jacobi-s-formula) gives $\delta g=g\,g^{ab}\delta g_{ab}$. Since a [Lorentzian metric](../../../general-relativity.md#lorentzian-metric) of signature $(+---)$ has negative [determinant](../../../linear-algebra.md#determinant),

$$
\boxed{\delta\sqrt{-g}
=\frac12\sqrt{-g}\,g^{ab}\delta g_{ab}.}
$$

The [variation of metric volume density](../../../general-relativity.md#variation-of-metric-volume-density) therefore has the opposite sign when expressed using the inverse [metric tensor](../../../general-relativity.md#metric-tensor): $\delta\sqrt{-g}=-\sqrt{-g}\,g_{ab}\delta g^{ab}/2$. This follows immediately from the [variation of inverse metric](../../../general-relativity.md#variation-of-inverse-metric) and explains the volume term in the field-equation derivation.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Although [connection coefficients](../../../fiber-bundle.md#connection-components) are not [tensor](../../../linear-algebra.md#tensor) components, their variation $C^a{}_{bc}=\delta\Gamma^a{}_{bc}$ is [tensorial](../../../fiber-bundle.md#tensoriality): the [difference of affine connections is a tensor](../../../fiber-bundle.md#difference-of-affine-connections-is-a-tensor). Varying the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) at fixed coordinates gives

$$
C^a{}_{bc}=\frac12g^{ad}
(\nabla_b\delta g_{cd}+\nabla_c\delta g_{bd}-\nabla_d\delta g_{bc}).
$$

In the paper's [curvature sign convention](../../../general-relativity.md#curvature-sign-convention), varying the [derivative](../../../calculus.md#derivative) and quadratic-connection terms and grouping them into [covariant derivatives](../../../general-relativity.md#covariant-derivative) gives the [Palatini identity](../../../general-relativity.md#palatini-identity)

$$
\boxed{\delta R_{bc}=\nabla_cC^a{}_{ba}-\nabla_aC^a{}_{bc}.}
$$

One may verify the grouping in [normal coordinates](../../../general-relativity.md#normal-coordinates) at a point, where the [affine connection](../../../fiber-bundle.md#affine-connection) vanishes and the expression is just the difference of two [partial derivatives](../../../calculus.md#partial-derivative); both sides are [tensors](../../../linear-algebra.md#tensor), so it holds in every [coordinate frame](../../../differential-geometry.md#coordinate-basis). Reversing the definition of the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) reverses this identity's right-hand side.

For completeness, put $q_{ab}=\delta g_{ab}$ and $q=g^{ab}q_{ab}$. The contracted variation uses $C^a{}_{ba}=\nabla_bq/2$ and $g^{bc}C^a{}_{bc}=\nabla_bq^{ab}-\nabla^aq/2$. After two [integrations by parts](../../../calculus.md#integration-by-parts),

$$
\int\sqrt{-g}\,\Phi g^{bc}\delta R_{bc}\,d^4x
=\int\sqrt{-g}\left[-\nabla_a\nabla_b\Phi\,q^{ab}
+\Box\Phi\,q\right]d^4x,
$$

up to the discarded [boundary term](../../../calculus.md#boundary-term). Substituting $q^{ab}=-\delta g^{ab}$ gives the differentiated-scalar terms in the [metric variation of a scalar-curvature coupling](../../../general-relativity.md#metric-variation-of-a-scalar-curvature-coupling).

## 4

↑ **Parent:** [Paper 68](paper-68.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The local [metric tensors](../../../general-relativity.md#metric-tensor) do not determine the global coordinate identifications. The usual complete [two-dimensional de Sitter spacetime](../../../general-relativity.md#two-dimensional-de-sitter-spacetime) is the hyperboloid $(X^0)^2-(X^1)^2-(X^2)^2=-1$ in ambient signature $(+--)$, with

$$
X^0=\sinh t,\qquad
X^1=\cosh t\cos\chi,\qquad X^2=\cosh t\sin\chi.
$$

Pulling back the ambient [metric tensor](../../../general-relativity.md#metric-tensor) gives $dt^2-\cosh^2t\,d\chi^2$, with

$$
\boxed{t\in\mathbb R,\qquad \chi\in\mathbb R/(2\pi\mathbb Z).}
$$

Unwrapping $\chi$ gives the [universal cover of two-dimensional de Sitter spacetime](../../../general-relativity.md#universal-cover-of-two-dimensional-de-sitter-spacetime) instead. The usual embedded [two-dimensional anti-de Sitter spacetime](../../../general-relativity.md#two-dimensional-anti-de-sitter-spacetime) has $(X^0)^2+(X^1)^2-(X^2)^2=1$ in signature $(++-)$ and

$$
X^0=\cosh r\cos t,\qquad
X^1=\cosh r\sin t,\qquad X^2=\sinh r.
$$

Here $r\in\mathbb R$ and $t$ is initially periodic modulo $2\pi$. The time circles are [closed timelike curves](../../../general-relativity.md#closed-timelike-curve). Its physically standard [universal cover](../../../algebraic-topology.md#universal-cover) removes that identification:

$$
\boxed{r\in\mathbb R,\qquad t\in\mathbb R.}
$$

The two signs of $r$ describe two spatial ends; imposing $r\ge0$ would retain only half of this complete model.

Both spacetimes have constant [curvature](../../../differential-geometry.md#curvature) and are [geodesically complete](../../../riemannian-geometry.md#geodesic-completeness). In the paper's convention their [Ricci scalars](../../../general-relativity.md#ricci-scalar) are respectively $+2$ and $-2$. Their embeddings show that [geodesics](../../../riemannian-geometry.md#geodesic) are intersections with planes through the ambient origin. They nevertheless have very different causal structures.

For the [geodesics of two-dimensional de Sitter spacetime](../../../general-relativity.md#geodesics-of-two-dimensional-de-sitter-spacetime), use an [affine parameter](../../../riemannian-geometry.md#affine-parameter) $\lambda$, normalization $\kappa=\dot t^2-\cosh^2t\,\dot\chi^2\in\{1,0,-1\}$ and conserved momentum $L=\cosh^2t\,\dot\chi$. Then

$$
\dot t^2=\kappa+\frac{L^2}{\cosh^2t}.
$$

[Timelike geodesics](../../../general-relativity.md#timelike-geodesic) extend to both infinite [proper times](../../../special-relativity.md#proper-time); $\chi=\text{constant}$ is a simple example. [Null geodesics](../../../special-relativity.md#null-geodesic) obey $\sinh t=\pm|L|(\lambda-\lambda_0)$, so their [affine parameter](../../../riemannian-geometry.md#affine-parameter) is also infinite at either temporal end. [Spacelike geodesics](../../../riemannian-geometry.md#spacelike-geodesic) have $|L|\ge1$, obey $\sinh t=\sqrt{L^2-1}\sin(\lambda-\lambda_0)$ and are closed curves on the embedded cylinder; $t=0$ is its simplest [spacelike geodesic](../../../riemannian-geometry.md#spacelike-geodesic) circle. Unwrapping the spatial circle removes closure but not completeness.

For the [geodesics of two-dimensional anti-de Sitter spacetime](../../../general-relativity.md#geodesics-of-two-dimensional-anti-de-sitter-spacetime), the timelike [Killing vector](../../../general-relativity.md#killing-vector-field) $\partial_t$ gives $E=\cosh^2r\,\dot t$. The normalization is $\kappa=\cosh^2r\,\dot t^2-\dot r^2$, hence

$$
\dot r^2=\frac{E^2}{\cosh^2r}-\kappa.
$$

Choose a future-directed [timelike geodesic](../../../general-relativity.md#timelike-geodesic), so $E\ge1$ and

$$
\sinh r=\sqrt{E^2-1}\sin(\lambda-\lambda_0).
$$

For $E>1$, it oscillates radially with proper period $2\pi$; $E=1$ gives the central [geodesic](../../../riemannian-geometry.md#geodesic) $r=0$. In both cases, global time advances by $2\pi$ over a [proper time](../../../special-relativity.md#proper-time) interval $2\pi$. The curve is closed on the original hyperboloid, while its lift on the universal cover is nonclosed and future-directed. [Null geodesics](../../../special-relativity.md#null-geodesic) have $\sinh r=\pm E(\lambda-\lambda_0)$ and reach either spatial end only at infinite [affine parameter](../../../riemannian-geometry.md#affine-parameter). [Spacelike geodesics](../../../riemannian-geometry.md#spacelike-geodesic) satisfy $\sinh r=\sqrt{E^2+1}\sinh(\lambda-\lambda_0)$ and also have infinite [proper length](../../../special-relativity.md#proper-length) toward either end. Thus the finite coordinate time discussed below does not imply physical [geodesic](../../../riemannian-geometry.md#geodesic) incompleteness.

The [conformal cylinder of two-dimensional de Sitter spacetime](../../../general-relativity.md#conformal-cylinder-of-two-dimensional-de-sitter-spacetime) follows by setting $\eta=\arctan(\sinh t)$:

$$
ds^2=\sec^2\eta(d\eta^2-d\chi^2),\qquad
-\frac\pi2<\eta<\frac\pi2.
$$

Its past and future [conformal boundaries](../../../geometry-and-topology.md#conformal-boundary) are spacelike circles. [Null geodesics](../../../special-relativity.md#null-geodesic) have $d\chi/d\eta=\pm1$ and can travel only a finite angular distance over the entire infinite proper-time history. For the complete observer $\chi=0$, an event can send a signal to that observer precisely when its shortest angular distance $d(\chi,0)$ is less than $\pi/2-\eta$. The [observer horizons in two-dimensional de Sitter spacetime](../../../general-relativity.md#observer-horizons-in-two-dimensional-de-sitter-spacetime) are therefore the null curves $d(\chi,0)=\pi/2-\eta$; its past signal horizon has $d(\chi,0)=\eta+\pi/2$. These are observer horizons, without [curvature](../../../differential-geometry.md#curvature) singularities. Their intersection bounds a static patch with [metric tensor](../../../general-relativity.md#metric-tensor)

$$
ds^2=(1-\rho^2)dT^2-\frac{d\rho^2}{1-\rho^2},\qquad |\rho|<1.
$$

The horizons at $\rho=\pm1$ are regular [Killing horizons](../../../general-relativity.md#killing-horizon) beyond which this static chart fails, while the global coordinates remain smooth.

For the [conformal strip of two-dimensional anti-de Sitter spacetime](../../../general-relativity.md#conformal-strip-of-two-dimensional-anti-de-sitter-spacetime), set $\psi=\arctan(\sinh r)$. On its universal cover,

$$
ds^2=\sec^2\psi(dt^2-d\psi^2),\qquad
-\frac\pi2<\psi<\frac\pi2,\qquad t\in\mathbb R.
$$

The two conformal boundaries are timelike. A null ray from the center approaches a boundary after coordinate time $\pi/2$, though its [affine parameter](../../../riemannian-geometry.md#affine-parameter) diverges. Every interior event can signal to the complete central static observer in finite global time, so that observer has no event horizon. A [Poincaré horizon](../../../general-relativity.md#poincare-horizon) concerns a restricted coordinate patch, and accelerated observers can have different causal horizons.

Finally, the global de Sitter cylinder and its spatial cover are [globally hyperbolic](../../../general-relativity.md#globally-hyperbolic-spacetime): constant-time slices are [Cauchy hypersurfaces](../../../general-relativity.md#cauchy-surface). The anti-de Sitter universal cover is not globally hyperbolic, because timelike infinity admits incoming signals within finite global time. A field's evolution therefore requires [boundary conditions](../../../differential-equation.md#boundary-condition) at its two conformal boundaries in addition to [initial data](../../../general-relativity.md#initial-data-in-general-relativity). The opposite placement of the conformal boundaries explains why de Sitter observers have cosmological horizons despite global hyperbolicity, while the central anti-de Sitter observer has no event horizon despite the failure of global hyperbolicity.

<a id="4/image-conformal-cylinder-and-observer-horizons-of-de-sitter-spacetime-compared-with-the-timelike-boundaries-of-the-anti-de-sitter-universal-cover"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-68-conformal-diagrams.png)

**[Figure 1](#4/image-conformal-cylinder-and-observer-horizons-of-de-sitter-spacetime-compared-with-the-timelike-boundaries-of-the-anti-de-sitter-universal-cover). Conformal cylinder and observer horizons of de Sitter spacetime compared with the timelike boundaries of the anti-de Sitter universal cover**.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
