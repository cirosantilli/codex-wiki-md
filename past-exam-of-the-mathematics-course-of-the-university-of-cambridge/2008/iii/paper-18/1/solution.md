<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Excision theorem](../../../../../excision-theorem.md) for [singular homology](../../../../../singular-homology.md) states that if $Z\subseteq A\subseteq X$ and $\overline Z\subseteq\operatorname{int}_X A$, inclusion induces isomorphisms $H_q(X\setminus Z,A\setminus Z;\mathbb Z)\cong H_q(X,A;\mathbb Z)$ for all $q$. For an open cover $X=U\cup V$, its small-chain form says that the subcomplex of singular chains whose individual simplices lie in $U$ or $V$ computes $H_*(X)$. Concretely, repeated [barycentric subdivision](../../../../../barycentric-subdivision.md) puts each finite chain in that subcomplex, and subdivision is chain-homotopic to the identity. There is then a [short exact sequence of chain complexes](../../../../../short-exact-sequence-of-chain-complexes.md)

$$
0\longrightarrow C_*(U\cap V)\xrightarrow{c\mapsto(c,-c)}C_*(U)\oplus C_*(V)\xrightarrow{(a,b)\mapsto a+b}C_*^{\{U,V\}}(X)\longrightarrow0.
$$

Its [long exact sequence in homology](../../../../../long-exact-sequence-in-homology.md), with excision identifying the last complex's homology with $H_*(X)$, is the [Mayer–Vietoris sequence](../../../../../mayer-vietoris-sequence.md):

$$
\cdots\longrightarrow H_q(U\cap V)\xrightarrow{(i_*,-j_*)}H_q(U)\oplus H_q(V)\longrightarrow H_q(X)\longrightarrow H_{q-1}(U\cap V)\longrightarrow\cdots.
$$

The [Real projective space](../../../../../real-projective-space.md) $\mathbb{RP}^1$ is a circle. The projective plane has one cell in each dimension $0,1,2$, with [cellular homology](../../../../../cellular-chain-complex.md) boundary maps $d_2=2$ and $d_1=0$. Thus, writing $A_q=H_q(\mathbb{RP}^2;\mathbb Z)$, we have $A_0=\mathbb Z$, $A_1=\mathbb Z/2$ and $A_q=0$ for $q\geq2$. Cover the circle by two open arcs with a two-component intersection and multiply this cover by the projective plane. In the [Mayer–Vietoris sequence](../../../../../mayer-vietoris-sequence.md) the overlap-to-cover map is

$$
A_q\oplus A_q\longrightarrow A_q\oplus A_q,\qquad(a,b)\longmapsto(a+b,-a-b).
$$

Its kernel and cokernel are each $A_q$. Consequently $0\to A_q\to H_q(X)\to A_{q-1}\to0$ for $q\geq1$. In degree one the quotient is free, so this sequence splits; in degree two it identifies the group directly with $A_1$. The [integral homology of a circle times a real projective plane](../../../../../integral-homology-of-a-circle-times-a-real-projective-plane.md) is therefore

$$
\boxed{H_q(\mathbb{RP}^1\times\mathbb{RP}^2;\mathbb Z)=\begin{cases}\mathbb Z,&q=0,\\\mathbb Z\oplus\mathbb Z/2,&q=1,\\\mathbb Z/2,&q=2,\\0,&q\geq3.\end{cases}}
$$

Without a compactness restriction, the answer to the final existence question is **yes: there is a noncompact oriented four-manifold**. Explicitly, take

$$
Y=S^1\times\bigl((S^2\times\mathbb R)/((v,t)\sim(-v,-t))\bigr).
$$

The involution is free and reverses orientation on both $S^2$ and $\mathbb R$, hence preserves their product orientation. Its quotient is consequently an oriented three-manifold, the [orientable total space of the orientation line bundle](../../../../../orientable-total-space-of-the-orientation-line-bundle.md) of the projective plane. The contraction $[v,t]\mapsto[v,(1-s)t]$ is a [deformation retraction](../../../../../deformation-retraction.md) onto $\mathbb{RP}^2$, so $Y\simeq X$.

If a closed oriented manifold is intended, the answer instead is **no**. A closed connected oriented $d$-manifold has $H_d\cong\mathbb Z$ and no homology above $d$. Here the highest nonzero positive-dimensional homology is the torsion group $H_2=\mathbb Z/2$, so no dimension can supply that required top fundamental class. The distinction is necessary because the printed wording does not require the oriented manifold to be closed or three-dimensional.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
