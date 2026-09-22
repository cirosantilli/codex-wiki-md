<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

Ordinary [electromagnetism](../../../../../electromagnetism-split.md) uses a one-form [gauge potential](../../../../../gauge-field.md), its [gauge transformation](../../../../../gauge-transformation.md) and its curvature. On [superspace](../../../../../superspace.md) the corresponding object is a [superspace gauge connection](../../../../../superspace-gauge-connection.md), with both vector and spinor components. Write $\nabla_A=D_A+i\mathcal A_A$. Its graded commutator contains the flat-frame torsion plus supercurvature. The conventional constraints set the two undotted-spinor curvatures, the two dotted-spinor curvatures and the conventional mixed spinor curvature to zero; the mixed derivative algebra then determines the vector connection. The remaining independent gauge curvature is packaged into a [chiral field-strength superfield](../../../../../chiral-field-strength-superfield.md). A real [vector superfield](../../../../../vector-superfield.md) $V=V^\dagger$ is a prepotential solving these constraints, rather than four unrelated ordinary [gauge potentials](../../../../../gauge-field.md).

Use the left-derivative conventions of Question 5, with $D^2=D^\alpha D_\alpha$ and $\bar D^2=\bar D_{\dot\alpha}\bar D^{\dot\alpha}$. An Abelian [supergauge transformation](../../../../../supergauge-transformation.md) has a chiral parameter $\Lambda$, and one consistent normalization is

$$
V'=V+i(\Lambda-\bar\Lambda),\qquad
\Phi'=e^{-2iq\Lambda}\Phi,\qquad\bar D_{\dot\alpha}\Lambda=0.
$$

The parameter is chiral so that the transformed matter is still a [chiral superfield](../../../../../chiral-superfield.md); its complex components remove more of the prepotential than an ordinary real gauge parameter. In [Wess-Zumino gauge](../../../../../wess-zumino-gauge.md), one convenient expansion is

$$
V=-\theta\sigma^m\bar\theta A_m+i\theta^2\bar\theta\bar\lambda
-i\bar\theta^2\theta\lambda+\frac12\theta^2\bar\theta^2D.
$$

Its components are the [gauge potential](../../../../../gauge-field.md) $A_m$, the [gaugino](../../../../../gaugino.md) $\lambda$ and the real [auxiliary field](../../../../../auxiliary-field.md) $D$. [Wess-Zumino gauge](../../../../../wess-zumino-gauge.md) removes the extra scalar and spinor components of a general real [superfield](../../../../../superfield.md). [Supersymmetry](../../../../../supersymmetry-split.md) transformations usually leave that gauge slice and require a compensating [supergauge transformation](../../../../../supergauge-transformation.md). For a residual chiral parameter with real lowest component $a(x)$, the expansion gives $A_m'=A_m+2\partial_ma$ and $\phi'=e^{-2iqa}\phi$; thus $\alpha=2a$ is the ordinary Maxwell gauge parameter.

The Abelian field strength is the [Abelian field-strength chiral projection](../../../../../abelian-field-strength-chiral-projection.md)

$$
\boxed{W_\alpha=-\frac14\bar D^2D_\alpha V.}
$$

Three barred derivatives vanish because there are only two anticommuting dotted components, so $\bar D_{\dot\beta}W_\alpha=0$. Gauge invariance follows directly: $D_\alpha\bar\Lambda=0$ by antichirality, while the mixed derivative algebra gives $\bar D^2D_\alpha\Lambda=0$ for chiral $\Lambda$. In chiral coordinates its component structure is

$$
W_\alpha=-i\lambda_\alpha+\theta_\alpha D
-i(\sigma^{mn}\theta)_\alpha F_{mn}
+\theta^2(\sigma^m\partial_m\bar\lambda)_\alpha,
\qquad F_{mn}=\partial_mA_n-\partial_nA_m,
$$

where $\sigma^{mn}=(\sigma^m\bar\sigma^n-\sigma^n\bar\sigma^m)/4$ fixes the tensor normalization. Overall [gaugino](../../../../../gaugino.md) phase choices do not change the gauge-invariant field strength or its Bianchi constraint.

Reality of $V$ and the derivative algebra imply the [superspace Yang-Mills Bianchi identity](../../../../../superspace-yang-mills-bianchi-identity.md)

$$
\boxed{D^\alpha W_\alpha=\bar D_{\dot\alpha}\bar W^{\dot\alpha}.}
$$

Indeed, the two sides are the same differential operator on $V$, because $D^\alpha\bar D^2D_\alpha=\bar D_{\dot\alpha}D^2\bar D^{\dot\alpha}$. This is the superspace counterpart of $dF=0$, and its components contain $\partial_{[m}F_{np]}=0$. It is a defining curvature constraint, not the [Maxwell equations](../../../../../maxwell-equations.md). Varying the pure gauge [action](../../../../../action.md) additionally sets the common real [superfield](../../../../../superfield.md) $D^\alpha W_\alpha$ to zero; matter supplies a current instead.

The [Supersymmetric Yang-Mills action](../../../../../supersymmetric-yang-mills-action.md) and minimal matter coupling are

$$
S=\frac1{4g^2}\int d^4x\,d^2\theta\,W^\alpha W_\alpha+\mathrm{h.c.}
+\int d^4x\,d^4\theta\,\bar\Phi e^{2qV}\Phi
+\left[\int d^4x\,d^2\theta\,\mathcal W(\Phi)+\mathrm{h.c.}\right].
$$

The chiral phase factors cancel in $\bar\Phi e^{2qV}\Phi$. The component matter derivative is $(\partial_m+iqA_m)\phi$, which transforms covariantly under the residual [gauge transformation](../../../../../gauge-transformation.md) just derived. The same superspace term generates the associated matter–[gaugino](../../../../../gaugino.md) [Yukawa coupling](../../../../../yukawa-interaction.md) and $qD|\phi|^2$ auxiliary coupling, so minimal coupling is not only replacing an ordinary derivative in the scalar [action](../../../../../action.md). The gauge [action](../../../../../action.md) contains $-F_{mn}F^{mn}/(4g^2)$, the [gaugino](../../../../../gaugino.md) kinetic term and $D^2/(2g^2)$. Rescaling the [vector multiplet](../../../../../supersymmetric-vector-multiplet.md) to canonical kinetic normalization gives the physical coupling $qg$. The holomorphic [superpotential](../../../../../superpotential.md) must be gauge invariant; a single field of nonzero continuous Abelian charge admits no nonconstant polynomial [superpotential](../../../../../superpotential.md) without additional fields. For several fields, invariance requires $\sum_iq_i\Phi_i\mathcal W_i=0$. A [Fayet–Iliopoulos term](../../../../../fayet-iliopoulos-term.md) is additionally possible for an Abelian factor, shifting the algebraic $D$ equation.

For a non-Abelian [gauge group](../../../../../gauge-group.md), $V$ and $\Lambda$ are Lie-algebra-valued, and multiplication cannot be reordered. For matter in a specified representation, set

$$
\Phi'=e^{-2i\Lambda}\Phi,\qquad
\boxed{e^{2V'}=e^{-2i\Lambda^\dagger}e^{2V}e^{2i\Lambda}.}
$$

The same matter quadratic form remains invariant. Its curvature is

$$
\boxed{W_\alpha=-\frac18\bar D^2\bigl(e^{-2V}D_\alpha e^{2V}\bigr),
\qquad W_\alpha'=e^{-2i\Lambda}W_\alpha e^{2i\Lambda}.}
$$

At first order in an Abelian $V$, this reduces to $-\bar D^2D_\alpha V/4$, fixing the factor $1/8$. In the chiral gauge frame, $\bar\nabla=\bar D$ and $\nabla_\alpha=e^{-2V}D_\alpha e^{2V}$ as an operator. The gauge-covariant Bianchi identity is $\nabla^\alpha W_\alpha=\bar\nabla_{\dot\alpha}\widetilde{\bar W}^{\dot\alpha}$, where $\widetilde{\bar W}=e^{-2V}\bar W e^{2V}$ is the conjugate curvature expressed in that same frame. It follows from the [graded Jacobi identity](../../../../../graded-jacobi-identity.md) of the [covariant derivatives](../../../../../covariant-derivative.md). Taking a trace of $W^\alpha W_\alpha$ makes the chiral gauge [action](../../../../../action.md) invariant. Its bosonic curvature becomes the ordinary Yang-Mills curvature, and the [gaugino](../../../../../gaugino.md) transforms in the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md). A constant Fayet–Iliopoulos coefficient cannot be inserted for a simple non-Abelian group, since it would need an invariant linear functional annihilating every Lie bracket. These constructions connect the constrained superspace connection, its prepotential and its component gauge multiplet.

## ↑ Ancestors (11)

1. [9](../9.md)
2. [Section B](../section-b.md)
3. [Paper 53](../../paper-53-split.md)
4. [Iii](../../split.md)
5. [2003](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
