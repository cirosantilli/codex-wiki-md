<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $K=\sigma_A(x)$ and equip $\mathcal O(U)$ with the [compact-open topology](../../../../../compact-open-topology.md). All [algebra homomorphisms](../../../../../algebra-homomorphism-over-a-field.md) here are complex linear. Choose a finite positively oriented [boundary](../../../../../boundary-of-a-set.md) cycle $\Gamma$ in $U\setminus K$ with [winding number](../../../../../winding-number.md) one on a neighborhood of $K$ and zero outside $U$. Such a cycle can be obtained as the [boundary](../../../../../boundary-of-a-set.md) of a finite union of sufficiently small squares whose [interior](../../../../../interior-topology.md) contains $K$ and whose closure is contained in $U$; holes are included with negative [boundary](../../../../../boundary-of-a-set.md) orientation. Define the [holomorphic functional calculus](../../../../../holomorphic-functional-calculus.md) by the norm-convergent [contour integral](../../../../../contour-integral.md)

$$
\Theta_x(f)=\frac1{2\pi i}\int_\Gamma f(z)R(z)\,dz,
\qquad R(z)=(z1-x)^{-1}.
$$

The [resolvent identity](../../../../../resolvent-identity.md) proves that $R$ is a [Banach-space-valued holomorphic function](../../../../../banach-space-valued-holomorphic-function.md) off $K$. The [Cauchy integral theorem](../../../../../cauchy-s-integral-theorem.md), applied after each [bounded linear functional](../../../../../continuous-linear-functional.md), makes the integral independent of the chosen [boundary](../../../../../boundary-of-a-set.md) cycle. The [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) then gives equality of the algebra-valued integrals. Moreover,

$$
\|\Theta_x(f)\|\le\frac{\operatorname{length}(\Gamma)}{2\pi}\sup_\Gamma\|R(z)\|\sup_\Gamma|f(z)|,
$$

which proves complex [linearity](../../../../../linearity.md) and [continuity](../../../../../continuous-function.md) for the [compact-open topology](../../../../../compact-open-topology.md).

For the constant function $1$ and the coordinate function $Z$, the contour can be deformed to a large circle because their integrands are [holomorphic](../../../../../complex-differentiability-at-a-point.md) everywhere outside $K$. There the [Neumann series](../../../../../neumann-series.md) gives $R(z)=\sum_{n\ge0}x^nz^{-n-1}$. Integrating term by term shows

$$
\Theta_x(1)=1,\qquad\Theta_x(Z)=x.
$$

To prove multiplicativity, take nested cycles $\Gamma_o,\Gamma_i$ around $K$, with the outer cycle winding once on the inner cycle and the inner winding zero on the outer cycle. Use the outer cycle for $f$ and the inner for $g$. The [resolvent identity](../../../../../resolvent-identity.md) reads

$$
R(z)R(w)=\frac{R(w)-R(z)}{z-w}.
$$

In the resulting double integral, the term containing $R(w)$ gives $f(w)g(w)R(w)$ after the $z$ integral, by the [Cauchy integral formula](../../../../../cauchy-integral-formula.md). The term containing $R(z)$ vanishes after the $w$ integral, because $w\mapsto g(w)/(z-w)$ is [holomorphic](../../../../../complex-differentiability-at-a-point.md) on and inside the inner cycle's region. Therefore

$$
\Theta_x(f)\Theta_x(g)=\Theta_x(fg).
$$

The integrals are over finite [compact](../../../../../compact-space.md) curves and have [continuous](../../../../../continuous-function.md) integrands, so exchanging their order is legitimate. This proves the existence of the required [continuous](../../../../../continuous-function.md) unital [algebra homomorphism](../../../../../algebra-homomorphism-over-a-field.md).

For uniqueness, the [Runge approximation theorem](../../../../../runge-s-theorem.md) gives density in $\mathcal O(U)$, for the [compact-open topology](../../../../../compact-open-topology.md), of [rational functions](../../../../../rational-function.md) with poles outside $U$. More explicitly, exhaust $U$ by [compact](../../../../../compact-space.md) sets that are holomorphically convex relative to $U$, and approximate on those sets by [rational functions](../../../../../rational-function.md) whose poles lie in the complement of $U$; this gives convergence on every [compact](../../../../../compact-space.md) subset. Any unital [algebra homomorphism](../../../../../algebra-homomorphism-over-a-field.md) taking $Z$ to $x$ must take $(Z-\alpha)^{-1}$, for $\alpha\notin U$, to $(x-\alpha1)^{-1}$, since it preserves inverse equations. Partial fractions and [polynomial](../../../../../polynomial-split.md) algebra therefore fix its value on every such [rational function](../../../../../rational-function.md). [Continuity](../../../../../continuous-function.md) fixes its value on their limits. Thus **the [continuous](../../../../../continuous-function.md) unital homomorphism with the prescribed coordinate value is unique**. Restricting a function to a smaller neighborhood of $K$ gives the same value, either by the contour definition or this uniqueness argument.

To prove the [holomorphic spectral mapping theorem](../../../../../holomorphic-spectral-mapping-theorem.md), first let $\mu\notin f(K)$. There is an open neighborhood $V\subseteq U$ of $K$ on which $f-\mu$ has no zeros. The [holomorphic function](../../../../../holomorphic-function.md) $h=1/(f-\mu)$ on $V$ supplies a two-sided inverse through

$$
\Theta_x(f)-\mu1=\Theta_x(f-\mu),\qquad
\Theta_x(f-\mu)\Theta_x(h)=\Theta_x(h)\Theta_x(f-\mu)=1.
$$

Thus $\sigma_A(\Theta_x(f))\subseteq f(K)$. Conversely, if $\lambda\in K$ and $\mu=f(\lambda)$, the divided difference

$$
g(z)=\frac{f(z)-f(\lambda)}{z-\lambda},\qquad g(\lambda)=f'(\lambda),
$$

is [holomorphic](../../../../../complex-differentiability-at-a-point.md) on $U$, and multiplicativity gives

$$
\Theta_x(f)-\mu1=(x-\lambda1)\Theta_x(g).
$$

The two factors commute. A commuting product $uv$ can be invertible only if both factors are invertible: its inverse commutes with each factor, and $v(uv)^{-1}$ is a two-sided inverse for $u$. Invertibility of the displayed product would therefore contradict $\lambda\in K$. This proves

$$
\boxed{\sigma_A(\Theta_x(f))=f(\sigma_A(x)).}
$$

For the root, let $D=\mathbb C\setminus(-\infty,0]$ and $q(z)=\exp(\operatorname{Log}z/3)$, using the [principal complex logarithm](../../../../../principal-complex-logarithm.md). Define $y=\Theta_x(q)$. Since $q(z)^3=z$, multiplicativity and the [holomorphic spectral mapping theorem](../../../../../holomorphic-spectral-mapping-theorem.md) give

$$
\boxed{y^3=x,\qquad\sigma_A(y)=q(K)\subseteq S,\qquad S=\{z\ne0:|\arg z|<\pi/3\}.}
$$

This is the [principal cube root of a Banach-algebra element](../../../../../principal-cube-root-of-a-banach-algebra-element.md).

For uniqueness, suppose $v^3=x$ and $\sigma_A(v)\subset S$. Cubing maps the whole open sector $S$ into $D$, so

$$
F:\mathcal O(D)\longrightarrow A,\qquad F(h)=\Theta_v\bigl(z\mapsto h(z^3)\bigr)
$$

is a [continuous](../../../../../continuous-function.md) unital [algebra homomorphism](../../../../../algebra-homomorphism-over-a-field.md): pullback by cubing is [continuous](../../../../../continuous-function.md) for the [compact-open topology](../../../../../compact-open-topology.md), since images of [compact](../../../../../compact-space.md) sets are [compact](../../../../../compact-space.md). It takes the coordinate function to $v^3=x$, and uniqueness already proved gives $F=\Theta_x$. For $z\in S$, the scalar [principal cube root](../../../../../principal-cube-root.md) satisfies $q(z^3)=z$, because $3\arg z\in(-\pi,\pi)$. Hence

$$
v=\Theta_v(q\circ(z\mapsto z^3))=F(q)=\Theta_x(q)=y.
$$

This proves **uniqueness with the stated spectral sector**, without assuming the ambient [Banach algebra](../../../../../banach-algebra-split.md) is [commutative](../../../../../commutativity.md) or that [algebra characters](../../../../../character-of-an-algebra.md) separate its elements.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
