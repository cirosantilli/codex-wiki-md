<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $N_G=\sum_{g\in G}g$. Its image on every module lies in the [invariant submodule](../../../../../../invariant-submodule.md), since $hN_G=N_G$. In the regular module,

$$
(kG)^G=kN_G,
$$

and this line is the socle of the projective cover $P_k$ of the trivial module.

Suppose $N_GM\ne0$. Choose $m\in M$ with $N_Gm\ne0$ and consider the homomorphism

$$
f:kG\longrightarrow M,
\qquad x\longmapsto xm.
$$

Its restriction $f|_{P_k}$ is nonzero on $\operatorname{Soc}(P_k)=kN_G$. Because $P_k$ is the [injective hull](../../../../../../injective-hull.md) of its simple socle, that socle is essential: every nonzero submodule meets it. Hence $\ker(f|_{P_k})=0$. The resulting embedding $P_k\hookrightarrow M$ splits because $P_k$ is injective. Since $M$ is indecomposable, $M\cong P_k$.

Conversely, on $P_k$ the image of $N_G$ is its one-dimensional socle. Thus the [group norm element detects the trivial projective cover](../../../../../../group-norm-element-detects-the-trivial-projective-cover.md):

$$
\boxed{
\dim_k(N_GM)=
\begin{cases}
1,&M\cong P_k,\\
0,&M\not\cong P_k.
\end{cases}}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 138](../../../paper-138-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
