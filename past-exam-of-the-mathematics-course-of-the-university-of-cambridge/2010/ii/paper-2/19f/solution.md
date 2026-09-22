<h1 id="19f/solution">Solution</h1>

↑ **Parent:** [19F](../19f.md)

If a [group representation](../../../../../group-representation.md) of $G$ has [character](../../../../../character-of-a-representation.md) $\chi$, its [restriction of a representation](../../../../../restriction-of-a-representation.md) to $H$ has character $\chi|_H$. For an $H$-representation $V$ with character $\psi$, the [induced representation](../../../../../induced-representation.md) is $\mathbb C[G]\otimes_{\mathbb C[H]}V$, with $G$ acting on the first factor. Decomposing into coset copies of $V$ shows that its [character](../../../../../character-of-a-representation.md) is

$$
(\operatorname{Ind}_H^G\psi)(g)=\frac1{|H|}\sum_{\substack{x\in G\\x^{-1}gx\in H}}\psi(x^{-1}gx).
$$

Indeed only cosets fixed by $g$ contribute to the [trace](../../../../../matrix-trace.md), and each coset has $|H|$ representatives.

The [Frobenius reciprocity](../../../../../frobenius-reciprocity.md) says $\langle\operatorname{Ind}_H^G\psi,\chi\rangle_G=\langle\psi,\operatorname{Res}_H^G\chi\rangle_H$. Directly, with the usual [character inner product](../../../../../character-inner-product.md),

$$
\begin{aligned}
\langle\operatorname{Ind}\psi,\chi\rangle_G
&=\frac1{|G||H|}\sum_{x\in G}\sum_{h\in H}\psi(h)\overline{\chi(xhx^{-1})}\\
&=\frac1{|H|}\sum_{h\in H}\psi(h)\overline{\chi(h)}.
\end{aligned}
$$

The first equality substitutes $g=xhx^{-1}$ in the finite sum, and the second uses conjugacy invariance. This proves the theorem.

## ↑ Ancestors (10)

1. [19F](../19f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
