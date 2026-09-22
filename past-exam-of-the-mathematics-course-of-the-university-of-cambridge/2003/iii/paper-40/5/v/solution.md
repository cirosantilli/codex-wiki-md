<h1 id="5/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Using cases as disease [haplotypes](../../../../../../haplotype.md) and controls as control [haplotypes](../../../../../../haplotype.md) in the model requested here, the chromosome counts estimate

$$
P(A\mid d)=20/200=0.10,\quad P(a\mid d)=0.90,\quad P(A\mid D)=120/200=0.60,\quad P(a\mid D)=0.40.
$$

These are conditional marker [allele](../../../../../../allele.md) frequencies, not the reverse [conditional probabilities](../../../../../../conditional-probability.md) $P(d\mid A)$. Under independent founder [chromosomes](../../../../../../chromosome.md), conditional on the father's $Dd,Aa$ [genotype](../../../../../../genotype.md), the phase $AD/ad$ has weight proportional to $0.60\cdot0.90=0.54$, and $Ad/aD$ has weight proportional to $0.10\cdot0.40=0.04$. Their normalized weights are $27/29$ and $2/29$. This conditions on the model's observed parental genotypes; the omitted disease-allele frequencies cancel in the phase-weight ratio.

Using the two phase-specific [pedigree likelihoods](../../../../../../pedigree-likelihood.md) already derived,

$$
\begin{aligned}
L_{\rm LD}(\theta)&=\frac{0.54L_1(\theta)+0.04L_2(\theta)}{0.58}\\
&=\frac{\theta(1-\theta)}{8(0.58)}\{0.54(1-\theta)+0.04\theta\}\\
&=\frac{\theta(1-\theta)(0.54-0.50\theta)}{4.64}.
\end{aligned}
$$

The normalizing factor is independent of $\theta$, so maximize $g(\theta)=0.54\theta-1.04\theta^2+0.50\theta^3$. Its derivative gives exactly

$$
\boxed{1.5\widehat\theta^2-2.08\widehat\theta+0.54=0.}
$$

Only the smaller root lies in $[0,1/2]$:

$$
\boxed{\widehat\theta=\frac{2.08-\sqrt{2.08^2-4(1.5)(0.54)}}3\simeq0.34590.}
$$

On this interval $g''(\theta)=-2.08+3\theta<0$, so this stationary point is the unique maximum. The maximum [LOD score](../../../../../../lod-score.md), retaining the same [linkage disequilibrium](../../../../../../linkage-disequilibrium.md) frequencies in numerator and denominator, is

$$
\boxed{Z_{\max}=\log_{10}\frac{\widehat\theta(1-\widehat\theta)(0.54-0.50\widehat\theta)}{(1/2)(1/2)(0.54-0.25)}\simeq0.05898.}
$$

This is only a [likelihood ratio](../../../../../../likelihood-ratio.md) of about $1.145$ against $\theta=1/2$, hence very weak evidence. The population frequencies are treated as fixed plug-in estimates, as requested; uncertainty in those estimates and possible disease-model differences between controls and normal-allele chromosomes would matter in a fuller analysis.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [5](../../5.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
