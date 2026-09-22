<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

If $x\in J$, part (ii) makes $1-x/\lambda$ invertible for every nonzero scalar $\lambda$. Thus $\sigma(x)\subseteq\{0\}$ and $r(x)=0$: it is a [quasinilpotent element](../../../../../../quasinilpotent-element.md). Conversely, let $I$ be a two-sided [ideal](../../../../../../ideal.md) consisting of quasinilpotent elements. For $x\in I$ and $y\in A$, $yx\in I$ has spectrum $\{0\}$, so $1+yx$ is invertible. Part (ii) implies $x\in J$. This proves **$J$ is the greatest ideal contained in the quasinilpotent set**, the [Jacobson radical as greatest quasinilpotent ideal](../../../../../../jacobson-radical-as-greatest-quasinilpotent-ideal.md) characterization.

A [semisimple Banach algebra](../../../../../../semisimple-banach-algebra.md) is one with $J=\{0\}$. For $B=\mathcal B(X)$, its natural action on $X$ is faithful and algebraically irreducible. Indeed, given $v\ne0$ and any $w\in X$, the [Hahn-Banach theorem](../../../../../../hahn-banach-theorem.md) gives a bounded functional $g$ with $g(v)=1$. The [rank-one operator](../../../../../../rank-one-operator.md) $z\mapsto g(z)w$ then maps $v$ to $w$. Any invariant subspace containing $v$ consequently contains every $w$. The faithful representation has kernel zero, so **zero is primitive and $B$ is semisimple**.

Nevertheless, choose a nonzero bounded functional $g$ and $0\ne x_0\in\ker g$, possible when $\dim X>1$. The nonzero rank-one operator $Tz=g(z)x_0$ satisfies $T^2z=g(z)g(x_0)x_0=0$. Hence $\sigma(T)=\{0\}$ and $r(T)=0$, although $T\ne0$. This proves **the quasinilpotent set of $B$ is not $\{0\}$**; it is not the same as the radical.

For infinite-dimensional $X$, the finite-rank operators form a nonzero proper two-sided ideal: products with bounded operators are finite-rank, and the identity has infinite rank. Thus zero is not maximal. Even if maximal ideals are required to be closed, the [compact operators](../../../../../../compact-operator-split.md) give a nonzero proper closed ideal containing the finite-rank operators. The identity is not compact on an infinite-dimensional Banach space, since the [Riesz lemma](../../../../../../riesz-s-lemma.md) supplies a bounded sequence with pairwise distances bounded below. Therefore **zero is primitive but not maximal in infinite dimension**.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
