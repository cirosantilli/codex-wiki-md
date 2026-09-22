<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Recall that a [flasque sheaf](../../../../../../flasque-sheaf.md) has surjective restriction maps on every inclusion of open subsets. We first prove the [flasque-kernel section-lifting lemma](../../../../../../flasque-kernel-section-lifting-lemma.md): in an exact sequence $0\to\mathcal A\to\mathcal B\to\mathcal C\to0$ of [sheaves](../../../../../../sheaf-mathematics.md), with $\mathcal A$ a [flasque sheaf](../../../../../../flasque-sheaf.md), every section of $\mathcal C$ on any open subset $V$ lifts to a section of $\mathcal B$ on $V$.

Fix such a section $c$. Order its lifts on open subsets $W\subseteq V$ by extension. A chain has an upper bound by the [sheaf gluing axiom](../../../../../../sheaf-gluing-axiom.md), so [Zorn's lemma](../../../../../../zorn-s-lemma.md) gives a maximal lift $b_W$. If $W\ne V$, choose a point outside $W$ and a neighborhood $T\subseteq V$ on which $c$ has a local lift $b_T$. On $W\cap T$, the difference $b_T-b_W$ is a section of $\mathcal A$. Extend it to $T$ by [flasqueness](../../../../../../flasque-sheaf.md) and subtract it from $b_T$. The corrected lift now agrees with $b_W$ and glues on $W\cup T$, contradicting maximality. Thus $W=V$, proving the lemma.

It follows also that if both $\mathcal A$ and $\mathcal B$ are [flasque sheaves](../../../../../../flasque-sheaf.md), then $\mathcal C$ is a [flasque sheaf](../../../../../../flasque-sheaf.md). Given a section of $\mathcal C$ on $U\subseteq V$, first lift it to $\mathcal B$ on $U$, extend that lift to $V$, and project to $\mathcal C$.

Next, an [injective sheaf of modules](../../../../../../injective-sheaf-of-modules.md) $\mathcal I$ is a [flasque sheaf](../../../../../../flasque-sheaf.md). For $U\subseteq V$, let $j_U$ and $j_V$ denote the open inclusions into $X$. [Extension by zero](../../../../../../extension-by-zero.md) gives a monomorphism $j_{U!}\mathcal O_U\to j_{V!}\mathcal O_V$: on every [stalk](../../../../../../stalk-of-a-sheaf.md) it is either $0\to\mathcal O_{X,x}$, the identity, or $0\to0$. By the adjunction for [extension by zero](../../../../../../extension-by-zero.md),

$$
\operatorname{Hom}_{\mathcal O_X}(j_{U!}\mathcal O_U,\mathcal I)=\Gamma(U,\mathcal I).
$$

Injectivity therefore makes $\Gamma(V,\mathcal I)\to\Gamma(U,\mathcal I)$ surjective. This proves [injective module sheaves are flasque](../../../../../../injective-module-sheaves-are-flasque.md).

Take an [injective resolution of sheaves](../../../../../../injective-resolution-of-sheaves.md) of $\mathcal F$. Write $\mathcal C^0=\mathcal F$ and, successively,

$$
0\longrightarrow\mathcal C^r\longrightarrow\mathcal I^r\longrightarrow\mathcal C^{r+1}\longrightarrow0.
$$

The initial $\mathcal C^0$ is a [flasque sheaf](../../../../../../flasque-sheaf.md); each $\mathcal I^r$ is a [flasque sheaf](../../../../../../flasque-sheaf.md); and the quotient argument proves inductively that all $\mathcal C^r$ are [flasque sheaves](../../../../../../flasque-sheaf.md). The section-lifting lemma makes each displayed sequence exact after [global sections](../../../../../../global-section.md). Consequently the complex of [global sections](../../../../../../global-section.md) of the [injective resolution of sheaves](../../../../../../injective-resolution-of-sheaves.md) has zero positive cohomology. Since that complex defines [sheaf cohomology](../../../../../../sheaf-cohomology.md),

$$
\boxed{H^p(X,\mathcal F)=0\quad(p>0).}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
