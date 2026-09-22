<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $a=(123)$ and $t=(12)$. Conjugation by $a$ fixes the three given idempotents of $k\langle a\rangle$, while $tat^{-1}=a^{-1}$ fixes $e_1$ and interchanges $e_2,e_3$. Their orbits are therefore $\boxed{\{e_1\},\{e_2,e_3\}}$, with central orbit sums

$$
b_0=e_1=1+a+a^2,\qquad b_1=e_2+e_3=a+a^2,
$$

using $\omega+\omega^2=1$ in characteristic $2$.

To ensure these sums really are primitive central idempotents, examine the two ideals. The first has basis $b_0,b_0t$, with $b_0a=b_0$, so $b_0kG\cong kC_2$, a [local ring](../../../../../../local-ring.md). The second has dimension $4$: $b_1k\langle a\rangle=ke_2\oplus ke_3$ has dimension $2$, and the two cosets of $\langle a\rangle$ double it. In the two-dimensional representation

$$
a\longmapsto\begin{pmatrix}\omega&0\\0&\omega^2\end{pmatrix},\qquad t\longmapsto\begin{pmatrix}0&1\\1&0\end{pmatrix},
$$

These matrices satisfy $a^3=t^2=1$ and $tat^{-1}=a^{-1}$, so they define a representation of $S_3$. In it, $b_1$ acts as identity and $b_0$ as zero. The distinct diagonal entries supply the two diagonal matrix units, and multiplying by the swap matrix supplies the off-diagonal units. The induced map $b_1kG\to M_2(k)$ is thus surjective and, by dimension, an isomorphism. Both summands have no nontrivial central idempotents, so $b_0,b_1$ are exactly the [2-modular blocks of S3](../../../../../../2-modular-blocks-of-s3.md).

The [Brauer morphism](../../../../../../brauer-morphism.md) at the trivial subgroup is the identity. For $H=\langle t\rangle$, $C_G(H)=H$, and neither $a$ nor $a^2$ lies in this centralizer. Thus

$$
\boxed{\begin{array}{c|c|c|c}
\text{block}&\operatorname{Br}_1^G&\operatorname{Br}_H^G&\text{defect group}\\\hline
b_0=1+a+a^2&b_0&1&H\\
b_1=a+a^2&b_1&0&1
\end{array}}.
$$

Indeed $H$ is Sylow, and all nontrivial $2$-subgroups are conjugate to it; these images therefore determine maximality in the definition of a [defect group of a block](../../../../../../defect-group-of-a-block.md). The original PDF provides the $S_3,\mathbb F_4,N,H$ setup missing from the TeX transcription.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 138](../../../paper-138-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
