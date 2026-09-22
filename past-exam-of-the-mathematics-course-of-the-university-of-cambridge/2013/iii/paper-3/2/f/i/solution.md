<h1 id="2/f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the field $F=\mathbb F_2[\zeta]/(\zeta^3+\zeta+1)$. The defining polynomial has no root in $\mathbb F_2$, hence is irreducible. Label its elements by

$$
1\leftrightarrow0,\quad2\leftrightarrow1,\quad3\leftrightarrow\zeta,\quad
5\leftrightarrow\zeta^2,\quad4\leftrightarrow\zeta^3,\quad
7\leftrightarrow\zeta^4,\quad8\leftrightarrow\zeta^5,\quad6\leftrightarrow\zeta^6.
$$

Since $F^*$ has prime order seven, $\zeta$ has order seven. Multiplication by $\zeta$ is exactly $b$. The identities $\zeta^3=\zeta+1$, $\zeta^6=\zeta^2+1$ and $\zeta^5=\zeta^4+1$ show that translation by one is exactly $a$.

Conjugating $a$ by powers of $b$ gives the translations $T_{\zeta^i}:z\mapsto z+\zeta^i$. The translations by $1,\zeta,\zeta^2$ generate all eight translations. Consequently

$$
\boxed{G=\{z\mapsto sz+t:s\in F^*,\ t\in F\}\cong\operatorname{AGL}_1(8),\qquad |G|=56.}
$$

For distinct $u,v$ and distinct target points $u',v'$, the unique affine map has $s=(v'-u')/(v-u)$ and $t=u'-su$. Thus the action is sharply two-transitive.

Its regular [characteristic subgroup](../../../../../../../characteristic-subgroup.md) is

$$
\boxed{K=\{T_t:t\in F\}\cong C_2^3
=\langle a,bab^{-1},b^2ab^{-2}\rangle.}
$$

Translations act regularly, $K$ is normal, and its order eight makes it the unique Sylow two-subgroup, hence characteristic. This identifies the abstract subgroup and explicit generators in the original permutation notation.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [F](../../f.md)
3. [2](../../../2.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
