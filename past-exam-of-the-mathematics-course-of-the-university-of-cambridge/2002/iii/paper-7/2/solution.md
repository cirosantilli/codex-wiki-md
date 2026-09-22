<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Give $\mathcal O(U)$ the [compact-open topology](../../../../../compact-open-topology.md). Choose a finite polygonal cycle $\Gamma$ in $U\setminus\sigma_A(x)$ whose [winding number](../../../../../winding-number.md) is one on the [Banach algebra spectrum](../../../../../spectrum-of-an-element.md) and zero outside $U$. One can take the oriented [boundary](../../../../../boundary-of-a-set.md) of a finite union of small squares surrounding the [compact](../../../../../compact-space.md) [Banach algebra spectrum](../../../../../spectrum-of-an-element.md) and contained in $U$. Define

$$
\Theta_x(f)=\frac1{2\pi i}\int_\Gamma f(z)(z1-x)^{-1}\,dz.
$$

The integral is an algebra-norm integral of a [continuous](../../../../../continuous-function.md) function on finitely many segments. Cauchy's theorem, applied after any [bounded linear functional](../../../../../continuous-linear-functional.md) on $A$, makes it independent of the cycle. Moreover

$$
\|\Theta_x(f)\|\le C_\Gamma\sup_{z\in\Gamma}|f(z)|,\qquad
C_\Gamma=\frac{\operatorname{length}(\Gamma)}{2\pi}\max_\Gamma\|(z1-x)^{-1}\|,
$$

so it is [continuous](../../../../../continuous-function.md) for the [compact-open topology](../../../../../compact-open-topology.md).

Here is a direct verification of the algebra properties and uniqueness using the allowed [Runge theorem](../../../../../runge-s-theorem.md). The version required is that every [holomorphic function](../../../../../holomorphic-function.md) on an [open](../../../../../open-set.md) plane [set](../../../../../set-split.md) is a locally uniform limit of [rational functions](../../../../../rational-function.md) with poles outside that [set](../../../../../set-split.md), allowing a [polynomial](../../../../../polynomial-split.md) part. A [rational function](../../../../../rational-function.md) $r=p/q$ of this kind has the unambiguous value $r(x)=p(x)q(x)^{-1}$, since the roots of $q$ avoid the [Banach algebra spectrum](../../../../../spectrum-of-an-element.md). These rational values form a [unital algebra](../../../../../unital-algebra.md) [homomorphism](../../../../../homomorphism.md).

They agree with the [contour integral](../../../../../contour-integral.md). First $\frac1{2\pi i}\int_\Gamma(z1-x)^{-1}\,dz=1$, by replacing the cycle with a large circle and integrating its Neumann expansion. The identity $z^j1-x^j=(z1-x)\sum_{k=0}^{j-1}z^{j-1-k}x^k$ then proves the assertion for [polynomials](../../../../../polynomial-split.md). For $a\notin U$, the [resolvent identity](../../../../../resolvent-identity.md) gives

$$
\frac{(z1-x)^{-1}}{z-a}
=(x-a1)^{-1}\left((z1-x)^{-1}-\frac1{z-a}1\right).
$$

The cycle has [winding number](../../../../../winding-number.md) zero at $a$, so integration gives $(x-a1)^{-1}$. This identity holds on a neighborhood of $a$ disjoint from the cycle and the [Banach algebra spectrum](../../../../../spectrum-of-an-element.md). Differentiating with respect to $a$ gives the analogous result for every power $(z-a)^{-k}$, and partial fractions give it for all the [rational functions](../../../../../rational-function.md) under consideration.

If $r_n\to f$ and $s_n\to g$ locally uniformly, the contour estimate makes their evaluated sequences converge. Since $r_ns_n\to fg$ locally uniformly and multiplication in $A$ is [continuous](../../../../../continuous-function.md), their limits satisfy $\Theta_x(fg)=\Theta_x(f)\Theta_x(g)$. Also $\Theta_x(1)=1$ and $\Theta_x(Z)=x$. Conversely any [continuous](../../../../../continuous-function.md) [unital](../../../../../unital-algebra.md) complex-algebra [homomorphism](../../../../../homomorphism.md) sending $Z$ to $x$ must send $Z-a$ to $x-a1$ and its reciprocal to the inverse. It therefore agrees on [rational functions](../../../../../rational-function.md) and then, by Runge density and [continuity](../../../../../continuous-function.md), on all of $\mathcal O(U)$. This proves **existence and uniqueness of the [holomorphic functional calculus](../../../../../holomorphic-functional-calculus.md)**.

For its spectral mapping property, first note compatibility on a smaller [open](../../../../../open-set.md) spectral neighborhood $W\subseteq U$: composing restriction to $W$ with the calculus there gives the calculus on $U$ by uniqueness. If $\mu\notin g(\sigma_A(x))$, choose such a $W$ where $\mu-g$ never vanishes. Then

$$
(\mu1-\Theta_x(g))^{-1}=\Theta_x\bigl((\mu-g)^{-1}\bigr),
$$

with the right side evaluated on $W$. Conversely, for $\lambda\in\sigma_A(x)$, write $g(z)-g(\lambda)=(z-\lambda)q(z)$ with $q$ [holomorphic](../../../../../complex-differentiability-at-a-point.md) on $U$. The evaluated factors commute. If their product were invertible, both factors would be invertible, contradicting $\lambda\in\sigma_A(x)$. Thus

$$
\boxed{\sigma_A(\Theta_x(g))=g(\sigma_A(x))\subseteq g(U)\subseteq V.}
$$

Pullback $h\mapsto h\circ g$ is [continuous](../../../../../continuous-function.md) from $\mathcal O(V)$ to $\mathcal O(U)$ because the image under $g$ of a [compact](../../../../../compact-space.md) [set](../../../../../set-split.md) is [compact](../../../../../compact-space.md). The composite $h\mapsto\Theta_x(h\circ g)$ is a [continuous](../../../../../continuous-function.md) [unital](../../../../../unital-algebra.md) [homomorphism](../../../../../homomorphism.md) taking the coordinate function to $y=\Theta_x(g)$. Uniqueness of the calculus at $y$ proves

$$
\boxed{\Theta_y(h)=\Theta_x(h\circ g).}
$$

For the exponential conclusion, let $K=\sigma_A(x)$. There is a simple polygonal arc from zero through its unbounded complementary component to outside a disk containing $K$, continued by a ray to infinity and avoiding $K$. Loops in an initial polygonal path can be removed to make the arc simple. The complement of this slit is a [simply connected](../../../../../simply-connected-space.md) [open](../../../../../open-set.md) neighborhood of $K$ avoiding zero, and hence admits a [holomorphic logarithm](../../../../../holomorphic-logarithm.md) $\ell$. [Set](../../../../../set-split.md) $y=\Theta_x(\ell)$. The composition rule gives

$$
\boxed{e^y=\Theta_x(e^\ell)=\Theta_x(Z)=x.}
$$

The calculus of the entire exponential agrees with the usual algebra exponential because its power-series partial sums converge locally uniformly. Finally an invertible [matrix](../../../../../matrix.md) over the [complex numbers](../../../../../complex-number.md) has a finite [Banach algebra spectrum](../../../../../spectrum-of-an-element.md) avoiding zero. Removing finitely many plane points leaves a [connected](../../../../../connected-space.md) [set](../../../../../set-split.md), so the hypothesis always holds: **every invertible [matrix](../../../../../matrix.md) over the [complex numbers](../../../../../complex-number.md) is an exponential of a [matrix](../../../../../matrix.md) over the [complex numbers](../../../../../complex-number.md)**.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
