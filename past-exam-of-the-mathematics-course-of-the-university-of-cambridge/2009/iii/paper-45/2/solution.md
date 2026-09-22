<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $R_a=\operatorname{ad}(T_a)$, where $\operatorname{ad}(X)Y=[X,Y]$. In the given basis, the [Adjoint representation of a Lie algebra](../../../../../adjoint-representation-of-a-lie-algebra.md) is

$$
(R_a)^c{}_b=f^c{}_{ab}.
$$

The [Jacobi identity](../../../../../jacobi-identity.md) gives $[\operatorname{ad}X,\operatorname{ad}Y]=\operatorname{ad}[X,Y]$, so $[R_a,R_b]=f^c{}_{ab}R_c$, as required for a [Lie algebra representation](../../../../../lie-algebra-representation.md). The [Killing form](../../../../../killing-form.md) is the symmetric [Trace form of a Lie algebra representation](../../../../../trace-form-of-a-lie-algebra-representation.md)

$$
\boxed{\kappa_{ab}=\operatorname{tr}(R_aR_b)=f^c{}_{ad}f^d{}_{bc}.}
$$

Cyclicity of the [trace](../../../../../matrix-trace.md) proves its invariance directly:

$$
\begin{aligned}
\kappa([T_a,T_b],T_c)+\kappa(T_b,[T_a,T_c])
&=\operatorname{tr}\bigl([R_a,R_b]R_c+R_b[R_a,R_c]\bigr)\\
&=\operatorname{tr}(R_aR_bR_c-R_bR_cR_a)=0.
\end{aligned}
$$

In components this is precisely $\boxed{\kappa_{dc}f^d{}_{ab}+\kappa_{bd}f^d{}_{ac}=0}$, so the [Killing form](../../../../../killing-form.md) is an [invariant bilinear form on a Lie algebra](../../../../../invariant-bilinear-form-on-a-lie-algebra.md).

Choose the infinitesimal [gauge transformation](../../../../../gauge-transformation.md) convention $\delta\phi=\omega\phi$, with $\omega(x)=\omega^a(x)t_a$, and write $A_\mu=A_\mu^at_a$. A [gauge covariant derivative](../../../../../gauge-covariant-derivative.md) must satisfy $D'_\mu=UD_\mu U^{-1}$ for $U=1+\omega+O(\omega^2)$; hence

$$
A'_\mu=UA_\mu U^{-1}-(\partial_\mu U)U^{-1},\qquad
\boxed{\delta A_\mu=-\partial_\mu\omega+[\omega,A_\mu].}
$$

Equivalently $\delta A_\mu^a=-\partial_\mu\omega^a+f^a{}_{bc}\omega^bA_\mu^c$. Expanding $\delta(D_\mu\phi)$ makes the cancellation transparent:

$$
\begin{aligned}
\delta(D_\mu\phi)
&=(\partial_\mu\omega)\phi+\omega\partial_\mu\phi
+(-\partial_\mu\omega+[\omega,A_\mu])\phi+A_\mu\omega\phi\\
&=\omega(\partial_\mu\phi+A_\mu\phi).
\end{aligned}
$$

Thus $\boxed{\delta(D_\mu\phi)=\omega^at_aD_\mu\phi}$: it transforms in the same representation as $\phi$. In [adjoint covariant derivative](../../../../../adjoint-covariant-derivative.md) notation, $\delta A_\mu=-D_\mu^{\mathrm{ad}}\omega$.

The commutator of two [gauge covariant derivatives](../../../../../gauge-covariant-derivative.md) defines the [gauge field strength](../../../../../gauge-field-strength.md):

$$
[D_\mu,D_\nu]\phi=F_{\mu\nu}^at_a\phi,\qquad
F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu+[A_\mu,A_\nu].
$$

Thus

$$
\boxed{F^a_{\mu\nu}=\partial_\mu A^a_\nu-\partial_\nu A^a_\mu+f^a{}_{bc}A^b_\mu A^c_\nu.}
$$

Conjugating the derivative commutator gives $F'_{\mu\nu}=UF_{\mu\nu}U^{-1}$, so the [gauge field strength](../../../../../gauge-field-strength.md) transforms homogeneously in the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md):

$$
\boxed{\delta F_{\mu\nu}=[\omega,F_{\mu\nu}],\qquad
\delta F^a_{\mu\nu}=f^a{}_{bc}\omega^bF^c_{\mu\nu}.}
$$

Even if the matrices $t_a$ in a particular matter representation are not faithful, the displayed component formula defines the Lie-algebra-valued curvature independently of that representation.

Only $g_{(ab)}$ contributes to the [Yang-Mills theory](../../../../../yang-mills-theory.md) Lagrangian, since $F^a_{\mu\nu}F^{b\mu\nu}$ is symmetric in $a,b$. Thus take $g_{ab}$ to be a constant real [symmetric bilinear form](../../../../../symmetric-bilinear-form.md). Its infinitesimal variation is

$$
\delta\mathcal L=-\frac14\omega^a\bigl(g_{dc}f^d{}_{ab}+g_{bd}f^d{}_{ac}\bigr)
F^b_{\mu\nu}F^{c\mu\nu}.
$$

Arbitrary local field strengths and gauge parameters give the necessary and sufficient [invariant gauge kinetic form](../../../../../invariant-gauge-kinetic-form.md) condition

$$
\boxed{g_{dc}f^d{}_{ab}+g_{bd}f^d{}_{ac}=0,\qquad g_{ab}=g_{ba}.}
$$

An antisymmetric part is unconstrained but contributes nothing. A nondegenerate kinetic term additionally needs a [nondegenerate bilinear form](../../../../../nondegenerate-bilinear-form.md); positive energy additionally needs a positive internal metric in the signature $(+---)$ convention. Neither extra condition follows solely from [gauge invariance](../../../../../gauge-invariance.md). For a compact simple real [Lie algebra](../../../../../lie-algebra-split.md), $-\kappa$ is positive definite and is the standard choice up to a positive factor.

For the intended complex-simple setting, the [Killing form](../../../../../killing-form.md) is nondegenerate. Consequently write any [invariant bilinear form on a Lie algebra](../../../../../invariant-bilinear-form-on-a-lie-algebra.md) uniquely as $g(X,Y)=\kappa(SX,Y)$. Invariance of both forms implies

$$
\kappa\bigl((S\operatorname{ad}Z-\operatorname{ad}Z\,S)X,Y\bigr)=0
$$

for every $X,Y,Z$, so $S$ commutes with the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md). A subspace invariant under all adjoint maps is an ideal, hence simplicity makes the adjoint representation irreducible. By [Schur lemma](../../../../../schur-s-lemma.md), $S=cI$, giving the [uniqueness of an invariant bilinear form on a simple Lie algebra](../../../../../uniqueness-of-an-invariant-bilinear-form-on-a-simple-lie-algebra.md):

$$
\boxed{g_{ab}=c\kappa_{ab}.}
$$

The same conclusion holds for compact simple real algebras by complexification, with $c$ real; nondegeneracy excludes $c=0$, and positive energy selects $c<0$ in the stated convention.

There is a genuine [real-simple exception to uniqueness of the Killing form](../../../../../real-simple-exception-to-uniqueness-of-the-killing-form.md) if “simple” is read as an arbitrary real simple algebra. Regard $\mathfrak{sl}_2(\mathbb C)$ as real. It is real simple: its complexification consists of two complex simple factors exchanged by conjugation, so a conjugation-stable ideal is zero or the whole algebra. Both $\operatorname{Re}\kappa_{\mathbb C}$ and $\operatorname{Im}\kappa_{\mathbb C}$ are real symmetric invariant forms, while $\kappa_{\mathbb R}=2\operatorname{Re}\kappa_{\mathbb C}$. With $H=\operatorname{diag}(1,-1)$, the [Killing form of the special linear Lie algebra](../../../../../killing-form-of-the-special-linear-lie-algebra.md) gives $\kappa_{\mathbb C}(H,H)=8$ and $\kappa_{\mathbb C}(H,iH)=8i$. Therefore the imaginary part cannot be a real multiple of $\kappa_{\mathbb R}$. The uniqueness conclusion requires the customary complex-simple or compact-real interpretation.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
