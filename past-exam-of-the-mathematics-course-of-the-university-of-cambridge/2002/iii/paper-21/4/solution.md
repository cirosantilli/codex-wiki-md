<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For the effective counterexample, let $K$ be the [diagonal halting set](../../../../../diagonal-halting-set.md) and let $K_s$ be the finite approximation obtained by running the first $s$ programs for $s$ steps. For $x<y<z$, define the [recursive triple colouring with no computable infinite homogeneous set](../../../../../recursive-triple-colouring-with-no-computable-infinite-homogeneous-set.md) by

$$
c(\{x,y,z\})=\begin{cases}0,&K_y\cap\{0,\ldots,x\}=K_z\cap\{0,\ldots,x\},\\1,&\text{otherwise}.\end{cases}
$$

This is a total recursive two-coloring: only bounded computations are involved. An infinite [homogeneous set](../../../../../homogeneous-set-for-a-colouring.md) $H$ cannot have color one. Fix $x\in H$ and take $y,z\in H$ sufficiently large that every halting computation with index at most $x$ that ever halts has already halted by stage $y$; then the color is zero. If $H$ has color zero, it computes $K$: given $e$, find $x<y$ in $H$ with $x\ge e$ and inspect $K_y(e)$. Agreement with every later stage $z\in H$, and the unboundedness of $H$, give $K_y\cap\{0,\ldots,x\}=K\cap\{0,\ldots,x\}$. Hence this is the correct answer. The [set](../../../../../set-split.md) $K$ is not recursive: a purported halting decider would produce a program that halts exactly when the decider says it does not halt on its own index. Thus **there is no recursive infinite [homogeneous set](../../../../../homogeneous-set-for-a-colouring.md)**. Here infinite is essential: every finite [subset](../../../../../subset.md) is recursive, and [sets](../../../../../set-split.md) with fewer than three elements are vacuously homogeneous.

A precise finite-arity [Erdős-Rado theorem for finite arities](../../../../../erdos-rado-theorem-for-finite-arities.md) is

$$
\boxed{\beth_r(\lambda)^+\longrightarrow(\lambda^+)^{r+1}_\lambda\quad(r<\omega,\ \lambda\text{ an infinite cardinal}),}
$$

where $\beth_0(\lambda)=\lambda$ and $\beth_{r+1}(\lambda)=2^{\beth_r(\lambda)}$. We prove the [closed elementary-submodel construction of an end-homogeneous sequence](../../../../../closed-elementary-submodel-construction-of-an-end-homogeneous-sequence.md) and then induct. We work with [AC](../../../../../axiom-of-choice.md), as in the usual [cardinal](../../../../../cardinal-number.md) partition calculus.

Put $\theta=(2^\mu)^+$, where $\mu$ is infinite, and let $c:[\theta]^{m+1}\to\lambda$ with $\lambda\le\mu$ and $m\ge1$. Choose a [regular cardinal](../../../../../regular-cardinal.md) $\chi$ large enough that this coloring and its domain belong to $H_\chi$, the [sets](../../../../../set-split.md) of hereditary size below $\chi$. There is $M\prec H_\chi$ of size $2^\mu$ containing $c,\theta,\mu$, every [ordinal](../../../../../ordinal.md) below $\mu^+$, and closed under externally given [sequences](../../../../../sequence.md) of length at most $\mu$. Here is the closure construction: start with a [Skolem hull](../../../../../skolem-hull.md) of the named parameters and the [ordinals](../../../../../ordinal.md) below $\mu^+$; iterate hulls after adjoining all at-most-$\mu$-sequences of the preceding hull for $\mu^+$ stages. Every stage and the [union](../../../../../set-union.md) have size $2^\mu$, since $(2^\mu)^\mu=2^\mu$ and $\mu^+\le2^\mu$. The [elementary chain theorem](../../../../../elementary-chain-theorem.md) gives elementarity. Any [sequence](../../../../../sequence.md) of at most $\mu$ members of the final [union](../../../../../set-union.md) lies in a bounded stage, because $\mu^+$ is regular, and is added at the next stage. This proves the required closure.

Let $\beta=\sup(M\cap\theta)$. Regularity of $\theta$ gives $\beta<\theta$, and $\beta\notin M$: otherwise $\beta+1$ would also belong to $M\cap\theta$. Recursively choose increasing $x_\alpha\in M\cap\theta$ for $\alpha<\mu^+$ so that, for every $m$-subset $u$ of the earlier points,

$$
c(u\cup\{x_\alpha\})=c(u\cup\{\beta\}).
$$

To justify the recursion, the earlier [sequence](../../../../../sequence.md) has length at most $\mu$, hence belongs to $M$. There are at most $\mu$ constraints. All their points and color values are in $M$, so their coded table belongs to $M$ by closure, even though $\beta$ itself is external to $M$. The supremum of the earlier points, plus one, also belongs to $M\cap\theta$ and is below $\beta$. Thus $\beta$ witnesses in $H_\chi$ that a point above that bound satisfying the table exists. Elementarity supplies such a point in $M$. This completes the recursion.

The [sequence](../../../../../sequence.md) is end-homogeneous: on any increasing $(m+1)$-tuple from it, the color depends only on its first $m$ entries. Define the induced $m$-tuple coloring by $g(u)=c(u\cup\{\beta\})$. For the [induction](../../../../../mathematical-induction.md), the arity-one assertion $\lambda^+\to(\lambda^+)^1_\lambda$ is the infinite pigeonhole principle: a [union](../../../../../set-union.md) of $\lambda$ [sets](../../../../../set-split.md) each of size at most $\lambda$ has size at most $\lambda$. At step $r\ge1$, take $\mu=\beth_{r-1}(\lambda)$, so $\theta=\beth_r(\lambda)^+$. The constructed [sequence](../../../../../sequence.md) has size $\mu^+=\beth_{r-1}(\lambda)^+$. The [induction](../../../../../mathematical-induction.md) hypothesis makes $g$ constant on a [subset](../../../../../subset.md) of size $\lambda^+$; end-homogeneity makes $c$ constant on its $(r+1)$-subsets. This proves the theorem. In particular $\lambda=\aleph_0$ gives an uncountable [homogeneous set](../../../../../homogeneous-set-for-a-colouring.md) for every finite-arity coloring with countably many colors, on a sufficiently large [cardinal](../../../../../cardinal-number.md).

There is no unrestricted infinite-exponent analogue under [AC](../../../../../axiom-of-choice.md). For any infinite [cardinal](../../../../../cardinal-number.md) $\kappa$, choose one representative $R$ from each equivalence class of $[\kappa]^\omega$ modulo [finite symmetric difference](../../../../../finite-symmetric-difference.md). Color $X$ by the parity of $|X\mathbin\triangle R|$. Removing one element of $X$ leaves it in the same class and reverses the parity. Every infinite proposed [homogeneous set](../../../../../homogeneous-set-for-a-colouring.md) contains both a countably infinite $X$ and $X\setminus\{x\}$, so cannot be homogeneous. Thus the [finite-symmetric-difference colouring of infinite subsets](../../../../../finite-symmetric-difference-colouring-of-infinite-subsets.md) proves

$$
\boxed{\kappa\not\longrightarrow(\omega)^\omega_2\quad\text{for every infinite }\kappa\text{, under AC}.}
$$

The contrast is between arbitrary colorings at countably infinite arity and the finite arities of the theorem; restrictions on the definability of an infinite-arity coloring can change the problem.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
