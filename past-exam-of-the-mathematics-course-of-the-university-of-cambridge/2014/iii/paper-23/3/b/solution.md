<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Reduction modulo $p$ maps $\mathrm{SL}_2(\mathbb Z)$ onto $\mathrm{SL}_2(\mathbb F_p)$, of order $p(p^2-1)$. The image of $\Gamma_1(p)$ is the upper unipotent [subgroup](../../../../../../subgroup.md) of order $p$. Thus its index in $\mathrm{SL}_2$ is $p^2-1$, and, since $-I\notin\Gamma_1(p)$ for $p\ge5$, its effective index is

$$
d=\frac{p^2-1}{2}.
$$

Every element of $\Gamma_1(p)$ has [trace](../../../../../../matrix-trace.md) congruent to two. An effective elliptic element of order two or three has [trace](../../../../../../matrix-trace.md) zero or $\pm1$ in a lift, so neither is possible for $p\ge5$. Hence $r_2=r_3=0$.

Represent a [modular cusp](../../../../../../cusp-of-a-modular-group.md) by a primitive column $(a,c)$, modulo sign. Its reduction is a nonzero vector in $\mathbb F_p^2$ modulo sign, and the unipotent [subgroup](../../../../../../subgroup.md) acts by $(a,c)\mapsto(a+bc,c)$. For $c=0$, the nonzero values of $a$ give $(p-1)/2$ orbits. For $c\ne0$, $a$ varies freely and $c$ modulo sign gives another $(p-1)/2$ orbits. Thus there are $p-1$ [modular cusps](../../../../../../cusp-of-a-modular-group.md). The reduction classification is sufficient as well as necessary: completing two primitive columns to determinant-one [matrices](../../../../../../matrix.md) and adjusting the second columns by a translation makes congruent columns related by $\Gamma(p)$.

More explicitly, if a determinant-one [matrix](../../../../../../matrix.md) has first column $(a,c)$, conjugating $T^w$ gives

$$
\begin{pmatrix}1-acw&a^2w\\-c^2w&1+acw\end{pmatrix}.
$$

Its least allowable [cusp width](../../../../../../width-of-a-cusp.md) in $\Gamma_1(p)$ is one for $c\equiv0$ and $p$ otherwise. Both types therefore number $(p-1)/2$, with [cusp widths](../../../../../../width-of-a-cusp.md) one and $p$; their [cusp width](../../../../../../width-of-a-cusp.md) sum is $d$. There are no sign-twisted [modular cusp](../../../../../../cusp-of-a-modular-group.md) periods here, because [trace](../../../../../../matrix-trace.md) two cannot be congruent to minus two for these primes. Substitution gives

$$
\boxed{g(X(\Gamma_1(p)))=1+\frac{p^2-1}{24}-\frac{p-1}{2}=\frac{(p-5)(p-7)}{24}.}
$$

These are the [prime Gamma 1 cusp counts and widths](../../../../../../prime-gamma-1-cusp-counts-and-widths.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
