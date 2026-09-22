<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Put $\Gamma=\pi_1(X,x)$ and $R=\mathbb Z[\Gamma]$. Give $\mathbb Z$ its trivial left $R$-[module](../../../../../module-mathematics.md) structure, through the augmentation $\varepsilon:R\to\mathbb Z$, $\sum n_g g\mapsto\sum n_g$. The [universal cover](../../../../../universal-cover.md) $\widetilde X$ has the lifted cell structure, with $\Gamma$ acting by [deck transformations](../../../../../deck-transformation.md).

For each cell of $X$, choose one lifted cell and orient every translate compatibly with its projection. The translates form one copy of the regular $R$-[module](../../../../../module-mathematics.md). Thus

$$
C_k(\widetilde X)\cong\bigoplus_{\text{$k$-cells of }X}R
$$

is a free left $R$-[module](../../../../../module-mathematics.md), and its boundary is $R$-linear. The augmentation $C_0(\widetilde X)\to\mathbb Z$ sends every vertex to one. The contractibility of $\widetilde X$ says that its reduced [homology](../../../../../homology-split.md) vanishes, so the augmented complex

$$
\cdots\longrightarrow C_2(\widetilde X)
\longrightarrow C_1(\widetilde X)
\longrightarrow C_0(\widetilde X)
\longrightarrow\mathbb Z\longrightarrow0
$$

is exact. It is therefore a [free resolution](../../../../../free-resolution.md) of the trivial [module](../../../../../module-mathematics.md). By the definition of the [Ext functor](../../../../../ext-functor.md),

$$
\operatorname{Ext}_R^i(\mathbb Z,\mathbb Z)
=H^i\!\left(\operatorname{Hom}_R(C_*(\widetilde X),\mathbb Z)\right).
$$

An $R$-linear cochain with values in the trivial [module](../../../../../module-mathematics.md) has the same value on every translate of a lifted cell. It is therefore exactly an ordinary integral cellular cochain on $X$. The correspondence does not depend on which lift was initially chosen. It also respects the coboundary: applying a constant-on-orbits cochain to the lifted cellular boundary sums precisely the incidence coefficients of the boundary in the base. Hence

$$
\operatorname{Hom}_R(C_*(\widetilde X),\mathbb Z)
\cong C_{\mathrm{cell}}^*(X;\mathbb Z)
$$

as [cochain complexes](../../../../../cochain-complex.md), not just as graded groups. Cellular [cohomology](../../../../../cohomology-split.md) computes the [cohomology](../../../../../cohomology-split.md) of a cell complex, giving

$$
\boxed{H^i(X;\mathbb Z)\cong\operatorname{Ext}_R^i(\mathbb Z,\mathbb Z)
\quad\text{for all }i\geq0.}
$$

At $i=0$ both sides are $\mathbb Z$, by connectedness and $\operatorname{Hom}_R(\mathbb Z,\mathbb Z)=\mathbb Z$. This is the [cellular free resolution from a contractible universal cover](../../../../../cellular-free-resolution-from-a-contractible-universal-cover.md) description of [group cohomology](../../../../../group-cohomology.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
