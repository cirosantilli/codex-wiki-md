<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

First show $C_N(h)=\{1\}$. If $z\in N$ commutes with $h$ and $z\ne1$, then $z\notin H$ because $N\cap H=\{1\}$. But $z^{-1}hz=h$, so the nonidentity element $h$ lies in $H\cap H^z$, contradicting the [Frobenius complement](../../../../../../frobenius-complement.md) property. Thus conjugation by $h$ has no nonidentity fixed element in the [Frobenius kernel](../../../../../../frobenius-kernel.md).

Normality of $N$ makes

$$
f_h:N\longrightarrow N,\qquad f_h(y)=h^{-1}y^{-1}hy
$$

well-defined. If $f_h(a)=f_h(b)$, cancellation gives $a^{-1}ha=b^{-1}hb$, and hence $ba^{-1}$ commutes with $h$. Since $ba^{-1}\in N$ and $C_N(h)=\{1\}$, we obtain $a=b$. The map is injective, and an injection of a finite set into itself is surjective. Consequently

$$
\boxed{\text{For every }x\in N\text{ there exists a unique }y\in N\text{ with }[h,y]=x.}
$$

This is the [commutator bijection from a fixed-point-free automorphism](../../../../../../commutator-bijection-from-a-fixed-point-free-automorphism.md), applied to $\alpha(y)=h^{-1}yh$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
