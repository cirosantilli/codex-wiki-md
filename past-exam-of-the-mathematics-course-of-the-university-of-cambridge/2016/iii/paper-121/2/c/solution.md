<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The construction gives a [Lusin set](../../../../../../lusin-set.md) $\boxed{A=\{x_\alpha:\alpha<\omega_1\}}$ with all $x_\alpha$ distinct.

Every [meagre set](../../../../../../meagre-set.md) is contained in a meagre $F_\sigma$ set: replace each [nowhere dense set](../../../../../../nowhere-dense-set.md) in a countable covering by its closure. There are at most $2^{\aleph_0}$ such covers, since each closed subset of $\mathbb R$ is determined by a countable rational basis for its open complement, and a countable sequence of such codes is again coded by a real. Under the [Continuum hypothesis](../../../../../../continuum-hypothesis.md), enumerate all meagre $F_\sigma$ sets as $(M_\alpha)_{\alpha<\omega_1}$, allowing repetitions.

By [transfinite recursion](../../../../../../transfinite-recursion.md), choose

$$
x_\alpha\in\mathbb R\setminus\left(\bigcup_{\beta\leq\alpha}M_\beta\ \cup\ \{x_\beta:\beta<\alpha\}\right).
$$

For each $\alpha<\omega_1$, the excluded union is a [meagre set](../../../../../../meagre-set.md): it is a countable union of [meagre sets](../../../../../../meagre-set.md) and singletons. The [Baire category theorem](../../../../../../baire-category-theorem.md) ensures that it does not cover $\mathbb R$, so the choice is possible. The resulting $A$ is uncountable. If $M$ is meagre, choose $\gamma$ with $M\subseteq M_\gamma$. Every $x_\alpha$ with $\alpha\geq\gamma$ avoids $M_\gamma$, hence

$$
A\cap M\subseteq\{x_\alpha:\alpha<\gamma\},
$$

which is countable. Thus $A$ has precisely the [Lusin set](../../../../../../lusin-set.md) property. Enumerating covers rather than all [meagre sets](../../../../../../meagre-set.md) avoids an unjustified claim that there are only continuum many arbitrary meagre subsets.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
