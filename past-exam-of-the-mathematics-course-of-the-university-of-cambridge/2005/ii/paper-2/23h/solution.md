<h1 id="23h/solution">Solution</h1>

↑ **Parent:** [23H](../23h.md)

A [function element](../../../../../function-element.md) is a pair $(f,D)$ where $D$ is a nonempty disk and $f$ is holomorphic there; the germ at its center captures its local information. Elements continue one another when their [functions](../../../../../function-split.md) agree on an overlapping [connected](../../../../../connected-space.md) neighborhood. A [complete analytic function](../../../../../complete-analytic-function.md) is a maximal collection reachable from one element by chains of [analytic continuation](../../../../../analytic-continuation.md), including all further continuations of its members.

If $f^n=p$ in the initial disk, the [identity theorem](../../../../../identity-theorem.md) propagates this identity across every overlapping disk in a continuation chain. Induction along the chain proves **every element of the [complete analytic function](../../../../../complete-analytic-function.md) also satisfies $\widetilde f^{\,n}=p$**.

Put $F(z,w)=w^n-p(z)$. Its gradient is $(-p'(z),nw^{n-1})$. At a point of the curve with $w\ne0$, the second entry is nonzero; at $w=0$, the root of $p$ is simple and the first entry is nonzero. Thus the [holomorphic implicit function theorem](../../../../../holomorphic-implicit-function-theorem.md) supplies charts. Its precise local statement is that a holomorphic equation with nonzero derivative in one variable can locally be solved uniquely and holomorphically for that variable as a function of the other. For $w\ne0$, use $z$ as coordinate and write $w=w(z)$; at a simple root use $w$ as coordinate and write $z=z(w)$. The transition maps are holomorphic with nonzero derivatives, giving a [Riemann surface](../../../../../riemann-surfaces.md). The two [projections](../../../../../projection-linear-algebra.md) are holomorphic because they are holomorphic expressions in either kind of chart.

Away from the zeros of $p$, the projection onto $z$ is an unramified $n$-sheeted covering. A germ of a root corresponds to $(z,f(z))$ and its analytic continuations follow this covering. Near a simple root, $z-z_0$ is a nonzero analytic factor times $w^n$; a circuit about $z_0$ cyclically permutes all $n$ branches. For nonconstant square-free $p$, these circuits connect all sheets. Hence the germ surface $S(F)$ is the curve with the points over the roots removed, and **$C$ is its branched completion obtained by adding those ramification points**. An ordinary function element in the variable $z$ cannot include such a point: the zero order of a holomorphic $n$th power is divisible by $n$, whereas $p$ has zero order one. If a convention already includes these branch points in the [Riemann surface](../../../../../riemann-surfaces.md) of a multivalued function, that completed surface is $C$ itself. For a nonzero constant $p$, the curve has $n$ separate components, and the chosen element determines just one of them. The identically zero polynomial is excluded by the non-singularity premise.

## ↑ Ancestors (10)

1. [23H](../23h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
