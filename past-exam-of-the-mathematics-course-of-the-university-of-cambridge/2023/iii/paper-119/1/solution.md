<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a [locally small category](../../../../../locally-small-category.md) $\mathcal C$, a [representation of a functor](../../../../../representation-of-a-functor.md) $F:\mathcal C\to\mathbf{Set}$ is an object $A$ and an element $a\in F(A)$ such that

$$
\theta_B:\mathcal C(A,B)\longrightarrow F(B),
\qquad
f\longmapsto F(f)(a)
$$

is a bijection for every $B$, naturally in $B$. Equivalently, $\theta:\mathcal C(A,-)\cong F$ is a [natural isomorphism](../../../../../natural-transformation.md).

Suppose $(A,a)$ and $(A',a')$ are two representations. Universality gives unique maps

$$
u:A\to A',\qquad v:A'\to A
$$

such that $F(u)(a)=a'$ and $F(v)(a')=a$. Then $F(vu)(a)=a$, and uniqueness applied to the element $a$ gives $vu=1_A$. Similarly $uv=1_{A'}$. Thus the representing objects are uniquely isomorphic in a way carrying one [universal element of a set-valued functor](../../../../../universal-element-of-a-set-valued-functor.md) to the other.

For $F:\mathcal C\to\mathcal D$ and $B\in\mathcal D$, the [comma category](../../../../../comma-category.md) $(B\downarrow F)$ has objects $(A,u)$ with $u:B\to F(A)$. A morphism $(A,u)\to(A',u')$ is a map $h:A\to A'$ satisfying

$$
F(h)u=u'.
$$

The [universal arrow from an object to a functor](../../../../../universal-arrow-from-an-object-to-a-functor.md) criterion says that $F$ has a left adjoint exactly when $(B\downarrow F)$ has an [initial object](../../../../../initial-object.md) for every $B$. Indeed, an initial $(L B,\eta_B)$ represents the functor $A\mapsto\mathcal D(B,F A)$, and uniqueness makes $B\mapsto L B$ functorial.

When $F:\mathcal C\to\mathbf{Set}$ and $1$ is a singleton, an arrow $1\to F(A)$ is just an element $a\in F(A)$. Hence $(1\downarrow F)$ is the category of elements, and its initial objects are exactly the representations of $F$. This proves

$$
F\text{ representable}
\quad\Longleftrightarrow\quad
(1\downarrow F)\text{ has an initial object}.
$$

If $F$ has a left adjoint, the universal-arrow criterion immediately makes it representable. Conversely, suppose $\mathcal C$ is [cocomplete](../../../../../cocomplete-category.md) and $F\cong\mathcal C(A,-)$. For a set $S$, form the copower

$$
L(S)=\coprod_{s\in S}A.
$$

The [coproduct in a category](../../../../../coproduct.md) universal property gives natural bijections

$$
\mathcal C(L(S),B)
\cong\prod_{s\in S}\mathcal C(A,B)
\cong\mathbf{Set}(S,F(B)),
$$

so $L\dashv F$.

Cocompleteness cannot be omitted. Let $\mathcal C$ be the [category of ordinals in reverse order](../../../../../category-of-ordinals-in-reverse-order.md): there is one arrow $\alpha\to\beta$ exactly when $\alpha\geq\beta$ in the ordinary ordering. This large poset is locally small and complete. For a set-indexed family $(\alpha_i)$, its product in the reversed order is the ordinary supremum $\sup_i\alpha_i$, and equalizers in a poset are automatic. But $\mathcal C$ has no initial object, since that would be a largest ordinal. Any representable functor $\mathcal C(A,-)$ is therefore the requested example: if it had a left adjoint $L$, then

$$
\mathcal C(L(\varnothing),B)
\cong\mathbf{Set}(\varnothing,\mathcal C(A,B))
$$

would be a singleton for every $B$, making $L(\varnothing)$ initial, a contradiction.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
