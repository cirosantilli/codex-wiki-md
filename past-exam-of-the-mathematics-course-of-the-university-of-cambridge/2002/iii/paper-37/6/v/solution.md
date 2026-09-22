<h1 id="6/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

For [full siblings](../../../../../../full-sibling.md) in an [outbred pedigree](../../../../../../outbred-pedigree.md), [Mendelian IBD sharing of full siblings](../../../../../../mendelian-ibd-sharing-of-full-siblings.md) gives prior sharing probabilities $(1/4,1/2,1/4)$ for $J=0,1,2$. Let $A$ be the event that both siblings are affected. Bayes' rule weights those probabilities by the pair penetrances, giving immediately

$$
\boxed{\frac{\Pr(J=2\mid A)}{\Pr(J=0\mid A)}
=\frac{(1/4)p^2\beta^2}{(1/4)p^2\alpha^4}
=\frac{\beta^2}{\alpha^4}.}
$$

To obtain the one-shared-copy probability, assign each [allele](../../../../../../allele.md) a risk multiplier $R$, equal to $1$ with probability $1-\phi$ and $\theta$ with probability $\phi$. Then $\mathbb E R=\alpha$ and $\mathbb E R^2=\beta$. With $J=1$, write the siblings' penetrances as $pR_sR_1$ and $pR_sR_2$, where the shared multiplier $R_s$ and the two unshared multipliers are independent. Conditional independence of the disease outcomes gives

$$
\Pr(A\mid J=1)=p^2\mathbb E(R_s^2)\mathbb E(R_1)\mathbb E(R_2)
=p^2\beta\alpha^2.
$$

The total pair probability is therefore $p^2(\beta+\alpha^2)^2/4$, and the three ascertained sharing probabilities are

$$
\boxed{(z_0,z_1,z_2)
=\frac{(\alpha^4,\,2\alpha^2\beta,\,\beta^2)}{(\alpha^2+\beta)^2}.}
$$

In particular,

$$
\frac12-z_1
=\frac{(\beta-\alpha^2)^2}{2(\beta+\alpha^2)^2}\geq0.
$$

**The one-IBD proportion is below one half for a polymorphic locus with a genuine penetrance effect.** Equality holds when $\beta=\alpha^2$, namely when $\phi\in\{0,1\}$ or $\theta=1$; there is then no variation in the allele risk multiplier. The inequality follows from the different ascertainment weights for zero, one and two shared copies, rather than from applying the unascertained sibling probabilities to affected pairs. This is [sibling IBD ascertainment under multiplicative penetrance](../../../../../../sibling-ibd-ascertainment-under-multiplicative-penetrance.md). All affected-pair conditional probabilities presume $\Pr(A)>0$; if disease never occurs, conditioning on affected pairs is undefined.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [6](../../6.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
