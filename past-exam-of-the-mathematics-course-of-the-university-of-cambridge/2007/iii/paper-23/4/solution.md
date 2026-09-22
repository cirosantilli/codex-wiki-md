<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $\Omega^1_C=\Omega^1_{C/k}$. A [dualizing sheaf on a smooth projective curve](../../../../../dualizing-sheaf-on-a-smooth-projective-curve.md), for the [vector bundles](../../../../../vector-bundle.md) in this question, consists of a [line bundle](../../../../../line-bundle.md) $D_C$ and a trace $H^1(C,D_C)\to k$ making evaluation induce natural perfect pairings

$$
H^i(C,E)\times H^{1-i}(C,E^\vee\otimes D_C)\longrightarrow k,\qquad i=0,1.
$$

In particular it represents the functor $E\mapsto H^1(C,E)^*$ through $\operatorname{Hom}_C(E,D_C)$. We construct it by reducing to the proved [residue duality on the projective line](../../../../../residue-duality-on-the-projective-line.md).

Choose a separating nonconstant rational function $t$ on $C$. Such a choice exists over any [field](../../../../../field.md) $k$: the function field of a [smooth algebraic curve](../../../../../smooth-algebraic-curve.md) is separably generated of transcendence degree one, and a choice with $dt\ne0$ makes its finite extension of $k(t)$ separable. The map $(t:1)$ extends across poles using $(1:t^{-1})$ in the [discrete valuation ring](../../../../../discrete-valuation-ring.md) at each point. It gives a finite generically separable morphism

$$
f:C\longrightarrow\mathbb P^1_k.
$$

Indeed it is nonconstant, hence has finite fibres, and is proper; a proper quasi-finite morphism is finite. This finite map is flat: locally its direct-image module is finite and torsion-free over a [discrete valuation ring](../../../../../discrete-valuation-ring.md), and hence free. The same argument works componentwise if needed.

For an affine chart $\operatorname{Spec}B\subset\mathbb P^1$ with inverse image $\operatorname{Spec}A$, form the $A$-[module](../../../../../module-mathematics.md)

$$
W=\operatorname{Hom}_B(A,B),\qquad(a\lambda)(a')=\lambda(aa').
$$

These modules glue to the relative trace-dual sheaf $W_f$ on $C$. There are two algebraic identities used here. First, finite-map adjunction gives

$$
\operatorname{Hom}_A(M,\operatorname{Hom}_B(A,N))\cong\operatorname{Hom}_B(M,N).
$$

The forward map evaluates at $1$; the inverse sends $g$ to $m\mapsto(a\mapsto g(am))$. Second, the different–differential identity for a finite generically separable map between smooth curves gives

$$
W_f\otimes f^*\Omega^1_{\mathbb P^1/k}\cong\Omega^1_{C/k}.
$$

To explain its algebraic content, the field trace identifies $\operatorname{Hom}_B(A,B)$ with the inverse [different ideal](../../../../../different-ideal.md), while the different is the vanishing ideal of $f^*\Omega^1_{\mathbb P^1/k}\to\Omega^1_{C/k}$. These identities include wild ramification; one must not replace the different by just ramification index minus one. This is the identity allowed to be quoted in the question; the finite-map description is recorded in [Stacks Project, finite morphisms](https://stacks.math.columbia.edu/tag/0FKW), and its differential form in [Stacks Project, Section 53.12](https://stacks.math.columbia.edu/tag/0C1B).

Set $D_C=W_f\otimes f^*\Omega^1_{\mathbb P^1/k}$. The second identity shows it is a [line bundle](../../../../../line-bundle.md) and already identifies it with $\Omega^1_C$. For a [vector bundle](../../../../../vector-bundle.md) $E$, the first identity gives the sheaf isomorphism

$$
f_*(E^\vee\otimes D_C)\cong\mathcal H om_{\mathbb P^1}(f_*E,\Omega^1_{\mathbb P^1/k})=(f_*E)^\vee\otimes\Omega^1_{\mathbb P^1/k}.
$$

The sheaf $f_*E$ is [locally free](../../../../../locally-free-sheaf.md): on an affine chart, the projective $A$-module defining $E$ is a summand of $A^r$, and $A$ is finite free over $B$. Since $f$ is finite, affine-cover [Čech cohomology](../../../../../cech-cohomology.md) identifies $H^j(C,F)$ with $H^j(\mathbb P^1,f_*F)$ for each of these sheaves. Apply the already established duality on $\mathbb P^1$ to $f_*E$. It gives

$$
\boxed{H^i(C,E)\cong H^{1-i}(C,E^\vee\otimes D_C)^*,\qquad D_C\cong\Omega^1_{C/k},\quad i=0,1.}
$$

The trace is obtained by evaluating the trace-dual module at $1$ and then using the trace $H^1(\mathbb P^1,\Omega^1_{\mathbb P^1/k})\to k$. The adjunction formulas show the displayed isomorphisms are induced by evaluation against this trace and are natural in $E$. They thus establish the requested dualizing property, not merely the existence of an invertible differential sheaf. Uniqueness follows from the [Yoneda lemma](../../../../../yoneda-lemma.md) applied to the representing functor on [vector bundles](../../../../../vector-bundle.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 23](../../paper-23-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
