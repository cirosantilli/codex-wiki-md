<h1 id="18h/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A primitive sixth root of unity satisfies

$$
\boxed{\Phi_6(x)=x^2-x+1,}
$$

which is irreducible over $\mathbb Q$ because its discriminant is $-3$. For the other polynomial choose $\alpha=i\,3^{1/6}$, so $\alpha^6=-3$ and $\alpha^3=-i\sqrt3$. Then $\zeta_6=(1-\alpha^3)/2\in\mathbb Q(\alpha)$, so this field already contains all six roots. The [Eisenstein criterion](../../../../../../eisenstein-criterion.md) at $3$ proves $x^6+3$ irreducible, giving a [splitting field](../../../../../../splitting-field.md) of degree six.

Put $r(\alpha)=\zeta_6^2\alpha$ and $s(\alpha)=\zeta_6\alpha$. The first automorphism fixes $\zeta_6$ and has order three. The second sends $\alpha^3$ to its negative, so sends $\zeta_6$ to $\zeta_6^{-1}$; hence $s^2=1$ and $srs=r^{-1}$. These six distinct transformations exhaust the [Galois group](../../../../../../galois-group.md). Therefore

$$
\boxed{\operatorname{Gal}(x^6+3/\mathbb Q)\cong S_3.}
$$

The presence of sixth roots of unity inside the [splitting field](../../../../../../splitting-field.md) is why this particular binomial has degree six rather than a generic twelve-degree [splitting field](../../../../../../splitting-field.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [18H](../../18h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
