<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

We use complex representations. By [Maschke's theorem](../../../../../../maschke-s-theorem.md), restriction to any finite subgroup is a [semisimple module](../../../../../../semisimple-module.md), so it has a canonical [isotypic decomposition](../../../../../../isotypic-decomposition.md). In particular, the $\theta$-[isotypic component](../../../../../../isotypic-component.md) $W_\theta$ is the sum of all copies of the irreducible $N$-module with character $\theta$. The central [character idempotent](../../../../../../character-idempotent.md)

$$
e_\theta=\frac{\theta(1)}{|N|}\sum_{n\in N}\theta(n^{-1})n
$$

projects onto this component. These projections preserve every $N$-submodule, which consequently decomposes as the [direct sum](../../../../../../direct-sum.md) of its intersections with the [isotypic components](../../../../../../isotypic-component.md).

Let $W$ afford $\xi\in\operatorname{Irr}(T\mid\theta)$. The component $W_\theta$ is nonzero. Since $T=I_G(\theta)$ fixes $\theta$, it preserves $W_\theta$. Irreducibility of $W$ as a $T$-module therefore gives $W=W_\theta$: its restriction to $N$ consists entirely of copies of $\theta$.

Form the [induced representation](../../../../../../induced-representation.md)

$$
V=\mathbb C[G]\otimes_{\mathbb C[T]}W=\bigoplus_{g\in\mathcal R}g\otimes W,
$$

where $\mathcal R$ represents the left cosets $G/T$. Because $N\triangleleft G$, for $n\in N$ we have

$$
n(g\otimes w)=g\otimes(g^{-1}ng)w.
$$

Thus $g\otimes W$ is $N$-isotypic of type $\theta^g$, where $\theta^g(n)=\theta(g^{-1}ng)$. These types are distinct for distinct cosets $gT$, precisely by the definition of the [inertia group of a character](../../../../../../inertia-group-of-a-character.md) $T$.

Let $Y$ be a nonzero $G$-submodule of $V$. Its [isotypic decomposition](../../../../../../isotypic-decomposition.md) as an $N$-module shows that it meets some $g\otimes W$ nontrivially. Acting by $g^{-1}$ gives $Y\cap(1\otimes W)\ne0$. This intersection is a $T$-submodule of the irreducible $W$, hence equals $1\otimes W$. The $G$-translates of that component span $V$, so $Y=V$. The induced representation is therefore irreducible, and its restriction contains $\theta$. Its [induced character](../../../../../../induced-character.md) satisfies

$$
\boxed{\xi^G\in\operatorname{Irr}(G\mid\theta).}
$$

This proves the irreducibility assertion directly from [isotypic components](../../../../../../isotypic-component.md); no form of the correspondence being proved has been assumed.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
