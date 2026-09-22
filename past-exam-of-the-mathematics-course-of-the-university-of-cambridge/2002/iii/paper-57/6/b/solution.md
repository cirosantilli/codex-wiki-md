<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the conventional additive pedigree relatedness $r_{UV}=2\phi_{UV}$, where $\phi_{UV}$ is the [kinship coefficient](../../../../../../kinship-coefficient.md), the [probability](../../../../../../probability.md) that randomly selected gene copies from $U$ and $V$ are [identical by descent](../../../../../../identity-by-descent.md). For noninbred individuals this convention gives ordinary [full siblings](../../../../../../full-sibling.md) relatedness $1/2$, as required. It is important that this is not the [probability](../../../../../../probability.md) of sharing at least one copy: that [probability](../../../../../../probability.md) is $3/4$ for ordinary [full siblings](../../../../../../full-sibling.md).

Let the parents be $M,F$. They are otherwise outbred [first cousins](../../../../../../first-cousin.md), so $\phi_{MF}=1/16$ and $\phi_{MM}=\phi_{FF}=1/2$. For two children $C,D$, independent [Mendelian segregation](../../../../../../mendelian-segregation.md) gives

$$
\phi_{CD}=\frac14(\phi_{MM}+\phi_{MF}+\phi_{FM}+\phi_{FF})=\frac9{32}.
$$

Therefore the autosomal additive relatedness is

$$
\boxed{r_{CD}=9/16.}
$$

The additional $1/16$ beyond $1/2$ comes from maternal-paternal cross-origin matches. Each child has [inbreeding coefficient](../../../../../../inbreeding-coefficient.md) $1/16$. The additive coefficient is a sum of descent [probabilities](../../../../../../probability.md) rather than a literal bounded [probability](../../../../../../probability.md) in all inbred pedigrees; a relationship normalized to self-relatedness would be $r_{CD}/(1+F)=9/17$. Likewise, [identity-by-descent sharing of inbred full siblings](../../../../../../identity-by-descent-sharing-of-inbred-full-siblings.md) gives a different matched-copy statistic. The exam's calibration to $1/2$ supports the additive convention, but the quoted [probability](../../../../../../probability.md) wording needs this qualification.

For sex chromosomes the route of cousinship matters, not merely the fact that the parents have opposite sex. Let $P_M$ be the mother-cousin's parent in the shared sibling pair, and $P_F$ the father-cousin's parent in that pair. Let $F_X$ be the [probability](../../../../../../probability.md) that the mother's randomly transmitted X matches the father's single X by descent. With no founder inbreeding, the possibilities are

$$
\begin{array}{c|c|c}
P_M& P_F&F_X\\\hline
\text{male}&\text{male}&0\\
\text{female}&\text{male}&0\\
\text{male}&\text{female}&1/8\\
\text{female}&\text{female}&3/16
\end{array}
$$

In the first two rows the father-cousin is related through his father, whose X he does not inherit. In the third row his mother is a sister of the mother-cousin's father: the relevant brother and sister match their maternal X copies with [probability](../../../../../../probability.md) $1/4$, and the mother-cousin transmits her paternal X with [probability](../../../../../../probability.md) $1/2$, giving $1/8$. In the last row the two sisters' random X gametes match with [probability](../../../../../../probability.md) $3/8$: their common father's X contributes $1/4$, and their common mother's two X copies contribute $1/8$. Transmission by the mother-cousin halves this to $3/16$. This derives the [sex-linked cousin kinship](../../../../../../sex-linked-cousin-kinship.md) values.

For an unweighted comparison by chromosome pair, two daughters have sex-pair additive relatedness $3/4+F_X$: their paternal X always matches, maternal X matches with [probability](../../../../../../probability.md) $1/2$, and the two cross-origin terms each contribute $F_X$. Two sons have [mean](../../../../../../expected-value.md) sex-pair relatedness $3/4$, from an X match of [probability](../../../../../../probability.md) $1/2$ and a common paternal Y with [probability](../../../../../../probability.md) one. A daughter-son pair has sex-pair value $1/4+F_X/2$, with the Y contribution zero. These calculations treat chromosomes as unrecombined blocks and weight X and Y equally; chromosome-length-weighted or locus-specific coefficients are different.

For two children with independent equally likely sexes, these three cases have weights $1/4,1/4,1/2$. Their [mean](../../../../../../expected-value.md) sex-pair relatedness is $1/2+F_X/2$, so averaging the 22 autosomal pairs and the sex pair gives

$$
\boxed{\overline r_{\rm genome}=\frac{22(9/16)+1/2+F_X/2}{23}.}
$$

If the cousins' route has $F_X=0$, this is $103/184$, slightly below $9/16$. If, as an additional sampling assumption, the four parent-sex routes in the table are equally likely, $\mathbb E F_X=5/64$ and the answer is $1653/2944$. These are different legitimate numerical corrections under different specified pedigrees. **There is no unique sex-chromosome correction from opposite-sex cousinhood alone.** The table and formula give it once the missing pedigree and offspring-sex information is supplied.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
