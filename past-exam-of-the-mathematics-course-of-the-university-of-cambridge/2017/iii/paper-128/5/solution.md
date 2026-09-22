<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Put $A^e=A\otimes_k A^{\mathrm{op}}$, so an $A$-[bimodule](../../../../../bimodule.md) is a left $A^e$-[module](../../../../../module-mathematics.md) through $(a\otimes b^{\mathrm{op}})m=amb$. The [Hochschild cohomology](../../../../../hochschild-cohomology.md) is

$$
\boxed{HH^n(A,M)=\operatorname{Ext}_{A^e}^n(A,M).}
$$

Equivalently, the [Hochschild cochain complex](../../../../../hochschild-cochain-complex.md) has $C^n(A,M)=\operatorname{Hom}_k(A^{\otimes n},M)$ and [coboundary map](../../../../../coboundary-map.md)

$$
(\delta f)(a_1,\ldots,a_{n+1})=a_1f(a_2,\ldots,a_{n+1})+\sum_{i=1}^n(-1)^if(a_1,\ldots,a_ia_{i+1},\ldots,a_{n+1})+(-1)^{n+1}f(a_1,\ldots,a_n)a_{n+1}.
$$

Its [cohomology](../../../../../cohomology-split.md) agrees with the displayed [Ext functor](../../../../../ext-functor.md) because the [bar resolution of an associative algebra](../../../../../bar-resolution-of-an-associative-algebra.md) is free over $A^e$ when $k$ is a [field](../../../../../field.md). The [Hochschild cohomological dimension](../../../../../hochschild-cohomological-dimension.md) is

$$
\boxed{\operatorname{Dim}(A)=\operatorname{pd}_{A^e}A=\sup\{n:HH^n(A,N)\ne0\text{ for some bimodule }N\}.}
$$

The supremum uses all [bimodules](../../../../../bimodule.md), not merely the finitely generated one supplied in the question; an unbounded [projective dimension](../../../../../projective-dimension.md) is infinity.

An extension in this classification is a [square-zero extension of an algebra](../../../../../square-zero-extension-of-an-algebra.md): a short [exact sequence](../../../../../exact-sequence.md) $0\to M\to E\to A\to0$, where $E$ and $A$ are unital [algebras](../../../../../algebra-split.md), $E\to A$ is unital, and $M$ is its two-sided [ideal](../../../../../ideal.md) with $M^2=0$ and induced $A$-[bimodule](../../../../../bimodule.md) structure equal to the prescribed one. An equivalence of extensions is an [algebra isomorphism](../../../../../algebra-isomorphism.md) of the middle terms commuting with the maps and inducing the identity on both $A$ and $M$. Arbitrary isomorphisms of middle [algebras](../../../../../algebra-split.md), or extensions without the [square-zero ideal](../../../../../square-zero-ideal.md) requirement, are not classified by this [cohomology](../../../../../cohomology-split.md) group.

Choose a $k$-[linear map](../../../../../linear-map.md) section $s:A\to E$ with $s(1)=1$. Its multiplication defect

$$
\mu(a,b)=s(a)s(b)-s(ab)\in M
$$

is a normalized [Hochschild cocycle](../../../../../hochschild-cocycle.md): $\mu(1,a)=\mu(a,1)=0$, and [associativity](../../../../../associative-property.md) in $E$ gives $\delta\mu=0$. Changing $s$ to $s+g$, where $g(1)=0$, changes the defect to $\mu+\delta g$, since $M^2=0$.

Conversely, for a normalized [Hochschild cocycle](../../../../../hochschild-cocycle.md) $\mu$, put $E_\mu=A\oplus M$ as a [vector space](../../../../../vector-space-split.md) and define

$$
(a,m)(b,n)=(ab,an+mb+\mu(a,b)).
$$

The [Hochschild cocycle](../../../../../hochschild-cocycle.md) equation is exactly [associativity](../../../../../associative-property.md), and $(1,0)$ is the identity. If $\mu'=\mu+\delta g$, the map $E_{\mu'}\to E_\mu$, $(a,m)\mapsto(a,m+g(a))$, is an equivalence. Conversely, every equivalence has this form after choosing sections. The [normalized Hochschild cochain complex](../../../../../normalized-hochschild-cochain-complex.md) computes the same [cohomology](../../../../../cohomology-split.md) as the full complex: in the [bar resolution of an associative algebra](../../../../../bar-resolution-of-an-associative-algebra.md), the degenerate terms containing an inserted identity form a contractible subcomplex. Passing to the normalized [bar resolution of an associative algebra](../../../../../bar-resolution-of-an-associative-algebra.md), then applying the [Hom functor](../../../../../hom-functor.md), gives the same [cohomology](../../../../../cohomology-split.md). Thus every class has a normalized representative. We obtain **a bijection between $HH^2(A,M)$ and equivalence classes of square-zero extensions**.

For a [formal associative deformation](../../../../../formal-associative-deformation.md), a completion convention is necessary. The usual [star product](../../../../../formal-associative-deformation.md) lives on the [formal power series module](../../../../../formal-power-series-module.md)

$$
A[[t]]=\varprojlim_r A\otimes_k k[t]/(t^r).
$$

This is the [adic completion of a module](../../../../../adic-completion-of-a-module.md) applied to the ordinary [tensor product](../../../../../tensor-product.md), rather than literally the ordinary $A\otimes_k k[[t]]$ when $A$ is infinite-dimensional. For example, $\sum_{n\geq0}X^nt^n$ lies in $k[X][[t]]$ but not in the ordinary [tensor product](../../../../../tensor-product.md), whose coefficient spaces have finite-dimensional span. The two agree when $A$ is finite-dimensional. We interpret the printed notation in this standard completed sense; the infinite iteration below requires that interpretation.

A [star product](../../../../../formal-associative-deformation.md) is a $k[[t]]$-bilinear, unital product continuous for the [adic topology](../../../../../adic-topology.md) satisfying [associativity](../../../../../associative-property.md) of the form

$$
a*b=ab+\sum_{r\geq1}t^r\mu_r(a,b),\qquad \mu_r\in\operatorname{Hom}_k(A\otimes A,A),\quad \mu_r(1,a)=\mu_r(a,1)=0.
$$

It is a [trivial formal deformation](../../../../../trivial-formal-deformation.md) if a $k[[t]]$-linear [automorphism](../../../../../automorphism.md) continuous for the [adic topology](../../../../../adic-topology.md) $T=\operatorname{id}+\sum_{r\geq1}t^rT_r$, with $T(1)=1$, satisfies $T(a*b)=T(a)T(b)$.

If $\operatorname{Dim}(A)\leq1$, then $HH^2(A,A)=0$. Suppose changes of coordinates have removed all coefficients below order $r$. The order-$r$ part of [associativity](../../../../../associative-property.md) then says $\delta\mu_r=0$. Hence $\mu_r=\delta g_r$ for a $k$-linear map $g_r:A\to A$. Its normalization gives $g_r(1)=0$, since $(\delta g_r)(1,1)=g_r(1)$. Transport the product by $T_r=\operatorname{id}+t^rg_r$:

$$
a*'b=T_r\bigl(T_r^{-1}(a)*T_r^{-1}(b)\bigr).
$$

The order-$r$ coefficient becomes $\mu_r-\delta g_r=0$, and lower coefficients remain zero. Repeating constructs compatible changes of coordinates modulo every $t^N$. They converge in the [adic topology](../../../../../adic-topology.md) to an invertible $T$ fixing $1$, with inverse obtained coefficient by coefficient. The limit product is ordinary multiplication. Therefore **every star product is trivial under the completed formal-series convention**. In fact, the argument only needs the vanishing of $HH^2(A,A)$, not all of [Hochschild cohomological dimension](../../../../../hochschild-cohomological-dimension.md) at most one.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 128](../../paper-128-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
