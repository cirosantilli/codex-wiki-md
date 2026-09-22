<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [one-dimensional Sobolev representative](../../../../../one-dimensional-sobolev-representative.md) is absolutely continuous. For $x<y$, the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) and [Holder inequality](../../../../../holder-inequality.md) give

$$
|u(y)-u(x)|\leq\int_x^y|u'(s)|ds
\leq\|u'\|_{L^q(0,1)}|y-x|^{1-1/q}.
$$

Thus **$u$ has a representative in $C^{0,1-1/q}([0,1])$**. The qualification about representatives matters because a [Sobolev space](../../../../../sobolev-space-split.md) element is an almost-everywhere equivalence class.

In two dimensions, the [Sobolev fundamental theorem of calculus on lines](../../../../../sobolev-fundamental-theorem-of-calculus-on-lines.md) and [Fubini's theorem](../../../../../fubini-s-theorem.md) imply that almost every horizontal and vertical slice belongs to $W^{1,q}(0,1)$ and has this one-dimensional [Hölder continuity](../../../../../holder-condition.md). The slice seminorm depends on the slice; this does not give one uniform pointwise estimate on the square. For $q>2$, [Morrey's inequality](../../../../../morrey-s-inequality.md) additionally gives a globally [Hölder continuous](../../../../../holder-condition.md) representative of exponent $1-2/q$. For $1<q\leq2$, global continuity need not hold. For example, with a smooth cutoff around an interior point, $u(x)=|x-x_0|^{-a}$ lies in $W^{1,q}$ when $0<a<2/q-1$, but is unbounded. At $q=2$, the cutoff version of $\log\log(e/|x-x_0|)$ is unbounded while its [gradient](../../../../../gradient.md) has finite squared integral, since

$$
\int_0^\varepsilon\frac{dr}{r\log^2(e/r)}<\infty.
$$

These examples distinguish [Sobolev slicing and planar continuity](../../../../../sobolev-slicing-and-planar-continuity.md) from a false two-dimensional application of the interval exponent.

Put $\Omega=(0,1)^2$. A [BV space](../../../../../function-of-bounded-variation-on-a-domain.md) is a function $u\in L^1(\Omega)$ whose [distributional derivative](../../../../../distributional-derivative.md) $Du$ is a finite vector-valued [Radon measure](../../../../../radon-measure.md). Equivalently its [total variation seminorm](../../../../../total-variation-seminorm-on-a-domain.md) is finite:

$$
\boxed{|Du|(\Omega)=\sup_{\substack{\varphi\in C_c^1(\Omega;\mathbb R^2)\\|\varphi(x)|\leq1}}
\int_\Omega u\,\operatorname{div}\varphi\,dx.}
$$

The [BV space](../../../../../function-of-bounded-variation-on-a-domain.md) has [norm](../../../../../norm.md) $\|u\|_{L^1}+|Du|(\Omega)$. For $u\in W^{1,1}(\Omega)$, [integration by parts](../../../../../integration-by-parts.md) against the compactly supported field gives $\int u\operatorname{div}\varphi=-\int\nabla u\cdot\varphi\leq\int|\nabla u|$. Conversely the measurable choice $\varphi=-\nabla u/|\nabla u|$ on nonzero [gradients](../../../../../gradient.md) attains the pointwise bound. Approximating this bounded field by smooth fields, using interior cutoffs and the finite [measure](../../../../../measure.md) $|\nabla u|dx$, justifies the [supremum](../../../../../supremum.md) and gives

$$
\boxed{|Du|(\Omega)=\int_\Omega|\nabla u|dx.}
$$

It is a [norm](../../../../../norm.md) of the [derivative](../../../../../derivative.md) [measure](../../../../../measure.md), rather than a pointwise [derivative](../../../../../derivative.md) at jump discontinuities.

There is a genuine mismatch in the printed definition of the next [functional](../../../../../functional.md). Its constraints on $\varphi_0$ and $\varphi$ are independent. Hence its stated [supremum](../../../../../supremum.md), denoted $A_{\mathrm{box}}$, separates as

$$
\boxed{A_{\mathrm{box}}(u)=|\Omega|+|Du|(\Omega).}
$$

The scalar [supremum](../../../../../supremum.md) is $|\Omega|$, by cutoffs approaching one, and the vector [supremum](../../../../../supremum.md) is the variation. For an affine [image signal](../../../../../image-signal.md) with $|\nabla u|=1$, this gives $2|\Omega|$, whereas the displayed square-root area would give $\sqrt2|\Omega|$. The intended [relaxed graph-area functional](../../../../../relaxed-graph-area-functional.md) instead uses the coupled pointwise constraint $\varphi_0^2+|\varphi|^2\leq1$, giving

$$
A(u)=\int_\Omega\sqrt{1+|\nabla u|^2}\,dx+|D^su|(\Omega),
$$

where $D^su$ is the singular part of $Du$. Both readings have a [minimizer](../../../../../global-minimizer.md), but their equations are different.

Here is the [direct method in the calculus of variations](../../../../../direct-method-in-the-calculus-of-variations.md) for either reading. Let $A_\bullet$ be the literal $A_{\mathrm{box}}$ or the corrected $A$, and define the energy on $BV(\Omega)\cap L^2(\Omega)$, assigning infinity elsewhere. A [minimizing sequence](../../../../../minimizing-sequence.md) has bounded energy by comparison with $u=0$. Both $A_\bullet\geq|Du|(\Omega)$, so its variation is bounded, and the fidelity bounds $\|u-g\|_2$, hence also $\|u\|_2$ and $\|u\|_1$. By [bounded-variation compactness](../../../../../bounded-variation-compactness.md), a subsequence converges strongly in $L^1$ to $u\in BV$, and after another subsequence almost everywhere. [Fatou's lemma](../../../../../fatou-s-lemma.md) proves

$$
\int_\Omega(u-g)^2\leq\liminf_j\int_\Omega(u_j-g)^2.
$$

The regularizer is a [supremum](../../../../../supremum.md) of affine [functionals](../../../../../functional.md) continuous in $L^1$, since the test-field divergence is bounded. It is therefore [lower semicontinuous](../../../../../lower-semicontinuity.md). Combining the two lower bounds proves **existence of a [minimizer](../../../../../global-minimizer.md)**. In fact the convex regularizer and the [strictly convex](../../../../../strictly-convex-function.md) squared fidelity make the [minimizer](../../../../../global-minimizer.md) unique up to null sets. This does not assert that the [minimizer](../../../../../global-minimizer.md) must belong to $W^{1,1}$.

For the intended graph area, conditionally assume that the [minimizer](../../../../../global-minimizer.md) is in $W^{1,1}$. For $\eta\in C_c^\infty(\Omega)$, differentiate at $u+t\eta$. The [derivative](../../../../../derivative.md) of the integrand is bounded by $|\nabla\eta|$, so dominated convergence applies. The weak equation is

$$
\alpha\int_\Omega\frac{\nabla u\cdot\nabla\eta}{\sqrt{1+|\nabla u|^2}}dx
+\int_\Omega(u-g)\eta\,dx=0,
$$

that is,

$$
\boxed{u-g-\alpha\operatorname{div}\frac{\nabla u}{\sqrt{1+|\nabla u|^2}}=0
\quad\hbox{in }\mathcal D'(\Omega).}
$$

This is the [graph-area Euler-Lagrange equation](../../../../../graph-area-euler-lagrange-equation.md). Compactly supported variations impose no boundary condition in this statement.

For the literal printed [supremum](../../../../../supremum.md), the constant $|\Omega|$ drops out and one obtains [total variation denoising](../../../../../total-variation-denoising.md). Its [total variation calibration](../../../../../total-variation-calibration.md) form is

$$
\boxed{u-g-\alpha\operatorname{div}z=0,\qquad
|z|\leq1,\qquad z\cdot\nabla u=|\nabla u|\ \hbox{a.e.}}
$$

The distributional equation means $\alpha\int z\cdot\nabla\eta+\int(u-g)\eta=0$. In particular $z=\nabla u/|\nabla u|$ wherever the [gradient](../../../../../gradient.md) is nonzero; writing this quotient without handling zero [gradients](../../../../../gradient.md) would be incomplete. Formally the one-sided [derivative](../../../../../derivative.md) of $\int|\nabla u|$ is

$$
\int_{\{\nabla u\ne0\}}\frac{\nabla u}{|\nabla u|}\cdot\nabla\eta
+\int_{\{\nabla u=0\}}|\nabla\eta|.
$$

Minimality in the directions $\eta$ and $-\eta$ bounds the remaining linear [functional](../../../../../functional.md) by the second integral. The [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) extends it on that zero-gradient set to a bounded vector field of magnitude at most one, furnishing $z$ and the displayed weak equation. Thus the literal definition has a nonsmooth [subgradient](../../../../../subgradient.md) equation, not the square-root equation above.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
