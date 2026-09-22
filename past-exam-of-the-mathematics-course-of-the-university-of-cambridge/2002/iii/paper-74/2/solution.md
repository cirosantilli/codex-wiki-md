<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [exterior derivative](../../../../../exterior-derivative.md) is a linear map $d:\Omega^k(M)\to\Omega^{k+1}(M)$, agrees with the ordinary differential on functions, satisfies $d^2=0$, and obeys the graded [Leibniz rule](../../../../../leibniz-rule.md)

$$
d(\alpha\wedge\beta)=d\alpha\wedge\beta+(-1)^k\alpha\wedge d\beta\qquad(\alpha\in\Omega^k).
$$

In local coordinates it differentiates the coefficient functions:

$$
d\left(\frac1{k!}\alpha_{i_1\cdots i_k}dx^{i_1}\wedge\cdots\wedge dx^{i_k}\right)
=\frac1{k!}\partial_j\alpha_{i_1\cdots i_k}dx^j\wedge dx^{i_1}\wedge\cdots\wedge dx^{i_k}.
$$

Antisymmetry cancels the second partial derivatives, proving $d^2=0$ locally. These properties determine the coordinate-independent derivative.

For any smooth $\phi:N\to M$, the [pullback of a differential form](../../../../../pullback-of-a-differential-form.md) is defined by

$$
(\phi^*\alpha)_x(v_1,\ldots,v_k)
=\alpha_{\phi(x)}(d\phi_xv_1,\ldots,d\phi_xv_k).
$$

There is no requirement that $\phi$ be invertible or an immersion. Pullback preserves wedge products and sends $df$ to $d(f\circ\phi)$ by the chain rule. Locally every form is a sum of $f\,dx^{i_1}\wedge\cdots\wedge dx^{i_k}$; applying the preceding identities and $d^2\phi^i=0$ proves

$$
\boxed{d(\phi^*\alpha)=\phi^*(d\alpha).}
$$

Describe the [brane](../../../../../brane.md) by an embedding $X:\Sigma\to M$, with nondegenerate [induced worldvolume metric](../../../../../induced-worldvolume-metric.md) $h=X^*g$. Locally the [Poincaré lemma](../../../../../poincare-lemma.md) gives $F=dA$ because $F$ is a [closed differential form](../../../../../closed-differential-form.md). For a timelike worldvolume, the geometric area and [Wess-Zumino brane coupling](../../../../../wess-zumino-brane-coupling.md) give the action

$$
\boxed{S[X]=-T\int_\Sigma d^{p+1}\sigma\,\sqrt{|\det h|}
+q\int_\Sigma X^*A,\qquad
h_{\alpha\beta}=g_{\mu\nu}(X)\partial_\alpha X^\mu\partial_\beta X^\nu.}
$$

$T$ is the [brane tension](../../../../../brane-tension.md) and $q$ the charge in this normalization. The geometric term is the higher-dimensional version of the [Nambu–Goto action](../../../../../nambu-goto-action.md). Both integrals are invariant under changes of worldvolume coordinates.

The additive gauge transformation is $A\mapsto A+d\Lambda$. Its change of action is

$$
\delta_\Lambda S=q\int_\Sigma X^*d\Lambda
=q\int_\Sigma d(X^*\Lambda)
=q\int_{\partial\Sigma}X^*\Lambda.
$$

The last step is the [Generalized Stokes theorem](../../../../../generalized-stokes-theorem.md). It vanishes for a closed worldvolume, or with suitable boundary restrictions. An open worldvolume can instead have a compensating boundary coupling, as in [gauge invariance of an open-brane coupling](../../../../../gauge-invariance-of-an-open-brane-coupling.md).

More directly, for a variation vector $V$ of the embedding, [Cartan's magic formula](../../../../../cartan-s-magic-formula.md) gives

$$
\delta\int_\Sigma X^*A
=\int_\Sigma X^*(\iota_VF)+\int_{\partial\Sigma}X^*(\iota_VA).
$$

Thus the interior force depends on $F$, not the gauge potential. Define the trace of the [second fundamental form](../../../../../second-fundamental-form-split.md) by

$$
K^\mu=\frac1{\sqrt{|h|}}\partial_\alpha\left(\sqrt{|h|}h^{\alpha\beta}\partial_\beta X^\mu\right)
+\Gamma^\mu_{\nu\rho}h^{\alpha\beta}\partial_\alpha X^\nu\partial_\beta X^\rho.
$$

The area variation is $-\int\sqrt{|h|}\,g(V,K)$ plus a boundary term. For compactly supported interior variations the resulting equations are

$$
\boxed{T\sqrt{|h|}\,K_\mu
+\frac{q}{(p+1)!}\varepsilon^{\alpha_0\cdots\alpha_p}
F_{\mu\nu_0\cdots\nu_p}\partial_{\alpha_0}X^{\nu_0}\cdots\partial_{\alpha_p}X^{\nu_p}=0.}
$$

They exhibit the [field-strength force on a charged brane](../../../../../field-strength-force-on-a-charged-brane.md) and are gauge invariant.

Two global qualifications are necessary. First, replacing $A$ by $d\Lambda$ alone, as printed, gives $dA'=0$ and would erase a nonzero $F$; **the intended transformation must be the additive shift** above. Second, closedness of $F$ only guarantees a potential locally. If a global potential does not exist and the worldvolume bounds a filling $B$, its charged term can be defined as $q\int_B F$. Different fillings differ by a period of $F$; independence of the quantum phase requires $q\int_C F\in2\pi\hbar\mathbb Z$ for the corresponding closed cycles. Without the required global potential or patching/filling data, the given closed form still defines the local variational equations, but not automatically a single globally defined real-valued action.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
