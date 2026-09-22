<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $(W_e)_{e\in\mathbb N}$ enumerate all [computably enumerable sets](../../../../../recursively-enumerable-set.md), with finite uniformly computable approximations $W_{e,s}$ increasing to $W_e$. For example, take $W_e=\operatorname{dom}\varphi_e$ and

$$
W_{e,s}=\{x<s:\varphi_e(x)\text{ halts within }s\text{ steps}\}.
$$

We construct a [simple set](../../../../../simple-set.md) by meeting the requirements $R_e$: if $W_e$ is infinite, then $W_e\cap X\ne\varnothing$. Begin with no enumerated elements and all requirements unmarked. At stage $s$, process $e=0,1,\ldots,s$ in this order. For an unmarked $R_e$, if there is an $x\in W_{e,s}$ with $x>2e$, enumerate the least such $x$ into $X$ and mark $R_e$ permanently. All membership tests at a stage are finite, and marking requires no test for eventual infinitude. The [sparse-witness construction of a simple set](../../../../../sparse-witness-construction-of-a-simple-set.md) therefore gives a [computably enumerable set](../../../../../recursively-enumerable-set.md) $X$; it is [semidecidable](../../../../../recursively-enumerable-set.md) by simulating this enumeration and halting when the input appears.

Each requirement enumerates at most one element. If an element in $[0,2n]$ is enumerated by $R_e$, then $2e<x\leq2n$, so $e<n$. At most $n$ elements of that interval can therefore enter $X$, even if some requirements choose the same element. Consequently

$$
\boxed{|[0,2n]\setminus X|\geq(2n+1)-n=n+1.}
$$

The [complement of a set](../../../../../complement-of-a-set.md) $\mathbb N\setminus X$ is infinite.

If $W_e$ is infinite, it contains some $x>2e$, and that element eventually belongs to $W_{e,s}$ at a stage with $s\geq e$. If $R_e$ has already acted, it already placed an element of $W_e$ in $X$. Otherwise it acts by this stage and does so now. Thus every infinite [semidecidable set](../../../../../recursively-enumerable-set.md) meets $X$. Equivalently, its infinite [complement of a set](../../../../../complement-of-a-set.md) is an [immune set](../../../../../immune-set.md). **The constructed $X$ is semidecidable, coinfinite, and meets every infinite semidecidable set.**

As a useful check on the construction, $X$ cannot be a [computable set](../../../../../computable-set.md). If it were, its infinite [complement of a set](../../../../../complement-of-a-set.md) would also be a [computably enumerable set](../../../../../recursively-enumerable-set.md) disjoint from $X$, contradicting the property just proved. The argument requires neither deciding which $W_e$ are infinite nor protecting a prechosen infinite list of omitted numbers; the numerical witness bound provides all the required room.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
