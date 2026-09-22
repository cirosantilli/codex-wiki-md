<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [flasque sheaf](../../../../../../flasque-sheaf.md) has surjective restriction maps $\mathcal F(V)\to\mathcal F(U)$ for every pair of opens $U\subseteq V$. To prove the claim for an [injective sheaf of modules](../../../../../../injective-sheaf-of-modules.md), let $j_U:U\hookrightarrow X$ and $j_V:V\hookrightarrow X$. The natural map

$$
(j_U)_!\mathcal O_U\longrightarrow(j_V)_!\mathcal O_V
$$

is a monomorphism: its [stalks](../../../../../../stalk-of-a-sheaf.md) are either the identity on $\mathcal O_{X,x}$, the map from zero to that stalk, or the zero-to-zero map. Here $j_!$ is [extension by zero](../../../../../../extension-by-zero.md) for module sheaves.

The extension-by-zero adjunction identifies

$$
\operatorname{Hom}_{\mathcal O_X}((j_U)_!\mathcal O_U,I)\cong\Gamma(U,I).
$$

The [injective object](../../../../../../injective-object.md) property extends every morphism from $(j_U)_!\mathcal O_U$ to one from $(j_V)_!\mathcal O_V$. Under the displayed identification this is exactly surjectivity of $I(V)\to I(U)$. **Injective module sheaves are therefore flasque.** This argument works on an arbitrary [ringed space](../../../../../../ringed-space-split.md), without Noetherian or separation assumptions.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 113](../../../paper-113-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
