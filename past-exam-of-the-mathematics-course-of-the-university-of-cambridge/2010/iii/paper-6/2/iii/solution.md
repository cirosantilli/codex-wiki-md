<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**False.** Take the separable [Banach space](../../../../../../banach-space-split.md) $E=\ell^1$, whose [continuous dual space](../../../../../../continuous-dual-space-split.md) is $\ell^\infty$. We prove that first countability of the weak unit ball would force this dual to be norm separable, producing a contradiction.

Suppose that $B$ had a countable weak neighbourhood base $(U_n)$ at zero. Inside each $U_n$, choose a basic relative weak neighbourhood specified by finitely many [continuous linear functionals](../../../../../../continuous-linear-functional.md) $F_n$. The union $F=\bigcup_nF_n$ is countable. For any $f\in E'$ and $\epsilon>0$, some $U_n$ lies in $\{x\in B:|f(x)|<\epsilon\}$. On the [vector subspace](../../../../../../vector-subspace.md)

$$
M_n=\bigcap_{g\in F_n}\ker g,
$$

this implies $\|f|_{M_n}\|\leq\epsilon$, by scaling vectors into $B$. The [Hahn-Banach theorem](../../../../../../hahn-banach-theorem.md) extends $f|_{M_n}$ to $h\in E'$ with $\|h\|\leq\epsilon$. The functional $f-h$ vanishes on $M_n$ and is therefore a linear combination of $F_n$: it factors through the finite-dimensional coordinate map $x\mapsto(g(x))_{g\in F_n}$, and a [linear functional](../../../../../../linear-functional.md) on that map's image extends to the finite-dimensional coordinate space. Hence

$$
\operatorname{dist}(f,\operatorname{span}F_n)\leq\epsilon.
$$

Every $f\in E'$ thus belongs to the norm closure of $\operatorname{span}F$. Taking rational coefficients, or rational real and imaginary parts, gives a countable norm-dense subset of $E'$. This proves that [weak-ball metrizability requires a norm-separable dual](../../../../../../weak-ball-metrizability-requires-a-norm-separable-dual.md).

For $\ell^1$, every bounded sequence $a=(a_j)$ defines $f_a(x)=\sum_ja_jx_j$ with $\|f_a\|=\|a\|_\infty$. Conversely, the values $f(e_j)$ of any bounded [linear functional](../../../../../../linear-functional.md) determine such a sequence and recover $f$ by density of finitely supported vectors. Thus $E'=\ell^\infty$. The uncountable family $\{0,1\}^{\mathbb N}$ in $\ell^\infty$ has distance one between distinct members, so this dual is not norm separable: disjoint balls of radius less than $1/2$ would require distinct members of any countable dense set. Since every metrizable space is first countable, the weak unit ball of $\ell^1$ is not metrizable.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
