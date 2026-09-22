<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For pairwise comaximal [ideals](../../../../../../ideal.md) $I_1,\ldots,I_r$ of $R$, reduction gives the [Chinese remainder theorem for ideals](../../../../../../chinese-remainder-theorem-for-ideals.md):

$$
\boxed{R/(I_1\cdots I_r)\cong\prod_{i=1}^rR/I_i.}
$$

Its kernel is $\bigcap_iI_i$. For two comaximal [ideals](../../../../../../ideal.md), write $1=u+v$ with $u\in I$, $v\in J$. If $x\in I\cap J$, then $x=xu+xv\in IJ$, showing $I\cap J=IJ$. Induction gives the product formula: a product of [ideals](../../../../../../ideal.md) individually comaximal with $J$ is still comaximal with $J$, by multiplying identities modulo $J$.

Put $J_i=\prod_{j\ne i}I_j$. Since $I_i+J_i=R$, choose $e_i\in J_i$ with $e_i\equiv1\pmod{I_i}$. The element $\sum_i a_ie_i$ has any prescribed residues $a_i\pmod{I_i}$, proving surjectivity. Its residue class modulo the product is unique because we already identified the kernel. In a [Dedekind domain](../../../../../../dedekind-domain.md), powers of distinct nonzero [prime ideals](../../../../../../prime-ideal.md) are pairwise comaximal, giving the prime-power form. The theorem requires comaximality; it is not a statement about arbitrary lists of [ideals](../../../../../../ideal.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
