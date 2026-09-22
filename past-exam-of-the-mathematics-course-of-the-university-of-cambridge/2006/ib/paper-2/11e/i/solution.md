<h1 id="11e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\mathcal S$ be the set of all subsets of $G$ with $p^n$ elements. First show that $|\mathcal S|=\binom{p^nr}{p^n}$ is not divisible by $p$. In the [polynomial](../../../../../../polynomial-split.md) ring over the [field](../../../../../../field.md) of $p$ elements, $(1+X)^p=1+X^p$, since the intermediate binomial coefficients are divisible by $p$. Iterating gives

$$
(1+X)^{p^nr}=(1+X^{p^n})^r\pmod p.
$$

Comparison of coefficients of $X^{p^n}$ yields $\binom{p^nr}{p^n}\equiv r\not\equiv0\pmod p$.

Let $G$ act on $\mathcal S$ by left translation. Because its [orbit](../../../../../../orbit-dynamical-system.md) sizes sum to a number not divisible by $p$, some [orbit](../../../../../../orbit-dynamical-system.md) has size prime to $p$. Choose a subset $S$ in that [orbit](../../../../../../orbit-dynamical-system.md), with [stabilizer](../../../../../../stabilizer-subgroup.md) $H$. The [orbit-stabilizer theorem](../../../../../../orbit-stabilizer-theorem.md) gives the [orbit](../../../../../../orbit-dynamical-system.md) size $[G:H]$, so $p\nmid[G:H]$. On the other hand $H$ acts freely on the elements of $S$: if $hs=s$, cancellation in the [group](../../../../../../group-split.md) gives $h=1$. Every $H$-orbit in $S$ therefore has $|H|$ elements, and $|H|$ divides $|S|=p^n$. Since

$$
p^nr=|G|=|H|[G:H]
$$

and the second factor has no factor of $p$, the first must contain all $p^n$. Hence $\boxed{|H|=p^n}$, proving the first of the [Sylow theorems](../../../../../../sylow-theorems.md). This is [Sylow existence by subset action](../../../../../../sylow-existence-by-subset-action.md) and includes the trivial case $n=0$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [11E](../../11e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
