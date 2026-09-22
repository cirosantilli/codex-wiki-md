<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [valuation ring](../../../../../../valuation-ring.md) is $\mathcal O=\{x\in K:|x|\le1\}$, and $\mathfrak m=\{x\in K:|x|<1\}$ is an ideal by the [ultrametric inequality](../../../../../../ultrametric-inequality.md). Its complement inside $\mathcal O$ consists exactly of elements of [field absolute value](../../../../../../absolute-value-algebra.md) one, whose inverses also lie in $\mathcal O$. Every proper ideal must avoid units and hence lie in $\mathfrak m$. Therefore $\mathfrak m$ is the unique [maximal ideal](../../../../../../maximal-ideal.md): **$\mathcal O$ is a [local ring](../../../../../../local-ring.md)**. Also its fraction field is $K$, since every nonzero element outside the ring has its inverse inside it.

If $z\in K$ is integral over $\mathcal O$, it satisfies a monic equation $z^n+a_{n-1}z^{n-1}+\cdots+a_0=0$ with $|a_i|\le1$. Were $|z|>1$, the leading term would have strictly larger [field absolute value](../../../../../../absolute-value-algebra.md) than every other term, so the [ultrametric inequality](../../../../../../ultrametric-inequality.md) would prevent cancellation to zero. Thus $z\in\mathcal O$, proving **the [valuation ring](../../../../../../valuation-ring.md) is integrally closed**.

For the ideal criterion, assume the [valuation](../../../../../../valuation.md) is nontrivial and write $v=-\log|\cdot|$. If its [value group](../../../../../../value-group.md) is discrete, normalize it to $\mathbb Z$ and choose a [uniformizer](../../../../../../uniformizer.md) $\pi$ of [valuation](../../../../../../valuation.md) one. In any nonzero ideal $I$, the nonnegative integer valuations have a least value $m$. Choose $a\in I$ of that value. For every $b\in I$, $v(b/a)\ge0$, so $b\in a\mathcal O$. Hence $I=(a)=(\pi^m)$ and $\mathcal O$ is a [principal ideal domain](../../../../../../principal-ideal-domain.md).

Conversely, if $\mathcal O$ is a [principal ideal domain](../../../../../../principal-ideal-domain.md), its nonzero [maximal ideal](../../../../../../maximal-ideal.md) is $(\pi)$. For every element $x$ of positive [valuation](../../../../../../valuation.md), $x\in\mathfrak m$ implies $x=\pi y$ with $y\in\mathcal O$, so $v(x)\ge v(\pi)>0$. Thus $\gamma=v(\pi)$ is the least positive value. For any value $t$, subtract $\lfloor t/\gamma\rfloor\gamma$. The remainder belongs to the [value group](../../../../../../value-group.md) and lies in $[0,\gamma)$, so is zero. The [value group](../../../../../../value-group.md) is therefore $\gamma\mathbb Z$, and the [valuation](../../../../../../valuation.md) is discrete. We have proved the [principal ideal criterion for a nontrivial rank-one valuation ring](../../../../../../principal-ideal-criterion-for-a-nontrivial-rank-one-valuation-ring.md).

The nontriviality qualification matters under the standard definition of [discrete valuation](../../../../../../discrete-valuation.md), which requires [value group](../../../../../../value-group.md) isomorphic to $\mathbb Z$. With the trivial [field absolute value](../../../../../../absolute-value-algebra.md), $\mathcal O=K$ is still a [principal ideal domain](../../../../../../principal-ideal-domain.md), but the [value group](../../../../../../value-group.md) is zero and there is no [uniformizer](../../../../../../uniformizer.md). Thus the literal unrestricted equivalence has a field exception. If “discrete” instead includes the trivial [value group](../../../../../../value-group.md) as a discrete subgroup of $\mathbb R$, that exceptional case satisfies the equivalence too.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
