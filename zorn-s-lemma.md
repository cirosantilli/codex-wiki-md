<h1 id="zorn-s-lemma">Zorn's lemma</h1>

↑ **Parent:** [Set theory](set-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Zorn's_lemma)

Let $(P,\leq)$ be a nonempty [partially ordered set](partially-ordered-set.md). If every [chain in a partial order](chain-in-a-partial-order.md) $C\subseteq P$ has an [upper bound](upper-bound-in-a-partially-ordered-set.md) in $P$, then $P$ has a [maximal element](maximal-element-of-a-partially-ordered-set.md). The hypothesis means

$$
\forall C\subseteq P\text{ that is a chain},\quad
\exists u\in P\quad\forall c\in C,\ c\leq u.
$$

The [upper bound](upper-bound-in-a-partially-ordered-set.md) may depend on $C$ and need not belong to $C$. A [least upper bound](least-upper-bound-in-a-partially-ordered-set.md) is not required. The conclusion asserts that some $m\in P$ satisfies $m\leq x\Longrightarrow x=m$; it does not assert a [greatest element](greatest-element.md), which would satisfy $x\leq m$ for every $x\in P$.[How to use Zorn’s lemma, “General discussion”: statement and distinction between maximal and bigger than everything else](how-to-use-zorn%E2%80%99s-lemma-by-timothy-gowers.md)

Here a [chain in a partial order](chain-in-a-partial-order.md) may be the [empty set](empty-set.md). Every member of $P$ is an [upper bound](upper-bound-in-a-partially-ordered-set.md) of the empty [chain in a partial order](chain-in-a-partial-order.md), so including it in the hypothesis already forces $P$ to be nonempty. If “chain” means only nonempty [chains in a partial order](chain-in-a-partial-order.md), the separate nonempty-$P$ assumption is essential: the empty [poset](partially-ordered-set.md) otherwise satisfies the hypothesis vacuously and has no [maximal element](maximal-element-of-a-partially-ordered-set.md). These are two equivalent conventions for the theorem.

The strength of [Zorn's lemma](zorn-s-lemma.md) is that compatible partial constructions can have a completed, unextendible member without an explicit procedure for finding it. The next examples separate the [upper bound](upper-bound-in-a-partially-ordered-set.md) calculation from the reason a [maximal element](maximal-element-of-a-partially-ordered-set.md) has the desired property. All [chains in a partial order](chain-in-a-partial-order.md) must be covered, including uncountable ones, rather than just increasing [sequences](sequence.md). The condition is sufficient, not necessary: a [poset](partially-ordered-set.md) can have a [maximal element](maximal-element-of-a-partially-ordered-set.md) and still have an unbounded [chain in a partial order](chain-in-a-partial-order.md) elsewhere.

**Table of contents**

- [Zorn's lemma in a finite poset](zorn-s-lemma-in-a-finite-poset.md)
- [Vector space bases from Zorn's lemma](vector-space-bases-from-zorn-s-lemma.md)
- [Finite greedy basis extension and choice](finite-greedy-basis-extension-and-choice.md)
- [Proof outline of Zorn's lemma](proof-outline-of-zorn-s-lemma.md)

## ↑ Ancestors (5)

1. [Set theory](set-theory-split.md)
2. [Foundations of mathematics](foundations-of-mathematics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (40)

- [Convex domination form of the Hahn-Banach theorem](convex-domination-form-of-the-hahn-banach-theorem.md)
- [Discontinuous additive function](discontinuous-additive-function.md)
- [Existence of minimal primes over a proper ideal](existence-of-minimal-primes-over-a-proper-ideal.md)
- [Finite greedy basis extension and choice](finite-greedy-basis-extension-and-choice.md)
- [One-dimensional dominated extension of a real linear functional](one-dimensional-dominated-extension-of-a-real-linear-functional.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-6/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-10/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-4/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-4/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-36/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-6/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-6/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-6/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-8/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-8/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-4/16g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-16/2/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-16/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-3/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-6/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-6/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-10/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-4/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-83/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-1/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-1/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-6/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-9/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-1/13i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-1/1/solution.md)
- [Proof outline of Zorn's lemma](proof-outline-of-zorn-s-lemma.md)
- [Sandwich form of the Hahn-Banach theorem](sandwich-form-of-the-hahn-banach-theorem.md)
- [Szpilrajn extension theorem](szpilrajn-extension-theorem.md)
- [Valuation domination lemma](valuation-domination-lemma.md)
- [Value in a lattice-ordered group](value-in-a-lattice-ordered-group.md)
- [Vector space bases from Zorn's lemma](vector-space-bases-from-zorn-s-lemma.md)
- [Vector-space freeness from maximal independence](vector-space-freeness-from-maximal-independence.md)
- [Zorn's lemma](zorn-s-lemma.md)
- [Zorn's lemma in a finite poset](zorn-s-lemma-in-a-finite-poset.md)
