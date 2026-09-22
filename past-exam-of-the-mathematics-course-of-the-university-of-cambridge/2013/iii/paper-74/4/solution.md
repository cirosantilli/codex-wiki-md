<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The two introductory requests can be settled before the lettered applications. In the [functor category](../../../../../functor-category.md) $[C,\mathbf{Set}]$, [finite limits](../../../../../finite-limit.md) and finite unions of [subobjects](../../../../../subobject.md) are pointwise. The component of the diagonal at $c$ is ordinary equality on $F(c)$. Its only possible complement is

$$
D(c)=\{(a,b)\in F(c)^2\mid a\ne b\}.
$$

This forms a subfunctor exactly when each $F(u)$ sends unequal elements to unequal elements, equivalently when every $F(u)$ is injective. In that case $D$ and the diagonal are disjoint and their union is $F^2$ at every component. Conversely, a diagonal complement must have these components and be stable under every transition map. Hence **$F$ is decidable exactly when every transition map is injective**.

Regard a [monoid](../../../../../monoid.md) $M$ as a one-object category; a covariant set-valued [functor](../../../../../functor.md) is a left [M-set](../../../../../m-set.md). Give $M\times A$ the diagonal left action $t\cdot(w,a)=(tw,t\cdot a)$. Let

$$
E=\operatorname{Hom}_M(M\times A,B),\qquad
(m\cdot f)(w,a)=f(wm,a).
$$

Right multiplication on the first coordinate commutes with the diagonal left action, so $m\cdot f$ remains equivariant. The formula obeys $m\cdot(n\cdot f)=(mn)\cdot f$ and $1\cdot f=f$. Evaluation is

$$
\operatorname{ev}:E\times A\to B,\qquad \operatorname{ev}(f,a)=f(1,a).
$$

It is equivariant because $\operatorname{ev}(m\cdot f,m\cdot a)=f(m,m\cdot a)=m\cdot f(1,a)$.

For an equivariant $h:C\times A\to B$, define

$$
\widehat h(c)(w,a)=h(w\cdot c,a).
$$

This is equivariant in $(w,a)$, and $\widehat h(m\cdot c)=m\cdot\widehat h(c)$. Evaluation recovers $h$. Conversely, currying the evaluation of a map $C\to E$ recovers that map by its equivariance. This proves the exponential universal property and the natural identification

$$
\boxed{B^A\cong\operatorname{Hom}_M(M\times A,B)}
$$

with exactly the stated action. In particular, [decidability in a set-valued functor category](../../../../../decidability-in-a-set-valued-functor-category.md) says that a left [M-set](../../../../../m-set.md) is decidable if and only if each of its action maps is injective.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
