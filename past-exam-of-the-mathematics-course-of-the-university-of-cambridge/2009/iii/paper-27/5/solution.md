<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For cusps $\alpha,\beta\in\mathbb P^1(\mathbb Q)$, the [modular symbol](../../../../../modular-symbol.md) $\{\alpha,\beta\}$ is the oriented path class in $H_1(X(\Gamma),C;\mathbb Z)$, where $C$ is the finite cusp set. Reversing paths changes the sign, concatenating paths gives $\{\alpha,\beta\}+\{\beta,\gamma\}=\{\alpha,\gamma\}$, and the group identifies translated paths. A [continued fraction](../../../../../continued-fraction.md) expansion subdivides any rational-endpoint path into determinant-one edges. Representatives of the finitely many cosets therefore supply [Manin symbols](../../../../../manin-symbol.md) $[g]=\{g0,g\infty\}$. With inversion $S$ and translation $T$, reversing an edge and taking the boundary of an ideal triangle give

$$
[g]+[gS]=0,\qquad[g]+[gST]+[g(ST)^2]=0.
$$

These relations give a finite rational linear algebra presentation. Integral computation additionally removes the elliptic torsion in this naive presentation; the actual relative homology group of the compact surface is torsion-free.

The boundary of $\{\alpha,\beta\}$ is $[\beta]-[\alpha]$ in $H_0(C)$. Its kernel is $H_1(X;\mathbb Q)$ by the [long exact sequence of a pair](../../../../../long-exact-sequence-in-relative-homology.md). A [Hecke operator](../../../../../hecke-operator.md) acts by summing the images of each path under its finite determinant-$n$ correspondence. Rational endpoints are again rational, so [continued fractions](../../../../../continued-fraction.md) reduce each image back to Manin symbols. Finite row reduction produces rational matrices for the relative symbols and for the boundary kernel. Integration of a weight-two [cusp form](../../../../../cusp-form.md) against these absolute cycles is compatible with the Hecke action. The resulting decomposition

$$
H_1(X;\mathbb C)\simeq S_2(\Gamma)^*\oplus\overline{S_2(\Gamma)}^{\,*}
$$

explains the relation between these matrices and cusp forms. Strictly, a rational matrix on absolute homology is not automatically a rational matrix on the holomorphic summand in an arbitrary complex basis. For subgroups preserved by real conjugation, the conjugation eigenspaces provide rational models of the cusp-form representation. More generally one should specify a compatible rational model or use the doubled homological representation. This distinction matters in interpreting the essay's rationality claim for an arbitrary subgroup; the algorithm on homology is always rational.

For the supplied subgroup, use $P=(1\,7\,3\,6)(2\,5\,4)$ for translation and $Q=(1\,7)(2\,6)(3\,4)$ for inversion, following the PDF's naming. Translation has two cycles, so there are two cusps of widths four and three. Inversion fixes just coset five, giving one elliptic orbit of order two. The order-three product acts with cycles $(1)(2\,5\,3)(4\,6\,7)$ in one of the two equivalent composition conventions, giving one elliptic orbit of order three. Since $Q^2=1$, the central $-I$ acts trivially and the effective index is seven. The [genus formula for a modular curve](../../../../../genus-formula-for-a-modular-curve.md) gives

$$
g=1+\frac7{12}-\frac14-\frac13-\frac22=0.
$$

The [long exact sequence of a pair](../../../../../long-exact-sequence-in-relative-homology.md) now gives

$$
\boxed{\operatorname{rank}H_1(X(\Gamma),C;\mathbb Z)=2g+|C|-1=1.}
$$

One can see this directly from the symbols. Over $\mathbb Q$, $Q$ gives $m_7=-m_1$, $m_6=-m_2$, $m_4=-m_3$ and $m_5=0$. The fixed order-three coset gives $m_1=0$, and the other triangle relations give $m_3=-m_2$. Thus $(m_1,\ldots,m_7)=(0,t,-t,t,0,-t,0)$. After removing elliptic torsion the integral group is free of rank one, agreeing with the surface calculation. Since $g=0$, the absolute boundary kernel and $S_2(\Gamma)$ both vanish: the cusp-form Hecke matrices for this particular example are the empty $0\times0$ matrices.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
