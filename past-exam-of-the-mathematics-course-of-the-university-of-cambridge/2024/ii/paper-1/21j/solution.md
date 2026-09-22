<h1 id="21j/solution">Solution</h1>

↑ **Parent:** [21J](../21j.md)

A [covering space](../../../../../covering-space.md) is a map $p:\widetilde X\to X$ such that every $x\in X$ has an open neighbourhood $U$ for which

$$
p^{-1}(U)=\coprod_{\alpha}U_\alpha
$$

and every restriction $p:U_\alpha\to U$ is a homeomorphism.

For path lifting, cover the compact image of $\gamma$ by evenly covered sets. The [Lebesgue number lemma](../../../../../lebesgue-number-lemma.md) supplies a subdivision

$$
0=t_0<t_1<\cdots<t_m=1
$$

for which each $\gamma([t_{j-1},t_j])$ lies in one such set. Starting in the sheet containing $\widetilde x_0$, lift the first segment with the inverse of that sheet. Its endpoint selects the sheet for the next segment, and induction constructs a continuous lift. Two lifts starting at the same point agree on the first segment because the relevant sheet map is injective, and the same argument at successive endpoints proves uniqueness.

Write $q:Y\to Y/\phi$ for the quotient map. The identity $p\circ Q=q\circ\operatorname{pr}_Y$ on $Y\times\mathbb Z$, where $Q$ is the quotient defining $\widetilde{Y/\phi}$, proves continuity of $p$ by the quotient property. Away from the two gluing regions, a small [open set](../../../../../open-set.md) lifts to one copy in every level. Near a glued point choose $U\Subset A$ and use the matched pair

$$
U\times\{i\}\ \cup\ \phi(U)\times\{i-1\}.
$$

After the prescribed identifications, each such pair maps homeomorphically to $q(U\cup\phi(U))$, and the pairs are disjoint for different $i$. Thus $p$ is a covering map.

Each copy of $Y$ is path-connected, and adjacent copies meet through the identified copies of the nonempty set $A$, so $\widetilde{Y/\phi}$ is path-connected. Translation

$$
\tau[(y,i)]=[(y,i+1)]
$$

is a deck transformation. Its powers act freely and transitively on every fibre, so the covering is regular. The [covering-space subgroup and deck-group quotient](../../../../../covering-space-subgroup-and-deck-group-quotient.md) then gives

$$
\boxed{G\trianglelefteq\pi_1(Y/\phi,[a_0]),
\qquad
\pi_1(Y/\phi,[a_0])/G\cong\langle\tau\rangle\cong\mathbb Z.}
$$

## ↑ Ancestors (10)

1. [21J](../21j.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
