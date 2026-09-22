<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An $\mathcal O_X$-module $\mathcal F$ is a [quasi-coherent sheaf](../../../../../../quasi-coherent-sheaf.md) when every affine open $V=\operatorname{Spec}A\subseteq X$ has $\mathcal F|_V\cong\widetilde M$ for some $A$-module $M$. For a morphism $f:X\to Y$, its [direct image sheaf](../../../../../../direct-image-sheaf.md) is

$$
(f_*\mathcal F)(V)=\mathcal F(f^{-1}V),
$$

while the [pullback of a sheaf of modules](../../../../../../pullback-of-a-sheaf-of-modules.md) is

$$
f^*\mathcal G=\mathcal O_X\otimes_{f^{-1}\mathcal O_Y}f^{-1}\mathcal G.
$$

If $i:Z\hookrightarrow X$ is a [closed immersion](../../../../../../closed-immersion.md) of [Noetherian schemes](../../../../../../noetherian-scheme.md), then on an affine open $V=\operatorname{Spec}A\subseteq X$ one has $Z\cap V=\operatorname{Spec}(A/I)$. The restriction of $i_*\mathcal O_Z$ corresponds to the cyclic $A$-module $A/I$, so it is finitely generated. Hence $i_*\mathcal O_Z$ is a [coherent sheaf](../../../../../../coherent-sheaf.md); more generally this is the [direct image of a coherent sheaf under a closed immersion](../../../../../../direct-image-of-a-coherent-sheaf-under-a-closed-immersion.md).

Coherence need not survive an arbitrary pushforward. Let

$$
j:D(x)=\operatorname{Spec}k[x,x^{-1}]\hookrightarrow\operatorname{Spec}k[x]
$$

be the [open immersion](../../../../../../open-immersion.md). The sheaf $\mathcal O_{D(x)}$ is coherent, but

$$
\Gamma(\mathbb A^1,j_*\mathcal O_{D(x)})=k[x,x^{-1}]
$$

is not a finitely generated $k[x]$-module. Therefore $j_*\mathcal O_{D(x)}$ is not coherent.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 113](../../../paper-113-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
