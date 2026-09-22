<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [vierbein](../../../../../orthonormal-coframe-in-spacetime.md) is a local orthonormal coframe, consisting of four [linearly independent](../../../../../linear-independence.md) [covectors](../../../../../covector.md) $e^\mu{}_a$ such that

$$
g_{ab}=\eta_{\mu\nu}e^\mu{}_ae^\nu{}_b.
$$

Here $a,b$ label spacetime coordinates, while $\mu,\nu$ label a Lorentz frame with $\eta=\operatorname{diag}(-1,1,1,1)$. Its inverse $e_\mu{}^a$ obeys $e_\mu{}^ae^\mu{}_b=\delta^a_b$ and $e_\mu{}^ae^\nu{}_a=\delta^\nu_\mu$. The [vierbein](../../../../../orthonormal-coframe-in-spacetime.md) converts tensor indices between the coordinate and orthonormal descriptions.

The metric is unchanged under an arbitrary [local Lorentz transformation](../../../../../local-lorentz-transformation.md) $e^\mu{}_a\mapsto\Lambda^\mu{}_{\nu}(x)e^\nu{}_a$, since $\Lambda^T\eta\Lambda=\eta$. This is local frame redundancy, with corresponding transformations of fields and connections; it is distinct from coordinate [diffeomorphism](../../../../../diffeomorphism.md) covariance. A generic curved spacetime does not have global Lorentz isometries. Rather, local tangent frames have Lorentz freedom, and the field equations can be written covariantly under their changes. On flat spacetime, global [Lorentz transformations](../../../../../lorentz-transformation.md) are also spacetime [isometries](../../../../../isometry.md).

A [spinor field](../../../../../spinor-field.md) is a section of the [spinor bundle](../../../../../spinor-bundle.md) associated to a [spin structure](../../../../../spin-structure.md). Local components transform in a [Spinor representation of the Lorentz group](../../../../../spinor-representation-of-the-lorentz-group.md), more precisely a representation of its spin double cover. For the proper orthochronous group in four dimensions, that cover is $\operatorname{Spin}^+(1,3)\simeq SL(2,\mathbb C)$. Thus a [spinor field](../../../../../spinor-field.md) transforms as $\epsilon\mapsto S(\Lambda)\epsilon$ under frame changes, rather than as a coordinate-index tensor. The double-valued lift of a frame rotation requires a consistent [spin structure](../../../../../spin-structure.md) globally; local spinor calculations alone do not choose that global structure. One can use a [Dirac spinor](../../../../../dirac-spinor.md) for the gamma-matrix calculation below.

Write $\omega_a{}^\mu{}_{\nu}$ for the Lorentz-frame [spin connection](../../../../../spin-connection.md). Expanding the [tetrad postulate](../../../../../tetrad-postulate.md) gives

$$
0=\nabla_ae^\mu{}_b=\partial_ae^\mu{}_b
-\Gamma^c{}_{ab}e^\mu{}_c+\omega_a{}^\mu{}_{\nu}e^\nu{}_b.
$$

Multiply by the inverse [vierbein](../../../../../orthonormal-coframe-in-spacetime.md) to solve for the connection:

$$
\boxed{\omega_a{}^\mu{}_{\nu}
=e_\nu{}^b\left(\Gamma^c{}_{ab}e^\mu{}_c-\partial_ae^\mu{}_b\right).}
$$

With the torsion-free [Levi-Civita connection](../../../../../levi-civita-connection.md), [metric compatibility](../../../../../metric-compatibility.md) makes $\omega_{a\mu\nu}=\eta_{\mu\rho}\omega_a{}^\rho{}_{\nu}$ antisymmetric in $\mu,\nu$. For constant flat [gamma matrices](../../../../../gamma-matrices.md) obeying $\{\widehat\gamma^\mu,\widehat\gamma^\nu\}=2\eta^{\mu\nu}$, define $\widehat\gamma^{\mu\nu}=[\widehat\gamma^\mu,\widehat\gamma^\nu]/2$. The [spinor covariant derivative](../../../../../spinor-covariant-derivative.md) is

$$
\nabla_a\epsilon=\partial_a\epsilon+\frac14\omega_{a\mu\nu}\widehat\gamma^{\mu\nu}\epsilon.
$$

Under a [local Lorentz transformation](../../../../../local-lorentz-transformation.md), the matrix connection acquires the inhomogeneous term needed to make $\nabla_a\epsilon$ transform as a spinor. The derivative of the [vierbein](../../../../../orthonormal-coframe-in-spacetime.md) in the boxed formula is therefore essential.

For the [conformally flat metric](../../../../../conformally-flat-metric.md), choose $e^\mu{}_a=\Omega\delta^\mu{}_a$ and $e_\mu{}^a=\Omega^{-1}\delta_\mu^a$. Let $\ell_a=\partial_a\log\Omega$ and raise these coordinate indices temporarily with the flat metric $\eta$. Directly evaluating the [Christoffel symbols](../../../../../christoffel-symbol.md) gives

$$
\Gamma^c{}_{ab}=\delta^c_a\ell_b+\delta^c_b\ell_a-\eta_{ab}\ell^c.
$$

Since $\partial_ae^\mu{}_b=\Omega\ell_a\delta^\mu_b$, the connection formula yields

$$
\omega_a{}^\mu{}_{\nu}=\delta^\mu_a\ell_\nu-\eta_{a\nu}\ell^\mu,
\qquad
\boxed{\omega_{a\mu\nu}=\eta_{a\mu}\ell_\nu-\eta_{a\nu}\ell_\mu.}
$$

This is the [spin connection of a conformally flat metric](../../../../../spin-connection-of-a-conformally-flat-metric.md) in the specified conformal frame. It is frame dependent, unlike an invariant curvature tensor.

Set $L=\widehat\gamma^c\ell_c$. Antisymmetry of $\omega$ makes its action on spinors

$$
\frac14\omega_{a\mu\nu}\widehat\gamma^{\mu\nu}
=\frac14[\widehat\gamma_a,L].
$$

For $\epsilon=\Omega^{1/2}\epsilon_0$ with $\partial_a\epsilon_0=0$, we have $\partial_a\epsilon=\ell_a\epsilon/2$. The [Clifford algebra](../../../../../clifford-algebra.md) gives $\{\widehat\gamma_a,L\}=2\ell_a$, so

$$
\nabla_a\epsilon=\left(\frac12\ell_a+\frac14[\widehat\gamma_a,L]\right)\epsilon
=\frac12\widehat\gamma_aL\epsilon.
$$

The curved [gamma matrices](../../../../../gamma-matrices.md) are $\gamma_a=\Omega\widehat\gamma_a$ and $\gamma^a=\Omega^{-1}\widehat\gamma^a$. Consequently

$$
\gamma^c\nabla_c\epsilon=2\Omega^{-1}L\epsilon,
\qquad
\nabla_a\epsilon=\frac14\gamma_a\gamma^c\nabla_c\epsilon.
$$

Thus the rescaled field is a [twistor spinor](../../../../../twistor-spinor.md). Multiplying this last equation by $\gamma_b$, symmetrizing in $a,b$ and using $\{\gamma_a,\gamma_b\}=2g_{ab}$ proves

$$
\boxed{\left[\gamma_a\nabla_b+\gamma_b\nabla_a-\frac12g_{ab}\gamma^c\nabla_c\right]\epsilon=0.}
$$

This is the [conformal rescaling of a parallel spinor to a twistor spinor](../../../../../conformal-rescaling-of-a-parallel-spinor-to-a-twistor-spinor.md). It does not claim that the rescaled spinor remains parallel in the conformal metric; the nonzero connection and the derivative of $\Omega^{1/2}$ combine precisely into its gamma-trace part.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
