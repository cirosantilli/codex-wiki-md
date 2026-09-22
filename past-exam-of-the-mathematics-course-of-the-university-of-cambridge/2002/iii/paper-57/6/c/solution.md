<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume a closed population with even size $N$, unrelated founders, monogamous mating, nonoverlapping generations and exactly two offspring per couple. Sex labels are exchangeable for the autosomal calculation, with enough individuals of each sex to form the stipulated pairs. A randomly chosen distinct offspring pair are siblings with [probability](../../../../../../probability.md) $1/(N-1)$: among the $\binom N2$ pairs, exactly $N/2$ are within-family pairs. This fixed-family-size fact, rather than independent sampling of all parents, determines the recurrence.

First give the elementary chromosome-sharing idealization consistent with taking self-relatedness as one and ordinary sibling relatedness as $1/2$. In this model each individual carries one ancestral label, passed through one randomly chosen parent. Let $r_G$ be [mean](../../../../../../expected-value.md) sharing between distinct individuals, and let $m_G$ be the [mean](../../../../../../expected-value.md) sharing between mates. Siblings share their parental label with [probability](../../../../../../probability.md) $(1+m_G)/2$. The average relatedness between parents from different couples is

$$
u_{G+1}=\frac{(N-1)r_G-m_G}{N-2}.
$$

To see the latter count, the ordered pairs from different couples are all ordered distinct pairs minus the $N$ ordered mating pairs. Each pair of parents from different couples contributes equally to the four possible cross-family offspring relationships. Combining sibling and nonsibling offspring gives

$$
\boxed{r_{G+1}=r_G+\frac{1-m_G}{2(N-1)}.}
$$

With random mating, $m_G=r_G$ in expectation, so $r_0=0$ gives

$$
\boxed{r_G=1-\left(1-\frac1{2(N-1)}\right)^G.}
$$

The [mean](../../../../../../expected-value.md) sharing tends to one, on a generation scale of order $2(N-1)$. It is not linear indefinitely: repeated ancestry saturates the [probability](../../../../../../probability.md). This is an exact result for the stated one-label approximation, not an exact diploid formula after substantial inbreeding has developed.

Now prohibit full-sibling matings, with $N\geq4$ and representative sampling of allowed nonsibling mating pairs. The following closed recurrences assume that opposite-sex mating pairs have the same mean autosomal sharing as all nonsibling pairs; a sex-specific or assortative scheme requires separate mating means. In the exchangeable one-label model write $u_G$ for [mean](../../../../../../expected-value.md) relatedness of a nonsibling pair, so $m_G=u_G$. The two required recurrences are

$$
\boxed{r_{G+1}=r_G+\frac{1-u_G}{2(N-1)},\qquad
u_{G+1}=\frac{(N-1)r_G-u_G}{N-2},\qquad r_0=u_0=0.}
$$

The second relation includes sharing through grandparents and more distant ancestors; setting $u_G=0$ forever would be wrong. For $v_G=1-r_G$, $w_G=1-u_G$, the linear recurrence [matrix](../../../../../../matrix.md) is

$$
\begin{pmatrix}v_{G+1}\\w_{G+1}\end{pmatrix}=
\begin{pmatrix}1&-1/[2(N-1)]\\(N-1)/(N-2)&-1/(N-2)\end{pmatrix}
\begin{pmatrix}v_G\\w_G\end{pmatrix}.
$$

Its [eigenvalues](../../../../../../eigenvalue.md) are

$$
\lambda_\pm=\frac{N-3\pm\sqrt{N^2-4N+5}}{2(N-2)},
$$

both of magnitude less than one for $N\geq4$. Thus $r_G\to1$ even when siblings never mate. Explicitly, $1-r_G=A\lambda_+^G+(1-A)\lambda_-^G$, where $A=[1-1/(2(N-1))-\lambda_-]/(\lambda_+-\lambda_-)$. Sibling avoidance prevents immediate close-relative matings, but it does not make the remaining population unrelated. In a fixed-two-offspring model it need not reduce average pairwise sharing at every generation: a smaller mating [mean](../../../../../../expected-value.md) actually increases the displayed increment in $r_G$.

For a fully diploid formulation, self-kinship also changes with inbreeding and cannot remain artificially fixed. Let $\Phi_G$ be [mean](../../../../../../expected-value.md) [kinship coefficient](../../../../../../kinship-coefficient.md) between distinct individuals, $F_G$ [mean](../../../../../../expected-value.md) [inbreeding coefficient](../../../../../../inbreeding-coefficient.md), and $\Phi_{m,G}$ [mean](../../../../../../expected-value.md) kinship of mates. A sibling pair has kinship $(1+F_G)/4+\Phi_{m,G}/2$, because parental self-kinship is $(1+F_G)/2$. Repeating the pair count yields [finite-population chromosomal coancestry](../../../../../../finite-population-chromosomal-coancestry.md):

$$
\boxed{\Phi_{G+1}=\Phi_G+\frac{1+F_G-2\Phi_{m,G}}{4(N-1)},\qquad
F_{G+1}=\Phi_{m,G}.}
$$

Initially $\Phi_0=F_0=0$. For random mating take $\Phi_{m,G}=\Phi_G$. An explicit solution is the affine [matrix](../../../../../../matrix.md) recurrence

$$
\begin{pmatrix}1-\Phi_G\\1-F_G\end{pmatrix}=
\begin{pmatrix}1-1/[2(N-1)]&1/[4(N-1)]\\1&0\end{pmatrix}^{G}
\begin{pmatrix}1\\1\end{pmatrix}.
$$

Its characteristic polynomial is $\lambda^2-[1-1/(2(N-1))]\lambda-1/[4(N-1)]$; its two roots have magnitude less than one. Hence $\Phi_G,F_G\to1$. The normalized relationship $2\Phi_G/(1+F_G)$ tends to one, while unnormalized additive relationship $2\Phi_G$ tends to two, demonstrating why that coefficient cannot always be read literally as a [probability](../../../../../../probability.md).

With sibling avoidance replace $\Phi_{m,G}$ by the nonsibling [mean](../../../../../../expected-value.md) $U_G$ and add

$$
U_{G+1}=\frac{(N-1)\Phi_G-U_G}{N-2},\qquad U_0=0.
$$

These equations compute every generation's kinship and inbreeding, including delayed consanguinity through cousins. Under random allowed mating in a connected closed population, backward ancestral gene-copy lineages have a positive chance to meet in each sufficiently long block of generations; repeated blocks force eventual coalescence. Thus sibling avoidance alone does not prevent long-term [identity by descent](../../../../../../identity-by-descent.md) and [genetic drift](../../../../../../genetic-drift.md). Maintaining distinct isolated breeding groups, introducing immigrants, or changing offspring-number [variance](../../../../../../variance-split.md) gives a different model. **The elementary exponential formula answers the fixed-self-sharing approximation; the diploid recurrences give the consistent inbreeding-aware answer.**

## ↑ Ancestors (11)

1. [C](../c.md)
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
