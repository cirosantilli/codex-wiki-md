<h1 id="6d/solution">Solution</h1>

↑ **Parent:** [6D](../6d.md)

For fixed $g\in G$, conjugation $g_*:x\mapsto gxg^{-1}$ preserves multiplication:

$$
g_*(xy)=gxyg^{-1}=(gxg^{-1})(gyg^{-1}),
$$

and its inverse is $(g^{-1})_*$. It is therefore a [group automorphism](../../../../../group-automorphism.md). Furthermore,

$$
(gh)_*(x)=ghx(gh)^{-1}=g_*(h_*(x)),
$$

so $\theta:g\mapsto g_*$ is a homomorphism $G\to\operatorname{Aut}(G)$. Its kernel consists of elements commuting with every $x$, hence

$$
\boxed{\ker\theta=Z(G),\qquad \operatorname{im}\theta=\operatorname{Inn}(G).}
$$

For $\alpha\in\operatorname{Aut}(G)$,

$$
\alpha g_*\alpha^{-1}=(\alpha(g))_*,
$$

so the [inner automorphism group](../../../../../inner-automorphism.md) is normal in the [automorphism group](../../../../../automorphism-group.md).

If $G=\langle x\rangle$ is cyclic, every automorphism has the form $x\mapsto x^a$. Two such maps commute because $ab=ba$, so $\operatorname{Aut}(G)$ is abelian. The conclusion fails for general abelian groups: for $G=C_2\times C_2$, its three nonidentity elements may be permuted arbitrarily, giving

$$
\boxed{\operatorname{Aut}(C_2\times C_2)\cong S_3,}
$$

which is nonabelian.

## ↑ Ancestors (10)

1. [6D](../6d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
