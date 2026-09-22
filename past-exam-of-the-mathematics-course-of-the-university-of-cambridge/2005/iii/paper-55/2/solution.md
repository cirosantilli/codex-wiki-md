<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a [chiral superfield](../../../../../chiral-superfield.md) of [mass dimension](../../../../../mass-dimension.md) one, a [renormalizable quantum field theory](../../../../../renormalizable-quantum-field-theory.md) has a quadratic [Kähler potential](../../../../../kahler-potential.md) and a [superpotential](../../../../../superpotential.md) of degree at most three. Before canonical normalization one may write

$$
K=Z\Phi^\dagger\Phi+[k_1\Phi+k_2\Phi^2+\mathrm{h.c.}]+k_0,\qquad Z>0,
$$

with real $k_0$, and

$$
W=w_0+\ell\Phi+\frac m2\Phi^2+\frac g3\Phi^3.
$$

The purely holomorphic terms in $K$, their conjugates and its constant have vanishing full [superspace integration](../../../../../superspace-integration.md); they are [Kähler transformations](../../../../../kahler-transformation.md) of the global theory. Rescaling the [chiral superfield](../../../../../chiral-superfield.md) sets $Z=1$, so the physically general kinetic choice is $K=\Phi^\dagger\Phi$ up to these terms. The [constant superpotential in global supersymmetry](../../../../../constant-superpotential-in-global-supersymmetry.md) also has no component effect. The dimensions of $\ell,m,g$ are respectively two, one and zero.

To eliminate the linear term, translate the complex [chiral superfield](../../../../../chiral-superfield.md) as $\Phi=\Phi'+s$. The shifted linear coefficient is

$$
W'(s)=\ell+ms+gs^2.
$$

If $g\ne0$, this quadratic has a root over the complex numbers; if $g=0$ but $m\ne0$, take $s=-\ell/m$. The resulting linear term vanishes and the new quadratic coefficient is $m+2gs$. The canonical [Kähler potential](../../../../../kahler-potential.md) changes only by holomorphic, antiholomorphic and constant terms, which do not change the global kinetic action. This is the [superpotential critical-point shift](../../../../../superpotential-critical-point-shift.md).

**The claim needs an exception:** if $m=g=0$ but $\ell\ne0$, the [superpotential](../../../../../superpotential.md) is purely linear and no invertible translation can remove it. More generally an invertible regular field redefinition cannot turn a nowhere-zero derivative into a critical point. The theory with $W=\ell\Phi$ has $F=-\bar\ell$, a constant positive [scalar potential](../../../../../scalar-potential.md) $|\ell|^2$, and [flat F-term breaking with a linear superpotential](../../../../../flat-f-term-breaking-with-a-linear-superpotential.md). Below, $m$ and $g$ denote the quadratic/cubic coefficients after the valid shift, as intended by the question.

Expand $\Phi=\phi+\sqrt2\theta\psi+\theta^2F$ in chiral coordinates. The highest component of $W(\Phi)$ is $W'(\phi)F-\tfrac12W''(\phi)\psi\psi$, while the full-superspace kinetic term contains $F^*F$. Thus the [auxiliary field](../../../../../auxiliary-field.md) part of the component [Lagrangian](../../../../../lagrangian.md) is

$$
\mathcal L_F=F^*F+(m\phi+g\phi^2)F
+(\bar m\bar\phi+\bar g\bar\phi^2)F^*.
$$

Varying $F$ and $F^*$ independently gives

$$
F^*=-(m\phi+g\phi^2),\qquad F=-(\bar m\bar\phi+\bar g\bar\phi^2).
$$

Substitution gives $\mathcal L_F=-|m\phi+g\phi^2|^2$, and hence the [F-term scalar potential](../../../../../f-term-scalar-potential.md)

$$
\boxed{V(\phi)=|m\phi+g\phi^2|^2.}
$$

It is nonnegative and vanishes at $\phi=0$, and also at $\phi=-m/g$ when $g\ne0$. These are [supersymmetric vacua](../../../../../supersymmetric-vacuum.md), since the [auxiliary field](../../../../../auxiliary-field.md) vanishes. Thus **the quadratic/cubic model does not spontaneously break supersymmetry**. If $m=0$ but $g\ne0$, zero is the sole critical point; if both vanish, every $\phi$ is a zero-energy vacuum. Nonzero $m,g$ give the usual two vacua, coinciding when $m=0$.

For the loop argument, promote the coefficients to background chiral [spurions](../../../../../spurion.md). One convenient pair of independent formal $U(1)$ charge assignments is

$$
\begin{array}{c|rrrr|r}
&\Phi&m&g&\theta&W\\\hline
U(1)&1&-2&-3&0&0\\
U(1)_R&2&-2&-4&1&2
\end{array}.
$$

Both symmetries act nontrivially on all three of $\Phi,m,g$; the second is an [R-symmetry](../../../../../r-symmetry.md). The [superspace integration](../../../../../superspace-integration.md) measure $d^2\theta$ has [R-charge](../../../../../r-charge.md) $-2$, so both tree monomials give invariant actions. These are spurionic selection rules, not necessarily actual symmetries after fixing numerical couplings. The R-row is an ordinary-charge redefinition of the usual [Wess–Zumino spurion charge assignment](../../../../../wess-zumino-spurion-charge-assignment.md).

A local Wilsonian [superpotential](../../../../../superpotential.md) is a [holomorphic function](../../../../../holomorphic-function.md) of the chiral fields and chiral [spurions](../../../../../spurion.md). The ratio $z=g\Phi/m$ is neutral under both charge assignments and has dimension zero, whereas $m\Phi^2$ has exactly the charges and dimension of $W$. The general symmetry-allowed form, on a patch with $m\ne0$ and up to a physically irrelevant global constant, is therefore

$$
\boxed{W_{\mathrm{eff}}=m\Phi^2 f\left(\frac{g\Phi}{m}\right),}
$$

with $f$ holomorphic where that description is regular. Symmetry by itself does not determine $f$.

For a regular perturbative local [Wilsonian effective action](../../../../../wilsonian-effective-action.md) retaining the same elementary field and an infrared cutoff, expand $f(z)=\sum_n c_nz^n$. Its term of order $n$ is $c_n g^n m^{1-n}\Phi^{n+2}$. Negative $n$ are singular in $g$, while $n\geq2$ are singular in $m$; these are excluded by perturbative holomorphic regularity at the free-coupling limits. Thus only the quadratic and cubic terms survive. Their regular holomorphic coefficients cannot acquire coupling-dependent invariant corrections. At $g=0$ the quadratic theory is Gaussian, fixing $c_0=1/2$ exactly. A contribution linear in $g$ to the cubic vertex has only one cubic interaction: three external lines exhaust that vertex, leaving no contraction to form a loop. Thus $c_1=1/3$ as well in the present normalization. This supplies the [holomorphy argument for superpotential non-renormalization](../../../../../holomorphy-argument-for-superpotential-non-renormalization.md) rather than concluding non-renormalization from symmetry alone.

The [Kähler potential](../../../../../kahler-potential.md) can still undergo [wave-function renormalization](../../../../../wave-function-renormalization.md). If its quadratic coefficient becomes $Z$, canonical normalization gives $m_c=m/Z$ and $g_c=g/Z^{3/2}$, so physical masses and interactions can run despite [superpotential non-renormalization](../../../../../non-renormalization-theorem.md). More generally a positive nonsingular effective [Kähler metric](../../../../../kahler-metric.md) replaces $V$ by $K^{\phi\bar\phi}|W'(\phi)|^2$ and does not remove its zero-energy critical points. Infrared-singular nonlocal one-particle-irreducible terms and eliminating the entire massive field are outside this Wilsonian statement.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
