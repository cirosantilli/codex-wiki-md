<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use four-dimensional [Minkowski spacetime](../../../../../minkowski-spacetime.md) with $\{\gamma^\mu,\gamma^\nu\}=2\eta^{\mu\nu}$ and $\gamma^{\mu\nu\rho}=\gamma^{[\mu}\gamma^\nu\gamma^{\rho]}$. The [Clifford algebra](../../../../../clifford-algebra.md) duality identity makes the displayed epsilon-form equation equivalent, up to a nonzero convention-dependent phase, to

$$
E^\mu:=\gamma^{\mu\nu\rho}\partial_\nu\Psi_\rho=0.
$$

This is the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) of the first-order [Rarita-Schwinger field](../../../../../rarita-schwinger-field.md) action $-\tfrac12\bar\Psi_\mu\gamma^{\mu\nu\rho}\partial_\nu\Psi_\rho$, with the overall phase adjusted to the chosen Majorana convention. Varying the [Majorana spinor](../../../../../majorana-spinor.md) action accounts for both occurrences of the field and cancels the one-half normalization.

A vector times a spinor contains [spin](../../../../../spin.md)-$3/2$ and unwanted [spin](../../../../../spin.md)-$1/2$ pieces, so the tensor type alone does not establish the physical spin. The field equation has [gauge invariance](../../../../../gauge-invariance.md)

$$
\Psi_\mu\longmapsto\Psi_\mu+\partial_\mu\epsilon,
$$

since the two derivatives contract an antisymmetric pair of gamma indices. Put $\chi=\gamma^\mu\Psi_\mu$ and $d=\partial^\mu\Psi_\mu$. [Gamma matrix](../../../../../gamma-matrices.md) multiplication gives

$$
E^\mu=\not\!\partial\Psi^\mu-\partial^\mu\chi
+\gamma^\mu(\not\!\partial\chi-d),\qquad
\gamma_\mu E^\mu=2(\not\!\partial\chi-d).
$$

Hence $d=\not\!\partial\chi$. Use the [gauge transformation](../../../../../gauge-transformation.md), under which $\delta\chi=\not\!\partial\epsilon$, to impose $\chi=0$. The equations then imply

$$
\boxed{\gamma\cdot\Psi=0,\qquad\partial\cdot\Psi=0,\qquad
\not\!\partial\Psi_\mu=0,}
$$

with residual gauge freedom satisfying $\not\!\partial\epsilon=0$.

For a [plane wave](../../../../../plane-wave.md) with nonzero momentum satisfying the [null condition](../../../../../null-condition.md) along the third axis, this residual freedom sets the temporal component to zero. Transversality then removes the longitudinal component, leaving the [tensor product](../../../../../tensor-product.md) of two transverse vector polarizations with the two massless spinor [helicities](../../../../../helicity.md). The possible total [helicities](../../../../../helicity.md) are $\pm3/2$ and $\pm1/2$. The [gamma trace](../../../../../gamma-trace-of-a-vector-spinor.md) is a rotation-covariant map to a spinor, which has only [helicities](../../../../../helicity.md) $\pm1/2$. It therefore vanishes on the aligned $\pm3/2$ combinations and removes the two mixed combinations. Equivalently, the transverse [gamma trace](../../../../../gamma-trace-of-a-vector-spinor.md) condition has rank two on the four remaining complex positive-frequency coefficients. The [massless Rarita-Schwinger polarization count](../../../../../massless-rarita-schwinger-polarization-count.md) is thus

$$
\boxed{h=\pm\tfrac32:\quad2\text{ physical states for a Majorana gravitino}.}
$$

The [Majorana spinor](../../../../../majorana-spinor.md) reality condition relates negative-frequency coefficients to their conjugates; it does not introduce a separate antiparticle multiplet. A complex vector-spinor would also have independent antiparticle states.

A nonzero standard [Rarita-Schwinger field](../../../../../rarita-schwinger-field.md) mass term destroys the massless [gauge invariance](../../../../../gauge-invariance.md) and adds the two longitudinal [helicities](../../../../../helicity.md). To see the constraints explicitly, choose its momentum-space sign so the equation is

$$
\gamma^{\mu\nu\rho}p_\nu u_\rho+m\gamma^{\mu\rho}u_\rho=0.
$$

Contracting with $p_\mu$ gives $\not\!p(\gamma\cdot u)-p\cdot u=0$. Its [gamma trace](../../../../../gamma-trace-of-a-vector-spinor.md) then gives $3m\,\gamma\cdot u=0$. For $m\ne0$ these imply $\gamma\cdot u=p\cdot u=0$, and the remaining [Dirac equation](../../../../../dirac-equation.md) is $(\not\!p-m)u_\mu=0$. In the rest frame $u_0=0$. Three spatial vector components times two positive-energy spinor components give six coefficients, and the [gamma trace](../../../../../gamma-trace-of-a-vector-spinor.md) removes two, leaving the irreducible [spin](../../../../../spin.md)-$3/2$ representation. Therefore

$$
\boxed{\text{a massive Majorana gravitino has }4\text{ physical states},
\quad h=\pm\tfrac32,\ \pm\tfrac12.}
$$

In [supergravity](../../../../../supergravity.md) a consistent spontaneous mass generation is the [super-Higgs mechanism](../../../../../super-higgs-mechanism.md), which supplies those extra states from the [goldstino](../../../../../goldstino.md).

The massless [graviton](../../../../../graviton.md) also has two physical [helicities](../../../../../helicity.md), so the [graviton](../../../../../graviton.md) and [gravitino](../../../../../gravitino.md) already match on shell. The reason for [auxiliary fields](../../../../../auxiliary-field.md) is the [off-shell component count of minimal supergravity](../../../../../off-shell-component-count-of-minimal-supergravity.md) mismatch, not a mismatch of these physical states. After removing gauge functions but before using field equations, a metric has $10-4=6$ independent bosonic components, while a Majorana vector-spinor has $16-4=12$ fermionic components. In [vierbein](../../../../../orthonormal-coframe-in-spacetime.md) language the same bosonic count is $16-6-4=6$, subtracting local Lorentz and [diffeomorphism](../../../../../diffeomorphism.md) gauges. [Old-minimal supergravity](../../../../../old-minimal-supergravity.md) adds a complex scalar and a real vector, supplying six real nonpropagating bosonic components. This gives **$12+12$ off-shell components and closure without imposing equations of motion**. Their algebraic elimination leaves the physical $2+2$ [graviton](../../../../../graviton.md)–[gravitino](../../../../../gravitino.md) spectrum unchanged.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 57](../../paper-57-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
