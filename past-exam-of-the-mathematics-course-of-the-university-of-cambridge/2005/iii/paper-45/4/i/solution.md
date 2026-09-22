<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $A\in\{0,1\}$ and $B\in\{0,1\}$ encode the [alleles](../../../../../../allele.md) at two loci on a randomly chosen population [haplotype](../../../../../../haplotype.md). Write $p_{ab}=P(A=a,B=b)$, $p_A=p_{10}+p_{11}$ and $p_B=p_{01}+p_{11}$. The [linkage disequilibrium](../../../../../../linkage-disequilibrium.md) coefficient is

$$
\boxed{D=p_{11}-p_Ap_B=p_{11}p_{00}-p_{10}p_{01}.}
$$

The determinant identity follows by substituting the marginal frequencies and $\sum p_{ab}=1$. All four [haplotype](../../../../../../haplotype.md) frequencies can be recovered as

$$
\begin{aligned}
p_{11}&=p_Ap_B+D,&p_{10}&=p_A(1-p_B)-D,\\
p_{01}&=(1-p_A)p_B-D,&p_{00}&=(1-p_A)(1-p_B)+D.
\end{aligned}
$$

Thus $D=0$ is precisely [independence](../../../../../../independent-random-variables.md) of the two allelic states. Its sign depends on which [alleles](../../../../../../allele.md) are labeled one, and its possible magnitude depends on the marginal frequencies.

One other measure is squared [allelic correlation](../../../../../../allelic-correlation.md). For segregating loci, $0<p_A,p_B<1$, their indicator-variable [covariance](../../../../../../covariance.md) is $D$, and their [variances](../../../../../../variance-split.md) are $p_A(1-p_A)$ and $p_B(1-p_B)$. Hence

$$
\boxed{r^2=\frac{D^2}{p_A(1-p_A)p_B(1-p_B)},\qquad 0\le r^2\le1.}
$$

This is the squared [correlation](../../../../../../pearson-correlation-coefficient.md), useful for measuring how well one marker predicts the other in [association mapping](../../../../../../association-mapping.md). It is undefined if a locus is monomorphic. [Linkage disequilibrium](../../../../../../linkage-disequilibrium.md) describes population [haplotype](../../../../../../haplotype.md) frequencies; [genetic linkage](../../../../../../genetic-linkage.md) describes transmission within [meioses](../../../../../../meiosis.md). Physically linked loci can have $D=0$, and population mixing can produce LD even between unlinked loci.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
