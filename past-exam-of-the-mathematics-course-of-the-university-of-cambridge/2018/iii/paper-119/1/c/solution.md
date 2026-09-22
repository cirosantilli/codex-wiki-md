<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume (c), and take an [epimorphism](../../../../../../epimorphism.md) $p:M\twoheadrightarrow h_A$ with $M$ a [monofunctor](../../../../../../monofunctor.md). Since $h_A$ is a [projective object in a category](../../../../../../projective-object.md), there is a [natural transformation](../../../../../../natural-transformation.md) $s:h_A\to M$ with $ps=1_{h_A}$. A [retract in a category](../../../../../../retract-in-a-category.md) of a [monofunctor](../../../../../../monofunctor.md) is a [monofunctor](../../../../../../monofunctor.md): if $h_A(f)(u)=h_A(f)(v)$, then naturality of $s$ gives $M(f)s(u)=M(f)s(v)$, injectivity of $M(f)$ gives $s(u)=s(v)$, and applying $p$ gives $u=v$. Thus (c) implies (b), completing

$$
\boxed{\text{(a)}\Longleftrightarrow\text{(b)}\Longleftrightarrow\text{(c)}.}
$$

The stronger assertion that every set-valued [functor](../../../../../../functor.md) is a [monofunctor](../../../../../../monofunctor.md) holds exactly when $\mathcal C$ is a [groupoid](../../../../../../groupoid.md). Sufficiency follows because a [functor](../../../../../../functor.md) preserves inverses, so sends every arrow to a bijection.

For necessity, fix $f:A\to B$, and form the pointwise [pushout in a category](../../../../../../pushout-in-a-category.md)

$$
P=h_A\amalg_{h_B}h_A,
$$

using twice the [natural transformation](../../../../../../natural-transformation.md) $h_B\to h_A$ given by precomposition with $f$. At an object $X$, $P(X)$ consists of two copies of $\mathcal C(A,X)$, with the two copies of $kf$ identified for every $k:B\to X$. No different underlying elements are identified: each generating relation simply joins the two copies of one element. In $P(B)$, the two copies of $f$ coincide, since $f=1_Bf$. Hence $P(f)$ sends the two copies of $1_A$ in $P(A)$ to the same element. If $P$ is a [monofunctor](../../../../../../monofunctor.md), those copies of $1_A$ coincide. The description of the pushout implies $rf=1_A$ for some $r:B\to A$. Thus every morphism is a [split monomorphism](../../../../../../split-monomorphism.md).

Apply the same conclusion to $r$: there is $t:A\to B$ with $tr=1_B$. Then $t=trf=f$, and so $fr=1_B$ as well. Every arrow is invertible, proving

$$
\boxed{\text{Every }F:\mathcal C\to\mathbf{Set}\text{ is a monofunctor}\ \Longleftrightarrow\ \mathcal C\text{ is a groupoid}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 119](../../../paper-119-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
