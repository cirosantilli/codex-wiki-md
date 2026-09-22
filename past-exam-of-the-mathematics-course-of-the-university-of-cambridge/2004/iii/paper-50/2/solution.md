<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Work with the local [Wilsonian effective action](../../../../../wilsonian-effective-action.md), retaining the elementary [chiral superfield](../../../../../chiral-superfield.md) and using a nonzero infrared cutoff. Its [superpotential](../../../../../superpotential.md) is holomorphic in both the field and chiral [spurions](../../../../../spurion.md) representing the couplings. A convenient pair of [spurion](../../../../../spurion.md) symmetries assigns charges

$$
\boxed{\begin{array}{c|rrrrr}
&\Phi&m&g&\theta&W\\\hline
U(1)&1&-2&-3&0&0\\
U(1)_R&3&-4&-7&1&2
\end{array}}
$$

Both couplings and $\Phi$ transform nontrivially under each displayed symmetry. Each [superpotential](../../../../../superpotential.md) monomial has ordinary charge zero and [R-charge](../../../../../r-charge.md) two, so the integral $\int d^2\theta\,W$ is invariant. This R assignment differs from the conventional $(1,0,-1)$ assignment for $(\Phi,m,g)$ by twice the ordinary charge, and describes the same two-dimensional charge space. These are formal [spurion](../../../../../spurion.md) symmetries; fixing the couplings to numerical values need not leave them as actual symmetries of the fields alone.

For $m\ne0$, $m\Phi^2$ has the required charges and mass dimension three, while $z=g\Phi/m$ has zero charge under both symmetries and is dimensionless. Thus the allowed holomorphic form is

$$
\boxed{W_{\mathrm{eff}}=m\Phi^2F\left(\frac{g\Phi}{m}\right).}
$$

One can see its generality directly. A holomorphic monomial $\Phi^u m^v g^w$ must obey $u-2v-3w=0$ and $3u-4v-7w=2$. Solving gives $u=w+2$ and $v=1-w$, hence precisely $m\Phi^2(g\Phi/m)^w$. A field-independent constant is irrelevant to this global supersymmetric action and can be dropped.

The symmetries alone leave the function arbitrary. To determine its perturbative form, use regularity as well as the two limits. A regular weak-coupling expansion at $g=0$ has

$$
F(z)=\sum_{r\ge0}c_rz^r,\qquad
W_{\mathrm{eff}}=\sum_{r\ge0}c_r g^r m^{1-r}\Phi^{r+2}.
$$

The $g\to0$ limit is a free massive theory, so $c_0=1/2$. Since the elementary field has not been integrated out, the Wilsonian [superpotential](../../../../../superpotential.md) must remain regular term by term as $m\to0$ with the infrared cutoff fixed. Every term with $r\ge2$ would introduce a pole in $m$ and is excluded. Negative powers of $g$ were already excluded by perturbative regularity at $g=0$. Consequently $F=c_0+c_1z$.

At $m=0$, the only surviving allowed interaction is proportional to $g\Phi^3$. Its coefficient is first order in $g$, and matching the tree three-field vertex gives $c_1=1/3$. No closed-loop three-field diagram can be made from a single cubic vertex; extra interaction vertices would produce higher coupling order. Equivalently free superspace propagators join chiral to antichiral fields, so a closed loop would require additional vertices or conjugate couplings, which the holomorphic charge constraints exclude for this term. This fixes the coefficient without assuming the desired conclusion. Therefore

$$
\boxed{F(z)=\frac12+\frac z3,\qquad
W_{\mathrm{eff}}^{\mathrm{pert}}=\frac12m\Phi^2+\frac13g\Phi^3=W_{\mathrm{tree}}.}
$$

The regularity condition is essential: it concerns the local Wilsonian [superpotential](../../../../../superpotential.md) with the field retained, not a nonlocal one-particle-irreducible functional at zero infrared cutoff or a [superpotential](../../../../../superpotential.md) obtained by eliminating a massive field. Such different operations can generate inverse masses or infrared singularities without contradicting this proof.

The [Kähler potential](../../../../../kahler-potential.md) is a real [D-term](../../../../../d-term.md), not a holomorphic [F-term](../../../../../f-term.md), and is not protected by this argument. For example its quadratic part becomes $Z(g,\bar g,m,\bar m;\mu)\Phi^\dagger\Phi$, with higher real operators also allowed. Terms involving $|g|^2$ are compatible with the symmetries and produce [wave-function renormalization](../../../../../wave-function-renormalization.md). After the canonical rescaling $\Phi_c=Z^{1/2}\Phi$, the parameters in the [superpotential](../../../../../superpotential.md) expressed using canonical fields are $m_c=m/Z$ and $g_c=g/Z^{3/2}$, so physical couplings can run despite the holomorphic non-renormalization statement.

**[Holomorphy](../../../../../holomorphic-function.md) is crucial.** Without it, neutral factors such as $1+c|g|^2$ could multiply either [superpotential](../../../../../superpotential.md) monomial while respecting both [spurion](../../../../../spurion.md) symmetries. Excluding conjugate couplings, together with regularity and tree matching, is what turns the charge argument into the [non-renormalization theorem](../../../../../non-renormalization-theorem.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 50](../../paper-50-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
