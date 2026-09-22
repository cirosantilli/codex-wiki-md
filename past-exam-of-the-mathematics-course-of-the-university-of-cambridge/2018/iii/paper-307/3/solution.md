<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the canonical [Kähler potential](../../../../../kahler-potential.md) and normalize [superspace integration](../../../../../superspace-integration.md) by $\int d^2\theta\,\theta^2=1$. The [superspace](../../../../../superspace.md) [Lagrangian density](../../../../../lagrangian-density.md) is

$$
\boxed{\mathcal L=\int d^4\theta\,\Phi^\dagger\Phi+
\left[\int d^2\theta\left(\frac m2\Phi^2+\frac g3\Phi^3\right)+\mathrm{h.c.}\right].}
$$

The full [superspace integration](../../../../../superspace-integration.md) produces a [D-term](../../../../../d-term.md), while the [chiral superfield](../../../../../chiral-superfield.md) integral produces an [F-term](../../../../../f-term.md). Work in chiral coordinates for the [chiral-superfield component expansion](../../../../../chiral-superfield-component-expansion.md), so the omitted spacetime-derivative terms do not enter the extraction of $F$.

Set $\delta\Phi=\sqrt2\theta\psi+\theta^2F$. A [Taylor expansion](../../../../../taylor-expansion.md) of the [superpotential](../../../../../superpotential.md) gives

$$
W(\varphi+\delta\Phi)=W(\varphi)+W'(\varphi)\delta\Phi+
\frac12W''(\varphi)(\delta\Phi)^2.
$$

Higher terms vanish because there are only two [Grassmann variables](../../../../../grassmann-variable.md) $\theta^\alpha$. With $\theta\psi=\theta^\alpha\psi_\alpha$ and $\psi\psi=\psi^\alpha\psi_\alpha$, their anticommutation gives $(\theta\psi)^2=-\tfrac12\theta^2\psi\psi$. Thus

$$
\left.W(\Phi)\right|_{\theta^2}=F W'(\varphi)-\frac12W''(\varphi)\psi\psi,
\qquad W'=m\varphi+g\varphi^2,\qquad W''=m+2g\varphi.
$$

The canonical [Kähler potential](../../../../../kahler-potential.md) contributes $F^*F$. Consequently the part of the [Lagrangian density](../../../../../lagrangian-density.md) containing the [auxiliary field](../../../../../auxiliary-field.md) is

$$
\boxed{\mathcal L_F=F^*F+F(m\varphi+g\varphi^2)
+F^*(m^*\varphi^*+g^*\varphi^{*2}).}
$$

The [fermion](../../../../../fermion.md) terms coming from the [superpotential](../../../../../superpotential.md) are

$$
\mathcal L_{\mathrm{mass+Yukawa}}=-\frac12(m+2g\varphi)\psi\psi
-\frac12(m^*+2g^*\varphi^*)\bar\psi\bar\psi.
$$

The [Weyl spinor](../../../../../weyl-spinor.md) kinetic term and the [complex scalar field](../../../../../complex-scalar-field.md) kinetic term are canonical because $K=\Phi^\dagger\Phi$.

Treat $F$ and $F^*$ as independent variables in their algebraic [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md). They give

$$
F^*=-W'(\varphi),\qquad F=-\overline{W'(\varphi)}.
$$

Equivalently,

$$
\mathcal L_F=\bigl|F+\overline{W'(\varphi)}\bigr|^2-|W'(\varphi)|^2.
$$

After eliminating the [auxiliary field](../../../../../auxiliary-field.md), the [Lagrangian density](../../../../../lagrangian-density.md) contains $-V$, so the [F-term scalar potential](../../../../../f-term-scalar-potential.md) is

$$
\boxed{V(\varphi)=|m\varphi+g\varphi^2|^2
=|m|^2|\varphi|^2+m^*g\varphi^*\varphi^2
+mg^*\varphi\varphi^{*2}+|g|^2|\varphi|^4\geq0.}
$$

It is nonnegative for arbitrary complex $m,g,\varphi$, since it is a [modulus](../../../../../modulus.md) squared. A [supersymmetric vacuum](../../../../../supersymmetric-vacuum.md) satisfies [F-flatness](../../../../../f-flatness.md), so its zeros are:

$$
\varphi=0,\qquad \varphi=-\frac m g\quad(g\ne0).
$$

If $m=0$ and $g\ne0$ these coincide; if $g=0$ and $m\ne0$ only the origin remains; if $m=g=0$ every constant $\varphi$ is a [supersymmetric vacuum](../../../../../supersymmetric-vacuum.md).

To compare masses, expand around a [supersymmetric vacuum](../../../../../supersymmetric-vacuum.md) $v$ satisfying $W'(v)=0$, writing $\varphi=v+\eta$. With $M=W''(v)=m+2gv$,

$$
W'(v+\eta)=M\eta+g\eta^2,\qquad
V=|M|^2|\eta|^2+\text{terms of degree at least three},
\qquad \mathcal L_{\mathrm{fermion\ mass}}=-\frac12M\psi\psi+\mathrm{h.c.}
$$

Writing $\eta=(A+iB)/\sqrt2$ gives the [scalar field](../../../../../scalar-field.md) mass term $-\tfrac12|M|^2(A^2+B^2)$; the [Weyl spinor](../../../../../weyl-spinor.md) has physical mass $|M|$. Therefore the [supersymmetric mass degeneracy](../../../../../supersymmetric-mass-degeneracy.md) is

$$
\boxed{m_A^2=m_B^2=|W''(v)|^2,\qquad m_\psi=|W''(v)|.}
$$

In particular, at $v=0$ the [boson](../../../../../boson.md) and [fermion](../../../../../fermion.md) masses are both $|m|$. At the second [supersymmetric vacuum](../../../../../supersymmetric-vacuum.md) $v=-m/g$ the sign of $M$ reverses, but the physical mass is again $|m|$. Equality here concerns fluctuations about a [supersymmetric vacuum](../../../../../supersymmetric-vacuum.md), not arbitrary backgrounds with $W'(v)\ne0$.

In the convention $V\supset\lambda|\varphi|^4$ and $\mathcal L_{\mathrm{Yukawa}}=-y\varphi\psi\psi+\mathrm{h.c.}$, the same [superpotential](../../../../../superpotential.md) coefficient gives $\lambda=|g|^2$ and $y=g$. The [supersymmetric relation between quartic and Yukawa couplings](../../../../../supersymmetric-relation-between-quartic-and-yukawa-couplings.md) is therefore

$$
\boxed{\lambda=|y|^2.}
$$

If instead the [Yukawa interaction](../../../../../yukawa-interaction.md) is written $-\tfrac12y_3\varphi\psi\psi+\mathrm{h.c.}$, then $y_3=2g$ and the same physical relation is $\lambda=|y_3|^2/4$. The numerical factor depends on the definition of the [Yukawa coupling](../../../../../yukawa-interaction.md).

The perturbative [non-renormalization theorem](../../../../../non-renormalization-theorem.md) applies to the local [holomorphic](../../../../../complex-differentiability-at-a-point.md) [superpotential](../../../../../superpotential.md) in the [Wilsonian effective action](../../../../../wilsonian-effective-action.md), using [regularization in quantum field theory](../../../../../regularization-in-quantum-field-theory.md) that preserves [supersymmetry](../../../../../supersymmetry-split.md). There are two complementary ways to see why it applies here.

First, in [supergraph](../../../../../supergraph.md) calculations in [perturbative quantum field theory](../../../../../perturbative-quantum-field-theory-split.md), the algebra of [supersymmetric covariant derivatives](../../../../../supersymmetric-covariant-derivative.md) puts any candidate local correction to the [superpotential](../../../../../superpotential.md) into a full $d^4\theta$ [superspace integration](../../../../../superspace-integration.md). It therefore corrects a [D-term](../../../../../d-term.md), such as the [Kähler potential](../../../../../kahler-potential.md), rather than a local chiral $d^2\theta$ [F-term](../../../../../f-term.md). Turning such a contribution into an apparent chiral integral would require nonlocal inverse spacetime derivatives, schematically $1/\Box$. These are excluded from the local [Wilsonian effective action](../../../../../wilsonian-effective-action.md) with a fixed nonzero momentum cutoff. This gives the diagrammatic [non-renormalization theorem](../../../../../non-renormalization-theorem.md).

Second, the [holomorphy argument for superpotential non-renormalization](../../../../../holomorphy-argument-for-superpotential-non-renormalization.md) treats $m$ and $g$ as background chiral [spurions](../../../../../spurion.md), so the [Wilsonian effective action](../../../../../wilsonian-effective-action.md) [superpotential](../../../../../superpotential.md) is a [holomorphic function](../../../../../holomorphic-function.md) of $\Phi,m,g$, with no dependence on $m^*$ or $g^*$. Assign an ordinary $U(1)$ spurion charge and an [R-charge](../../../../../r-charge.md) as follows:

$$
\begin{array}{c|cccc}
&\Phi&m&g&\theta\\\hline
U(1)&1&-2&-3&0\\
R&1&0&-1&1
\end{array}
$$

The [superpotential](../../../../../superpotential.md) has ordinary charge zero and [R-charge](../../../../../r-charge.md) two, since $d^2\theta$ has [R-charge](../../../../../r-charge.md) minus two. A prospective [holomorphic](../../../../../complex-differentiability-at-a-point.md) monomial $m^a g^b\Phi^c$ must therefore satisfy

$$
c-2a-3b=0,\qquad c-b=2,
\qquad\text{hence}\qquad a=3-c,\quad b=c-2.
$$

For perturbative corrections, regularity at $m=0$ and $g=0$ requires nonnegative powers of the couplings. Regularity in $m$ is justified by keeping a nonzero Wilsonian momentum cutoff and retaining $\Phi$ as a light field. Hence only $c=2$ and $c=3$ survive: the existing $m\Phi^2$ and $g\Phi^3$ structures. The quadratic coefficient is fixed by the free theory at $g=0$, where there are no interaction loops. The cubic coefficient is fixed at first order in $g$, where a connected three-field interaction has only its [tree-level Feynman diagram](../../../../../tree-level-feynman-diagram.md); loop corrections would require further powers of the interaction couplings, which the [holomorphy argument for superpotential non-renormalization](../../../../../holomorphy-argument-for-superpotential-non-renormalization.md) charge constraints forbid. Thus

$$
\boxed{W_{\mathrm{Wilsonian}}(\Phi)=\frac m2\Phi^2+\frac g3\Phi^3
\quad\text{to all perturbative orders in holomorphic variables}.}
$$

A field-independent constant is physically irrelevant in this rigid model; the spurion charges would in any case require $m^3/g^2$, which is not regular at $g=0$.

The [Kähler potential](../../../../../kahler-potential.md) can still receive [wave-function renormalization](../../../../../wave-function-renormalization.md). For example, $K=Z\Phi^\dagger\Phi+\cdots$ gives the [canonical field normalization](../../../../../canonical-field-normalization.md) $\Phi_c=Z^{1/2}\Phi$, and consequently

$$
m_c=\frac m Z,\qquad g_c=\frac g{Z^{3/2}}.
$$

These canonically normalized parameters can run with the [renormalization scale](../../../../../renormalization-scale.md); this does not contradict the [holomorphic](../../../../../complex-differentiability-at-a-point.md) [non-renormalization theorem](../../../../../non-renormalization-theorem.md). When massless modes are included in the full [quantum effective action](../../../../../effective-action.md), nonlocal terms associated with [infrared divergences](../../../../../infrared-divergence.md) can also imitate an [F-term](../../../../../f-term.md). Distinguishing that action from the local [Wilsonian effective action](../../../../../wilsonian-effective-action.md) is part of the theorem's convention.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 307](../../paper-307-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
