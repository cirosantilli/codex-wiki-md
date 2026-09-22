<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use matrix multiplication together with the [wedge product of differential forms](../../../../../wedge-product-of-differential-forms.md), suppressing wedge symbols in this calculation. Set $F=dA+A^2$ and $a=\delta A$. The [gauge field strength](../../../../../gauge-field-strength.md) varies as $\delta F=da+Aa+aA$, the [covariant exterior derivative](../../../../../exterior-covariant-derivative.md) of $a$. The [matrix trace](../../../../../matrix-trace.md) has graded cyclicity, $\operatorname{Tr}(\alpha\beta)=(-1)^{pq}\operatorname{Tr}(\beta\alpha)$ for forms of degrees $p,q$. Thus the [Chern-Simons 5-form](../../../../../chern-simons-5-form.md) can be expanded as

$$
Q_5=\operatorname{Tr}\left(A(dA)^2+\frac32A^3dA+\frac35A^5\right).
$$

For example, the two cross terms in $F^2A$ both become $\operatorname{Tr}(A^3dA)$; combining the remaining two terms gives the displayed coefficients. This expansion keeps track of the noncommuting products rather than treating $A$ as a scalar one-form.

Put $B=dA$. Vary the first term and use the graded [exterior derivative](../../../../../exterior-derivative.md) to move derivatives off $a$:

$$
\begin{aligned}
\delta\operatorname{Tr}(AB^2)
&=\operatorname{Tr}(aB^2+A\,da\,B+AB\,da)\\
&=3\operatorname{Tr}(aB^2)-d\operatorname{Tr}(AaB+ABa)\\
&=3\operatorname{Tr}(aB^2)+d\operatorname{Tr}\bigl[a(BA+AB)\bigr].
\end{aligned}
$$

Here $dB=0$. For the next term use $d(A^3)=BA^2-ABA+A^2B$. Graded cyclicity then gives

$$
\begin{aligned}
\delta\operatorname{Tr}(A^3B)
&=\operatorname{Tr}(aA^2B+AaAB+A^2aB+A^3da)\\
&=2\operatorname{Tr}\bigl[a(A^2B+BA^2)\bigr]+d\operatorname{Tr}(aA^3).
\end{aligned}
$$

Finally all five contributions to $\delta\operatorname{Tr}(A^5)$ are equal under the [matrix trace](../../../../../matrix-trace.md), giving $5\operatorname{Tr}(aA^4)$. Combining these results proves the [variation of the Chern-Simons 5-form](../../../../../variation-of-the-chern-simons-5-form.md):

$$
\boxed{\delta Q_5=3\operatorname{Tr}(aF^2)+d\Theta,\qquad
\Theta=\operatorname{Tr}\left[a\left(FA+AF-\frac12A^3\right)\right].}
$$

Consequently, on an oriented five-manifold $N$,

$$
\boxed{\delta I_{\rm CS}=3\int_N\operatorname{Tr}(\delta A\wedge F\wedge F)+\int_{\partial N}\Theta.}
$$

The boundary term vanishes for a closed manifold, for variations supported in its interior, or when the tangential boundary connection is held fixed. A different boundary variational problem would require boundary conditions or a boundary action as well.

Write $A=A^\alpha T_\alpha$ in a basis of the [Lie algebra](../../../../../lie-algebra-split.md). Independent compactly supported variations of each component yield the bulk [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md)

$$
\boxed{\operatorname{Tr}(T_\alpha F\wedge F)=0\quad\text{for every }\alpha.}
$$

Equivalently, with $d_{\alpha\beta\gamma}=\tfrac12\operatorname{Tr}[T_\alpha\{T_\beta,T_\gamma\}]$, these are $d_{\alpha\beta\gamma}F^\beta\wedge F^\gamma=0$. The symmetry of the two curvature two-forms accounts for the anticommutator. Writing simply $F\wedge F=0$ as a full matrix equation requires an additional assumption: variations must span a matrix algebra paired nondegenerately by the [matrix trace](../../../../../matrix-trace.md). For a smaller [Lie algebra](../../../../../lie-algebra-split.md), only its trace-paired projection is constrained. If the trace is literally taken in the adjoint representation of a [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md), its symmetric cubic invariant vanishes, and these bulk equations are identically zero. Indeed, the adjoint generators are skew with respect to the nondegenerate invariant [Killing form](../../../../../killing-form.md); transposition in this pairing reverses the sign of the symmetrized trace of three generators. The usual nontrivial five-dimensional theory therefore needs an invariant cubic trace that does not vanish; saying that the gauge field transforms in the adjoint alone does not specify such a trace.

Under a [Yang-Mills gauge transformation](../../../../../yang-mills-gauge-transformation.md), use $A^g=g^{-1}Ag+g^{-1}dg$, so $F^g=g^{-1}Fg$. For any Lie-algebra element $T$,

$$
\operatorname{Tr}\bigl(TF^g\wedge F^g\bigr)
=\operatorname{Tr}\bigl(gTg^{-1}F\wedge F\bigr).
$$

Since $gTg^{-1}$ is still in the [Lie algebra](../../../../../lie-algebra-split.md), the right-hand side vanishes whenever the original field satisfies every equation. **Every gauge transform of a bulk solution remains a bulk solution.** This conclusion follows from covariance of the field equations; it does not require the action itself to be exactly invariant under all large gauge transformations or under transformations changing prescribed boundary data.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
