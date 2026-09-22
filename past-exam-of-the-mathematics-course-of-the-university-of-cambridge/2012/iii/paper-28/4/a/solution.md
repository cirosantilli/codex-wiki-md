<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Normalize $v_K$ to have value group $\mathbb Z$, and extend it to an algebraic closure. Suppose $\alpha$ is a root of a monic [Eisenstein polynomial](../../../../../../eisenstein-polynomial.md) of degree $n$. A root cannot have nonpositive valuation: the leading term would then have uniquely smallest valuation. If $w=v_K(\alpha)>0$, the constant term has valuation one, all the other nonleading terms have valuation strictly greater than one, and the leading term has valuation $nw$. Cancellation forces $nw=1$. The value group of $K(\alpha)$ is $(1/e)\mathbb Z$, so $n\mid e$. Since $e\leq[K(\alpha):K]\leq n$, equality holds throughout. Thus the polynomial is irreducible and the extension is [totally ramified](../../../../../../totally-ramified-extension.md).

Conversely, let $L/K$ be [totally ramified](../../../../../../totally-ramified-extension.md) of degree $n$, and choose a [uniformizer](../../../../../../uniformizer.md) $\pi_L$. Its extended $v_K$ value is $1/n$. The same denominator argument gives $[K(\pi_L):K]\geq n$, so $K(\pi_L)=L$. Every conjugate has valuation $1/n$, by the [unique extension of an absolute value to a finite extension](../../../../../../unique-extension-of-an-absolute-value-to-a-finite-extension.md) of a complete field. The nonleading coefficients of its minimal polynomial are elementary symmetric expressions in these conjugates, so their valuations are positive, hence at least one because the coefficients lie in $K$. The constant coefficient is their product and has valuation exactly one. **Its minimal polynomial is an [Eisenstein polynomial](../../../../../../eisenstein-polynomial.md), and $\boxed{L=K(\pi_L)}$.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
