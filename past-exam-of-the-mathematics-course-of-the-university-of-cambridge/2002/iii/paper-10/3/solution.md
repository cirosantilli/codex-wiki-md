<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

We take $\mathbb N=\{1,2,\ldots\}$. An [ultrafilter](../../../../../ultrafilter.md) $p$ on $\mathbb N$ is a proper [filter on a set](../../../../../filter-set-theory.md) which decides every subset: it contains $\mathbb N$ but not $\varnothing$, is closed under finite [intersections](../../../../../set-intersection.md) and passage to supersets, and contains exactly one of $A$ and $\mathbb N\setminus A$ for every $A\subseteq\mathbb N$. A [principal ultrafilter](../../../../../principal-ultrafilter.md) has the form $\delta_n=\{A:n\in A\}$; all other [ultrafilters](../../../../../ultrafilter.md) are [nonprincipal ultrafilters](../../../../../nonprincipal-ultrafilter.md).

To prove existence, start with the [cofinite filter](../../../../../cofinite-filter.md) and order its proper filter extensions by inclusion. The union of a chain is again a proper [filter on a set](../../../../../filter-set-theory.md): the finitely many sets involved in an intersection all belong to one member of the chain, and no member contains the empty set. Thus [Zorn's lemma](../../../../../zorn-s-lemma.md) supplies a maximal proper filter $p$. If $A\notin p$, adjoining $A$ must make the generated filter improper; equivalently, some $B\in p$ has $A\cap B=\varnothing$. Then $B\subseteq\mathbb N\setminus A$, so $\mathbb N\setminus A\in p$. This proves that $p$ is an [ultrafilter](../../../../../ultrafilter.md). It contains the complement of every finite set and hence no finite set. In particular, it contains no singleton and is **nonprincipal**.

The [Stone-Čech compactification of the natural numbers](../../../../../stone-cech-compactification-of-the-natural-numbers.md) $\beta\mathbb N$ is the set of all [ultrafilters](../../../../../ultrafilter.md) with basic [open sets](../../../../../open-set.md)

$$
\widehat A=\{p:A\in p\},\qquad A\subseteq\mathbb N.
$$

We have $\widehat A\cap\widehat B=\widehat{A\cap B}$ and $\beta\mathbb N\setminus\widehat A=\widehat{\mathbb N\setminus A}$, so these basic sets define a [topology](../../../../../topology-split.md) and are [clopen sets](../../../../../clopen-set.md). If $p\ne q$, choose $A\in p\setminus q$. The disjoint basic [neighbourhoods](../../../../../neighbourhood-mathematics.md) $\widehat A$ and $\widehat{\mathbb N\setminus A}$ separate them. Thus the space is [Hausdorff](../../../../../hausdorff-space.md).

For [compactness](../../../../../compact-space.md), it suffices to show every basic open cover has a finite subcover, since an arbitrary open cover can be refined by basic [open sets](../../../../../open-set.md). Suppose $\{\widehat{A_i}:i\in I\}$ has no finite subcover. The complements $\mathbb N\setminus A_i$ have the [finite intersection property](../../../../../finite-intersection-property.md): if a finite intersection were empty, the corresponding finite family of $\widehat{A_i}$ would cover every [ultrafilter](../../../../../ultrafilter.md). Their generated proper [filter on a set](../../../../../filter-set-theory.md) extends to an [ultrafilter](../../../../../ultrafilter.md), by the same [Zorn's lemma](../../../../../zorn-s-lemma.md) argument. This [ultrafilter](../../../../../ultrafilter.md) contains every $\mathbb N\setminus A_i$, and therefore belongs to none of the alleged cover members, a contradiction. We have proved that $\beta\mathbb N$ is a **compact Hausdorff space**. The map $n\mapsto\delta_n$ embeds the discrete natural numbers densely: any nonempty $\widehat A$ contains $\delta_n$ for some $n\in A$.

For [addition on the Stone-Čech compactification of the natural numbers](../../../../../addition-on-the-stone-cech-compactification-of-the-natural-numbers.md), define

$$
A-n=\{m\in\mathbb N:n+m\in A\},\qquad D_q(A)=\{n:A-n\in q\},
$$

and put

$$
A\in p+q\quad\Longleftrightarrow\quad D_q(A)\in p.
$$

The map $D_q$ preserves intersections and complements, because translation does and $q$ is an [ultrafilter](../../../../../ultrafilter.md). It also sends $\mathbb N$ to $\mathbb N$ and the empty set to itself. Consequently the displayed rule defines an [ultrafilter](../../../../../ultrafilter.md) $p+q$. On principal points it satisfies $\delta_n+\delta_m=\delta_{n+m}$, so it extends ordinary addition.

Write $(\forall^p n)\,\varphi(n)$ to mean that $\{n:\varphi(n)\}\in p$. The [ultrafilter](../../../../../ultrafilter.md) addition rule is then an iterated quantifier, with its order fixed. Expansion gives

$$
\begin{aligned}
A\in(p+q)+r
&\Longleftrightarrow (\forall^p n)(\forall^q m)(\forall^r \ell)\,[n+m+\ell\in A],\\
A\in p+(q+r)
&\Longleftrightarrow (\forall^p n)(\forall^q m)(\forall^r \ell)\,[n+(m+\ell)\in A].
\end{aligned}
$$

Ordinary addition is an [associative operation](../../../../../associative-operation.md), and the quantifiers are in the same order on both lines. Thus $\boxed{(p+q)+r=p+(q+r)}$. This argument does not interchange [ultrafilter](../../../../../ultrafilter.md) quantifiers and does not assert that this extended addition is commutative.

For fixed $q$, the translation $R_q:p\mapsto p+q$ has

$$
R_q^{-1}(\widehat A)=\widehat{D_q(A)},
$$

a basic [clopen set](../../../../../clopen-set.md). Therefore addition is **continuous in its left variable**. This is the left-continuity convention used here: right translations are continuous, giving a [left-topological semigroup](../../../../../left-topological-semigroup.md). Continuity in both variables jointly is not part of the assertion.

**Hindman's theorem** says that every [finite colouring](../../../../../finite-coloring.md) of the [positive integers](../../../../../positive-integer.md) has an increasing sequence $x_1<x_2<\cdots$ whose [finite-sums set](../../../../../finite-sums-set.md)

$$
\operatorname{FS}(x_1,x_2,\ldots)=\left\{\sum_{i\in F}x_i:\varnothing\ne F\subseteq\mathbb N\text{ finite}\right\}
$$

is [monochromatic](../../../../../monochromatic-set.md). Assume, as permitted, that the addition just defined has an [idempotent ultrafilter](../../../../../idempotent-ultrafilter.md) $p$, so $p+p=p$. This [ultrafilter](../../../../../ultrafilter.md) is nonprincipal: a principal $\delta_n$ would satisfy $\delta_n+\delta_n=\delta_{2n}\ne\delta_n$ for positive $n$. Hence every member of $p$ is infinite and every [cofinite set](../../../../../cofinite-set.md) belongs to $p$.

Exactly one cell $A$ of the finite colour partition belongs to $p$. Define its star set by

$$
A^*=A\cap D_p(A)=\{n\in A:A-n\in p\}.
$$

Since $A\in p+p$, we have $D_p(A)\in p$ and therefore $A^*\in p$. Moreover, for each $n\in A^*$, the set $A-n$ belongs to $p$. Idempotence gives $D_p(A-n)\in p$, and translation of the defining formula shows

$$
D_p(A-n)=D_p(A)-n,\qquad
A^*-n=(A-n)\cap D_p(A-n)\in p.
$$

This proves the [idempotent-ultrafilter star-set lemma](../../../../../idempotent-ultrafilter-star-set-lemma.md) rather than merely invoking it.

Choose $x_1\in A^*$. Suppose $x_1<\cdots<x_k$ have been chosen with every nonempty finite sum in $A^*$. Choose $x_{k+1}$ from

$$
A^*\cap\bigcap_{s\in\operatorname{FS}(x_1,\ldots,x_k)}(A^*-s)\cap\{n:n>x_k\}.
$$

This is a finite intersection of members of the [ultrafilter](../../../../../ultrafilter.md) $p$, and so it is nonempty. The new sums are $x_{k+1}$ and $s+x_{k+1}$; all lie in $A^*$ by the choice. [Mathematical induction](../../../../../mathematical-induction.md) yields an increasing infinite sequence with

$$
\boxed{\operatorname{FS}(x_1,x_2,\ldots)\subseteq A^*\subseteq A.}
$$

Thus the assumed idempotent gives the full [Hindman theorem](../../../../../hindman-theorem.md), with distinct increasing generators and all their nonempty finite sums of one colour.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
