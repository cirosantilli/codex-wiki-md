<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $1<s\leq\sqrt2$, use [centered tent-map period-doubling renormalization](../../../../../../centered-tent-map-period-doubling-renormalization.md). Let

$$
c=s-1,\qquad J_s=[-c,c],\qquad h_s(y)=-cy.
$$

The image $T_s(J_s)=[1+s-s^2,1]$ lies to the right of $J_s$, with disjoint interiors, because $1+s-s^2\geq s-1$. It lies in the positive branch. Consequently,

$$
T_s^2(x)=1-s+s^2|x|=-c+s^2|x|\quad(x\in J_s),
$$

and its range $[-c,(s^2-1)c]$ is contained in $J_s$. The orientation-reversing [affine map](../../../../../../affine-map.md) $h_s$ gives the exact [topological conjugacy](../../../../../../topological-conjugacy.md)

$$
\boxed{h_s^{-1}\circ T_s^2\circ h_s(y)=1-s^2|y|=T_{s^2}(y).}
$$

Thus renormalization squares the slope and halves the return period. Since $s>1$, there is a least $n\geq0$ for which $s^{2^n}>\sqrt2$. Minimality implies $s^{2^n}\leq2$, and all previous slopes are in the renormalizable range. Successive [affine maps](../../../../../../affine-map.md) therefore conjugate the restriction of $T_s^{2^n}$ on a nested central interval to $T_{s^{2^n}}$.

By the preceding part, an iterate $T_{s^{2^n}}^m$ has a [horseshoe for an interval map](../../../../../../horseshoe-for-an-interval-map.md). Pull its two branch intervals and its range interval back through the composed conjugacy. They give a horseshoe for $T_s^{2^n m}$. Therefore

$$
\boxed{T_s\text{ has an iterate with a horseshoe for every }1<s\leq2.}
$$

At the endpoint $s=\sqrt2$, one renormalization gives the full slope-two tent map, so the argument includes that endpoint without assuming the strict inequality from part (a).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
