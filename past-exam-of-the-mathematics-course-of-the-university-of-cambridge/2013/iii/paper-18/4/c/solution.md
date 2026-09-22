<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [currying adjunction for small categories](../../../../../../currying-adjunction-for-small-categories.md) uses the [bijection](../../../../../../bijection.md)

$$
\operatorname{Fun}(\mathcal D\times\mathcal C,\mathcal E)
\cong\operatorname{Fun}(\mathcal D,[\mathcal C,\mathcal E]).
$$

It sends $H$ to the [functor](../../../../../../functor.md) $d\mapsto H(d,-)$, with an arrow $u:d\to d'$ inducing the [natural transformation](../../../../../../natural-transformation.md) whose $c$-component is $H(u,1_c)$. Conversely, for $K:\mathcal D\to[\mathcal C,\mathcal E]$, define its uncurried [functor](../../../../../../functor.md) by $(d,c)\mapsto K(d)(c)$ and

$$
(u,v):(d,c)\to(d',c')\quad\longmapsto\quad K(d')(v)K(u)_c.
$$

Naturality of $K(u)$ allows the two factors to be interchanged in the appropriate order, giving functoriality. The constructions are inverse and natural in $\mathcal D$ and $\mathcal E$. Hence $-\times\mathcal C$ is a [left adjoint](../../../../../../adjoint-functors.md) to $[\mathcal C,-]$ on the [category of small categories](../../../../../../category-of-small-categories.md).

The unit sends $d$ to the [functor](../../../../../../functor.md) $c\mapsto(d,c)$ and $u$ to the transformation $(u,1_c)$. The counit is evaluation $[\mathcal C,\mathcal E]\times\mathcal C\to\mathcal E$: $(H,c)\mapsto H(c)$ and $(\alpha,v)\mapsto H'(v)\alpha_c=\alpha_{c'}H(v)$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
