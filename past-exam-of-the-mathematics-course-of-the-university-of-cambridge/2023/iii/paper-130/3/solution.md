<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

[Hindman theorem](../../../../../hindman-theorem.md) states that every [finite coloring](../../../../../finite-coloring.md) of $\mathbb N$ admits an infinite sequence $x_1,x_2,\ldots$ whose [finite-sums set](../../../../../finite-sums-set.md) is monochromatic.

Identify the [Stone-Čech compactification of the natural numbers](../../../../../stone-cech-compactification-of-the-natural-numbers.md) $\beta\mathbb N$ with the compact Hausdorff space of [ultrafilters](../../../../../ultrafilter.md) on $\mathbb N$, equipped with [addition on the Stone-Čech compactification of the natural numbers](../../../../../addition-on-the-stone-cech-compactification-of-the-natural-numbers.md). This makes $\beta\mathbb N$ a compact Hausdorff left-topological [semigroup](../../../../../semigroup.md). For completeness, the [Ellis–Numakura lemma](../../../../../ellis-numakura-lemma.md) gives an idempotent in every such semigroup: by the [Hausdorff space](../../../../../hausdorff-space.md) property and [compactness](../../../../../compact-space.md), the intersection of a descending chain of nonempty compact subsemigroups is nonempty, so Zorn's lemma gives a minimal one $K$. For $a\in K$, the compact subsemigroup $K+a$ equals $K$. Hence the nonempty compact subsemigroup

$$
\{x\in K:x+a=a\}
$$

is also $K$, and in particular $a+a=a$. Choose the resulting [idempotent ultrafilter on the natural numbers](../../../../../idempotent-ultrafilter-on-the-natural-numbers.md) $\mathcal U$.

One color class $A$ belongs to $\mathcal U$. For $x\in\mathbb N$, write

$$
A-x=\{y:x+y\in A\},
$$

and define

$$
A^*=\{x\in A:A-x\in\mathcal U\}.
$$

The identity $\mathcal U+\mathcal U=\mathcal U$ implies $A^*\in\mathcal U$. It also implies that $A^*-x\in\mathcal U$ for every $x\in A^*$: both $A-x$ and the set of $y$ for which $A-(x+y)$ belongs to $\mathcal U$ lie in $\mathcal U$, and their intersection is $A^*-x$.

Choose $x_1\in A^*$. Having chosen $x_1,\ldots,x_n$ with every nonempty finite sum in $A^*$, choose

$$
x_{n+1}\in A^*\cap
\bigcap_{s\in\operatorname{FS}(x_1,\ldots,x_n)}(A^*-s).
$$

This is possible because it is a finite intersection of members of the [ultrafilter](../../../../../ultrafilter.md) $\mathcal U$. Every old finite sum remains in $A^*$, and every new one has the form $s+x_{n+1}$ and also lies in $A^*$. By [mathematical induction](../../../../../mathematical-induction.md), all nonempty finite sums lie in $A^*\subseteq A$, proving Hindman's theorem.

Now put

$$
S_A=\{x_n:n\in A\}
$$

for each $A\in\mathcal U$. If $A_1,\ldots,A_r\in\mathcal U$, then their intersection belongs to $\mathcal U$ and is nonempty, while

$$
S_{A_1\cap\cdots\cap A_r}\subseteq S_{A_1}\cap\cdots\cap S_{A_r}.
$$

Thus the sets $S_A$ have the [finite intersection property](../../../../../finite-intersection-property.md). Their [closures](../../../../../closure-topology.md) are closed subsets of the compact interval $[0,1]$, so their total intersection contains some $x$. Equivalently, every [neighbourhood](../../../../../neighbourhood-mathematics.md) of $x$ meets every $S_A$; this is the [ultrafilter limit](../../../../../ultralimit.md) of the sequence.

The point is unique. If distinct points $x,y$ both had this property, choose disjoint neighborhoods $U,V$. The index set $I_U=\{n:x_n\in U\}$ must belong to $\mathcal U$, because otherwise its complement would belong to $\mathcal U$ and the associated $S_A$ would miss $U$. Similarly $I_V\in\mathcal U$. Their intersection is empty, contradicting the definition of an ultrafilter.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 130](../../paper-130-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
