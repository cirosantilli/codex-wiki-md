<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $a$ denote the disease [allele](../../../../../../allele.md). Complete [penetrance](../../../../../../penetrance.md) with [recessive inheritance](../../../../../../recessive-inheritance.md) makes each affected child $aa$. The unaffected parents must therefore both be $Aa$ [genetic carriers](../../../../../../genetic-carrier.md). Condition on these parental [genotypes](../../../../../../genotype.md) and the fully informative marker; the distinct paternal and maternal marker copies identify which parent's copies are shared. Average over the two equally likely marker-disease [haplotype](../../../../../../haplotype.md) phases in each parent. This is the phase-symmetric model implicit in the requested [pedigree likelihood](../../../../../../pedigree-likelihood.md) identities.

For one parent, suppose first that both children receive the same marker copy. If that marker copy is on the parental [chromosome](../../../../../../chromosome.md) carrying $a$, both children receive $a$ with [probability](../../../../../../probability.md) $(1-\theta)^2$; in the opposite phase the [probability](../../../../../../probability.md) is $\theta^2$. The phase-averaged [probability](../../../../../../probability.md) is

$$
v=\frac{(1-\theta)^2+\theta^2}{2}=\frac12-\theta(1-\theta).
$$

If the children receive different marker copies, one disease-[allele](../../../../../../allele.md) transmission is recombinant and the other is nonrecombinant in either phase. The [probability](../../../../../../probability.md) that both receive $a$ is therefore

$$
u=\theta(1-\theta).
$$

Paternal and maternal transmissions are independent. Sharing zero marker copies means the different-copy case for both parents; sharing two means the same-copy case for both; sharing one means one of each. Thus the [recessive affected-sib-pair likelihood](../../../../../../recessive-affected-sib-pair-likelihood.md) is

$$
\boxed{\begin{aligned}
L_0&=\theta^2(1-\theta)^2=u^2,\\
L_1&=\frac{\theta(1-\theta)}2\bigl[(1-\theta)^2+\theta^2\bigr]=uv,\\
L_2&=\frac14\bigl[(1-\theta)^2+\theta^2\bigr]^2=v^2.
\end{aligned}}
$$

Here $L_j$ is the [probability](../../../../../../probability.md) that both children are affected conditional on the marker sharing state $J=j$, not the [probability](../../../../../../probability.md) of $J=j$ conditional on their being affected. Since $u,v\ge0$,

$$
\boxed{\sqrt{L_0L_2}=uv=L_1,\qquad \sqrt{L_0}+\sqrt{L_2}=u+v=\frac12.}
$$

At $\theta=1/2$, all three conditional disease [probabilities](../../../../../../probability.md) equal $1/16$, as expected from two independent children of an $Aa\times Aa$ mating. At $\theta=0$, only the two-copy-sharing state can produce two affected children. Phase weights other than $1/2$ would require a different [likelihood function](../../../../../../likelihood-function.md) and need not obey these identities.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
