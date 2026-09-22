<h1 id="b/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A unital [C-star algebra](../../../../c-star-algebra.md) is a complex [Banach algebra](../../../../banach-algebra-split.md) $A$ with a multiplicative identity $1_A$ and a conjugate-linear [involution](../../../../involution.md) $a\mapsto a^*$ satisfying $(ab)^*=b^*a^*$ and the [C-star identity](../../../../c-star-identity.md) $\|a^*a\|=\|a\|^2$. A [C-star isomorphism](../../../../c-star-isomorphism.md) $\Phi:A\to B$ is a bijective complex-linear map preserving products and the [involution](../../../../involution.md). It carries $1_A$ to $1_B$ and is automatically isometric.

For a commutative unital [C-star algebra](../../../../c-star-algebra.md), let $\Omega$ be its [maximal ideal space](../../../../maximal-ideal-space-of-a-commutative-banach-algebra.md), equivalently the space of [Gelfand characters](../../../../character-of-an-algebra.md), with the [weak-star topology](../../../../weak-star-topology.md). A [Gelfand character](../../../../character-of-an-algebra.md) has $\chi(1)=1$ and $\|\chi\|=1$. The equations $\chi(ab)=\chi(a)\chi(b)$ and $\chi(1)=1$ define a closed in the [weak-star topology](../../../../weak-star-topology.md) subset of the dual unit ball. The [Banach-Alaoglu theorem](../../../../banach-alaoglu-theorem.md) makes $\Omega$ a [compact Hausdorff space](../../../../compact-hausdorff-space.md). Maximal ideals give characters by the [Gelfand-Mazur theorem](../../../../gelfand-mazur-theorem.md), and the [Banach algebra spectrum](../../../../spectrum-of-an-element.md) satisfies $\sigma(a)=\{\chi(a):\chi\in\Omega\}$.

The [Gelfand transform](../../../../gelfand-representation.md) is $\widehat a(\chi)=\chi(a)$. It preserves products, constants and the [involution](../../../../involution.md); the latter uses the fact that [characters of a C-star algebra respect the involution](../../../../characters-of-a-c-star-algebra-respect-the-involution.md). Every element of a commutative [C-star algebra](../../../../c-star-algebra.md) is normal, so the [C-star identity](../../../../c-star-identity.md) and the [spectral radius formula](../../../../spectral-radius-formula.md) give

$$
\|\widehat a\|_\infty=\sup_{\chi\in\Omega}|\chi(a)|=r(a)=\|a\|.
$$

Thus its [image](../../../../image-of-a-function.md) is a closed self-adjoint subalgebra of $C(\Omega)$, contains the constants, and separates characters. The complex [Stone-Weierstrass theorem](../../../../stone-weierstrass-theorem.md) makes that [image](../../../../image-of-a-function.md) dense and therefore all of $C(\Omega)$. This is the [Commutative Gelfand--Naimark theorem](../../../../commutative-gelfand-naimark-theorem.md).

For the [convergent sequence space](../../../../convergent-sequence-space.md) $c$, coordinatewise multiplication satisfies $\|\alpha\beta\|_\infty\leq\|\alpha\|_\infty\|\beta\|_\infty$, and coordinatewise complex conjugation is an [involution](../../../../involution.md). The constant sequence $1$ is the identity, and

$$
\|\alpha^*\alpha\|_\infty=\sup_n|\alpha_n|^2=\|\alpha\|_\infty^2.
$$

It is complete: a uniform limit of convergent sequences is convergent, so $c$ is a closed [linear subspace](../../../../vector-subspace.md) of the [Banach space](../../../../banach-space-split.md) $\ell_\infty$. Hence it is a commutative unital [C-star algebra](../../../../c-star-algebra.md).

Take

$$
\boxed{\Omega=\mathbb N\cup\{\infty\},\quad\text{the one-point compactification of discrete }\mathbb N.}
$$

Every finite point is isolated, and the neighbourhoods of $\infty$ contain all but finitely many integers. This is a [compact Hausdorff space](../../../../compact-hausdorff-space.md): an open cover has a set containing $\infty$, leaving only finitely many points to cover. Define

$$
\Phi(\alpha)(n)=\alpha_n,\qquad\Phi(\alpha)(\infty)=\lim_{n\to\infty}\alpha_n.
$$

Continuity at $\infty$ is exactly convergence of the sequence. Thus $\Phi$ is onto $C(\Omega)$, and pointwise operations show it is a [C-star isomorphism](../../../../c-star-isomorphism.md) with $\|\Phi\alpha\|_\infty=\|\alpha\|_\infty$. Explicitly, these are all [Gelfand characters](../../../../character-of-an-algebra.md): each $\chi(e_n)$ is $0$ or $1$ and at most one is $1$. If $\chi(e_n)=1$, multiplication by $e_n$ gives $\chi(\alpha)=\alpha_n$. If all vanish, [density of finitely supported sequences in l-p](../../../../density-of-finitely-supported-sequences-in-l-p.md) in $c_0$ gives $\chi|_{c_0}=0$, so $\chi(\alpha)=\lim\alpha_n$.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [B](../../b.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../split.md)
5. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
