<h1 id="16h/solution">Solution</h1>

↑ **Parent:** [16H](../16h.md)

A [first-order structure](../../../../../first-order-structure.md) consists of a nonempty domain, an interpretation of each constant as a domain element, each $k$-ary function symbol as a map from the $k$-fold domain product to the domain, and each $k$-ary relation symbol as a subset of that product. Under an assignment of values to variables, terms are evaluated recursively. Atomic formulas assert equality of term values or membership in an interpreted relation. Boolean connectives act on truth values, and quantifiers range over the whole domain. The set $[[\varphi]]_A$ consists of assignments to the free variables making the formula true.

For a [substructure](../../../../../substructure-of-a-first-order-structure.md) $B\subseteq A$, constants lie in $B$, functions restrict to $B$, and relations restrict to tuples from $B$. Induction on terms shows that every term with arguments from $B$ has the same value in both structures. Atomic formulas consequently have the same truth values, and induction on Boolean connectives gives

$$
\boxed{[[\varphi]]_B=[[\varphi]]_A\cap B^n}
$$

for every [quantifier-free formula](../../../../../quantifier-free-formula.md).

For a nonempty chain of $T$-model [substructures](../../../../../substructure-of-a-first-order-structure.md), form their union $U$. Every finite tuple belongs to one member of the chain, so $U$ is closed under all interpreted functions and contains the constants. Consider any inductive axiom $\forall x\,\exists y\,\psi(x,y)$. A specified finite tuple $x$ lies in one member, which supplies witnesses $y$ there. The [quantifier-free formula](../../../../../quantifier-free-formula.md) $\psi$ has the same truth value in that member and $U$, so $U$ satisfies the axiom. Hence $U$ is a $T$-model and the least upper bound of the chain. **The poset is complete for nonempty chains.** If chain-complete is defined to include the empty chain, a least element must additionally exist, which the stated hypotheses do not ensure.

## ↑ Ancestors (10)

1. [16H](../16h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
