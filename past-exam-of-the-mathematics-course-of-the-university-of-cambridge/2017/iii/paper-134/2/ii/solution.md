<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Part (i) first shows that $D-C$ is effective. Also $C^2<0$: writing $D=aC+E$ with $a\ge1$ and $E$ effective without $C$ as a component gives $D\cdot C=aC^2+E\cdot C$, where $E\cdot C\ge0$.

For $0\le j<m$,

$$
(mD-jC)\cdot C=m(D-C)\cdot C+(m-j)C^2<0.
$$

Every effective member of $|mD|$ therefore contains $C$; after subtracting it, the same reasoning applies again, until $m$ copies have been subtracted. Conversely adding $mC$ to an effective member of $|m(D-C)|$ is allowed. Hence

$$
\boxed{|mD|=|m(D-C)|+mC\qquad(m\ge0).}
$$

For $m=0$ this is just the identity system $|0|$. The extra intersection hypothesis is needed: on the [Hirzebruch surface](../../../../../../hirzebruch-surface.md) $\mathbb F_2$, with negative section $S$ and fibre $F$, take $D=S+F$. Then $D\cdot S=-1$ but $(D-S)\cdot S=1$. Here $h^0(2D)=4$ while $h^0(2F)=3$, so removing $2S$ loses a section.

For the point [blowup of a smooth algebraic surface](../../../../../../blowup-of-a-smooth-algebraic-surface.md) $\psi:\widetilde X\to X$ with exceptional curve $E$, the [canonical divisor formula for a surface blowup](../../../../../../canonical-divisor-formula-for-a-surface-blowup.md) and the [intersection formula for blowing up a surface](../../../../../../intersection-formula-for-blowing-up-a-surface.md) give

$$
K_{\widetilde X}=\psi^*K_X+E,\qquad E^2=-1,\qquad\psi^*K_X\cdot E=0.
$$

One must not assume $K_{\widetilde X}$ itself is effective. Instead, if an effective member of $|mK_{\widetilde X}|$ exists, then for each $0\le j<m$ its class after removing $jE$ has intersection $-m+j<0$ with $E$. The same fixed-component argument removes exactly the required $mE$, giving

$$
H^0(\widetilde X,\mathcal O(m\psi^*K_X))\xrightarrow{\ \cdot s_E^m\ }H^0(\widetilde X,\mathcal O(mK_{\widetilde X}))
$$

as an isomorphism, also when both sides are zero. Since $X$ is normal and $\psi$ is proper and birational, $\psi_*\mathcal O_{\widetilde X}=\mathcal O_X$. The [projection formula for sheaves](../../../../../../projection-formula.md) therefore identifies the space on the left with $H^0(X,\mathcal O_X(mK_X))$. Consequently

$$
\boxed{H^0(\widetilde X,mK_{\widetilde X})\cong H^0(X,mK_X)\quad(m\ge0).}
$$

The PDF writes equality of spaces; this is the canonical identification just described, rather than literal equality of spaces on different schemes. This proves [blowup invariance of plurigenera](../../../../../../blowup-invariance-of-plurigenera.md) in arbitrary characteristic.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 134](../../../paper-134-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
