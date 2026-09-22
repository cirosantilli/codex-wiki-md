<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Absorb the gauge coupling into the connection $A_\mu=A_\mu^aT_a$ and use $D_\mu=\partial_\mu+A_\mu$. The anti-Hermitian generators make $U(x)=\exp[\omega^a(x)T_a]$ unitary for real parameters. With a matter field transforming as $\psi'=U\psi$, require $D_\mu'\psi'=UD_\mu\psi$. Applying both sides to an arbitrary field gives

$$
\boxed{A_\mu'=UA_\mu U^{-1}-(\partial_\mu U)U^{-1}.}
$$

Expanding $U=1+\omega+O(\omega^2)$ and $U^{-1}=1-\omega+O(\omega^2)$ yields the [infinitesimal gauge transformation with an anti-Hermitian connection](../../../../../infinitesimal-gauge-transformation-with-an-anti-hermitian-connection.md)

$$
\boxed{\delta A_\mu=[\omega,A_\mu]-\partial_\mu\omega
=-D_\mu\omega.}
$$

The [adjoint covariant derivative](../../../../../adjoint-covariant-derivative.md) is $D_\mu\omega=\partial_\mu\omega+[A_\mu,\omega]$. In components,

$$
\boxed{\delta A_\mu^a=-\partial_\mu\omega^a-f_{bca}A_\mu^b\omega^c.}
$$

The trace normalization makes the [structure constants](../../../../../structure-constant.md) totally antisymmetric: $f_{abc}=-\operatorname{Tr}([T_a,T_b]T_c)$ and cyclicity of the trace supply antisymmetry in the remaining indices. Replacing $U=e^\omega$ by $e^{-\omega}$ reverses the infinitesimal parameter convention and gives $\delta A=D\omega$; mixing the two conventions would change the ghost operator incorrectly. The trace normalization also gives the invariant quadratic form $-\operatorname{Tr}(A_\mu A_\nu)=A_\mu^aA_\nu^a$.

A gauge-invariant [functional integral](../../../../../functional-measure.md) counts all representatives along each [gauge orbit](../../../../../gauge-orbit.md). The gauge condition $\mathcal F[A]=0$ selects a representative, and its delta functional enforces that selection. Assume a local patch where each orbit intersects the gauge slice once and the gauge-condition derivative has no residual zero modes. Define

$$
M_{ab}(x,y)=\left.\frac{\delta\mathcal F_a[A^\omega](x)}{\delta\omega^b(y)}\right|_{\omega=0}.
$$

Changing the orbit integration variable from $\omega$ to $\mathcal F[A^\omega]$ gives

$$
\int\mathcal D\omega\,\delta[\mathcal F(A^\omega)]
=\frac1{|\det M|},\qquad
1=|\det M|\int\mathcal D\omega\,\delta[\mathcal F(A^\omega)].
$$

Insert this [Faddeev-Popov gauge-orbit identity](../../../../../faddeev-popov-gauge-orbit-identity.md) into the unfixed path integral. The action and measure are invariant under a change $A\mapsto A^\omega$, so integration over $\omega$ factors out as the gauge-group volume. Dividing by that redundant volume leaves the fixed integral and its [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md). In a perturbative patch with fixed determinant sign or phase, the absolute value is replaced by the oriented determinant, up to a field-independent normalization:

$$
\boxed{\Delta[A]=\det M,\qquad
M_{ab}(x,y)=-\int d^dz\,
\frac{\delta\mathcal F_a[A](x)}{\delta A_\mu^c(z)}
D_\mu^{cb}(z)\delta^{(d)}(z-y).}
$$

Here $D_\mu^{cb}=\delta^{cb}\partial_\mu+f_{dbc}A_\mu^d$. This is a [functional determinant](../../../../../functional-determinant.md) of the gauge-condition Jacobian, not an arbitrary extra weight. The local invertibility assumption matters: residual gauge transformations or multiple orbit intersections, described by the [Gribov ambiguity](../../../../../gribov-ambiguity.md), prevent treating this derivation as a global unique gauge slice without further qualifications.

Both extra factors can be incorporated into an enlarged action. An auxiliary real field $b^a$ Fourier-represents the delta functional, while a [Grassmann Gaussian integral](../../../../../grassmann-gaussian-integral.md) over independent [Faddeev-Popov ghost fields](../../../../../faddeev-popov-ghost.md) $c,\bar c$ represents the determinant:

$$
\delta[\mathcal F]\propto\int\mathcal Db\,e^{i\int b^a\mathcal F_a},\qquad
\det M\propto\int\mathcal D\bar c\,\mathcal Dc\,
\exp\left(i\int dx\,dy\,\bar c^a(x)M_{ab}(x,y)c^b(y)\right).
$$

Thus the original fixed integral can be written with **action $S+\int b\mathcal F+\int\bar cMc$** and ordinary integration over the extra fields, with no explicit delta functional or determinant. The anticommuting fields give a determinant rather than the inverse determinant obtained from commuting Gaussian fields.

For the usual Gaussian family of gauges, add $\xi b^ab^a/2$ and integrate out $b$. [Completing the square](../../../../../completing-the-square.md) produces

$$
\boxed{S_{\rm gf+gh}=S-\frac1{2\xi}\int d^dx\,\mathcal F_a\mathcal F_a
+\int dx\,dy\,\bar c^a(x)M_{ab}(x,y)c^b(y).}
$$

This is [Gaussian gauge fixing with an auxiliary field](../../../../../gaussian-gauge-fixing-with-an-auxiliary-field.md); equivalently one averages the condition $\mathcal F=f$ with its Gaussian weight. Gauge-invariant observables are unchanged apart from normalization. For the [Lorenz gauge](../../../../../lorenz-gauge-condition.md) $\mathcal F_a=\partial^\mu A_\mu^a$, the chosen transformation convention gives $M=-\partial^\mu D_\mu$. The ghost action is $-\int\bar c\,\partial^\mu D_\mu c$, or $\int(\partial^\mu\bar c)D_\mu c$ after [integration by parts](../../../../../integration-by-parts.md). The dependence of $D$ on $A$ accounts for the ghost interactions.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 65](../../paper-65-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
