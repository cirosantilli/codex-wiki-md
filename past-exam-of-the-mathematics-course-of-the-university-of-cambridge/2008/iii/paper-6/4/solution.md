<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $P=L\ltimes U$ and $Q=M\ltimes V$ be rational [parabolic subgroups](../../../../../parabolic-subgroup.md) with rational [Levi subgroups](../../../../../levi-subgroup.md). Work with complex representations of their [finite groups of Lie type](../../../../../finite-group-of-lie-type.md). Here [Harish-Chandra induction](../../../../../harish-chandra-induction.md) and [Harish-Chandra restriction](../../../../../harish-chandra-restriction.md) mean

$$
R_{L\subset P}^{G}(E)=\operatorname{Ind}_{P^F}^{G^F}\operatorname{Inf}_{L^F}^{P^F}E,\qquad {}^*R_{M\subset Q}^{G}(A)=A^{V^F}.
$$

The latter is an $M^F$-module, and it is adjoint to the former by [Frobenius reciprocity](../../../../../frobenius-reciprocity.md).

Define

$$
\mathcal S(M,L)=\{x\in G:M\cap{}^xL\text{ contains a maximal algebraic torus of }G\}.
$$

For $x\in\mathcal S(M,L)^F$, put $H_x=M\cap{}^xL$ and let $\operatorname{ad}x$ transport an $L^F$-module to a $({}^xL)^F$-module. The [Mackey formula for Harish-Chandra induction](../../../../../mackey-formula-for-harish-chandra-induction.md) is the natural functor isomorphism

$$
\boxed{{}^*R_{M\subset Q}^{G}R_{L\subset P}^{G}\cong\bigoplus_{x\in M^F\backslash\mathcal S(M,L)^F/L^F}R_{H_x\subset M\cap{}^xP}^{M}\ {}^*R_{H_x\subset Q\cap{}^xL}^{{}^xL}\ \operatorname{ad}x.}
$$

On [characters](../../../../../character-of-a-representation.md) the direct sum becomes a sum. The intersection parabolics displayed in the subscripts are important: they specify exactly which [Harish-Chandra induction](../../../../../harish-chandra-induction.md) and [Harish-Chandra restriction](../../../../../harish-chandra-restriction.md) occur.

We use the following parabolic-intersection lemmas, stating explicitly the geometric input to the proof. First, representatives of $M^F\backslash\mathcal S(M,L)^F/L^F$ represent exactly the double cosets $Q^F\backslash G^F/P^F$. Second, for such $x$, the groups $M\cap{}^xP$ and $Q\cap{}^xL$ are [parabolic subgroups](../../../../../parabolic-subgroup.md) of $M$ and ${}^xL$, respectively, with common [Levi subgroup](../../../../../levi-subgroup.md) $H_x$ and respective [unipotent radicals](../../../../../unipotent-radical.md) $M\cap{}^xU$ and $V\cap{}^xL$. If $K=Q\cap{}^xP$, projection $Q\to M$ maps $K$ onto $M\cap{}^xP$ with kernel $K\cap V$. Projection ${}^xP\to{}^xL$ maps $K\cap V$ onto $V\cap{}^xL$ with kernel $V\cap{}^xU$. These assertions hold on rational points as well. The surjectivity on rational points uses connectedness of the unipotent kernels and the [Lang theorem for algebraic groups](../../../../../lang-theorem-for-algebraic-groups.md). These are the compatible-Levi and rational double-coset lemmas; they follow by applying the root-subgroup decomposition after choosing the common [maximal algebraic torus](../../../../../maximal-algebraic-torus.md).

For completeness, the representation-theoretic reduction is as follows. The [group algebra](../../../../../group-algebra.md) realization of [induced representation](../../../../../induced-representation.md) splits according to the double cosets:

$$
\mathbb C[G^F]=\bigoplus_x\mathbb C[Q^FxP^F]
$$

as a $(Q^F,P^F)$-bimodule. Tensoring on the right with an inflated $L^F$-module $E$ identifies each summand with induction from $K^F=(Q\cap{}^xP)^F$. This proves the finite-group [Mackey restriction formula](../../../../../mackey-restriction-formula.md) in the form

$$
\operatorname{Res}_{Q^F}^{G^F}R_{L\subset P}^{G}(E)\cong\bigoplus_x\operatorname{Ind}_{K^F}^{Q^F}\left(\operatorname{Res}_{K^F}^{({}^xP)^F}{}^x\widetilde E\right).
$$

Here ${}^x\widetilde E$ is trivial on $({}^xU)^F$.

We next record the elementary normal-subgroup identity underlying [Harish-Chandra restriction](../../../../../harish-chandra-restriction.md). If $N\triangleleft D$ are finite groups, with $N$ a [normal subgroup](../../../../../normal-subgroup.md), and $C\subset D$, then for a complex $C$-module $A$,

$$
\left(\operatorname{Ind}_C^D A\right)^N\cong\operatorname{Ind}_{CN/N}^{D/N} A^{C\cap N}.
$$

To see this, replace invariants by coinvariants using the averaging idempotent $|N|^{-1}\sum_{n\in N}n$. Taking coinvariants in $\mathbb C[D]\otimes_{\mathbb C[C]}A$ first replaces $\mathbb C[D]$ by $\mathbb C[D/N]$, and forces $C\cap N$ to act trivially on $A$. Thus it yields $\mathbb C[D/N]\otimes_{\mathbb C[CN/N]}A_{C\cap N}$; averaging over $C\cap N$ identifies this last module with the one displayed. This also shows why characteristic zero makes the argument exact.

Apply this identity to $D=Q^F$, $N=V^F$, $C=K^F$. By the intersection lemmas, $CN/N=(M\cap{}^xP)^F$. Since ${}^x\widetilde E$ is trivial on $({}^xU)^F$, its $(K\cap V)^F$-invariants are exactly

$$
({}^xE)^{(V\cap{}^xL)^F}={}^*R_{H_x\subset Q\cap{}^xL}^{{}^xL}({}^xE).
$$

Moreover $(M\cap{}^xU)^F$ acts trivially on this module, so induction from $(M\cap{}^xP)^F$ to $M^F$ is precisely [Harish-Chandra induction](../../../../../harish-chandra-induction.md) from $H_x$. Substituting into each double-coset summand gives the boxed formula. This proves the formula for rational parabolics; it does not assume a general Mackey formula for nonrational [Deligne-Lusztig induction](../../../../../deligne-lusztig-induction.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
