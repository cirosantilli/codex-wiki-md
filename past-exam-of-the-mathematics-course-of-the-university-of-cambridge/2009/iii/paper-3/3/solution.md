<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [Noetherian module](../../../../../noetherian-module.md) satisfies the [ascending chain condition](../../../../../ascending-chain-condition.md) on its [submodules](../../../../../submodule.md); equivalently every [submodule](../../../../../submodule.md) is a [finitely generated module](../../../../../finitely-generated-module.md). If the latter condition holds, the union of an ascending chain has a finite generating set lying in one member, so the chain stabilizes. Conversely, a submodule with no finite generating set allows successive choices outside the submodule generated so far, producing a strictly ascending chain. A [Noetherian ring](../../../../../noetherian-ring.md) is a ring that is [Noetherian](../../../../../noetherian-ring.md) as a module over itself, equivalently one whose [ideals](../../../../../ideal.md) are all finitely generated.

The [formal power series ring](../../../../../formal-power-series.md) consists of sequences written $\sum_{i\ge0}a_ix^i$, with coefficientwise addition and the [Cauchy product](../../../../../cauchy-product.md):

$$
\left(\sum_{i\ge0}a_ix^i\right)\left(\sum_{j\ge0}b_jx^j\right)=\sum_{n\ge0}\left(\sum_{i=0}^na_ib_{n-i}\right)x^n.
$$

Every coefficient uses a finite sum; no analytic convergence is involved. Evaluation at zero gives $A[[x]]/(x)\cong A$. A [quotient ring](../../../../../quotient-ring.md) of a [Noetherian ring](../../../../../noetherian-ring.md) is [Noetherian](../../../../../noetherian-ring.md), because its ascending chains of [ideals](../../../../../ideal.md) lift to such chains upstairs. Thus one direction of [Noetherianity of a formal power series ring](../../../../../noetherianity-of-a-formal-power-series-ring.md) is immediate.

For the other direction suppose $A$ is [Noetherian](../../../../../noetherian-ring.md), and let $I\subseteq A[[x]]$ be an [ideal](../../../../../ideal.md). Define the [coefficient ideals of a formal power series ideal](../../../../../coefficient-ideals-of-a-formal-power-series-ideal.md)

$$
I_r=\{[x^r]g:g\in I\cap x^rA[[x]]\}\subseteq A.
$$

Each is an [ideal](../../../../../ideal.md), and multiplication by $x$ gives $I_r\subseteq I_{r+1}$. Choose $N$ with $I_N=I_{N+1}=\cdots$. For $0\le r\le N$, choose generators $a_{r1},\ldots,a_{r m_r}$ for $I_r$, and choose series $g_{rj}\in I\cap x^rA[[x]]$ whose $x^r$ coefficients are those generators. Empty generating sets are allowed for zero [ideals](../../../../../ideal.md).

These finitely many series generate $I$. To prove this without assuming that $I$ is closed, start with $g\in I$ and cancel its coefficients successively. If the residual $h_r$ lies in $I\cap x^rA[[x]]$, its $x^r$ coefficient lies in $I_r$. Put $s=\min(r,N)$; since $I_r=I_s$ when $r\ge N$, write that coefficient as $\sum_jc_{rj}a_{sj}$ and subtract $\sum_jc_{rj}x^{r-s}g_{sj}$. The new residual belongs to $I\cap x^{r+1}A[[x]]$.

For $s<N$, the generators $g_{sj}$ are used only at the single step $r=s$. For $s=N$, their accumulated multipliers are the genuine [formal power series](../../../../../formal-power-series.md) $\sum_{r\ge N}c_{rj}x^{r-N}$. Thus the construction yields the exact coefficientwise identity

$$
g=\sum_{s<N}\sum_jc_{sj}g_{sj}+\sum_j\left(\sum_{r\ge N}c_{rj}x^{r-N}\right)g_{Nj}.
$$

Every coefficient of the residual vanishes after finitely many steps. This is an ordinary finite generating expression in $A[[x]]$, not merely an approximation by elements of a smaller [ideal](../../../../../ideal.md). Therefore every [ideal](../../../../../ideal.md) is finitely generated, proving

$$
\boxed{A\text{ is Noetherian}\iff A[[x]]\text{ is Noetherian}.}
$$

Finally, for the surjective [module endomorphism](../../../../../module-endomorphism.md) $f$, the kernels $\ker f\subseteq\ker f^2\subseteq\cdots$ stabilize because $M$ is a [Noetherian module](../../../../../noetherian-module.md). Take $N$ with $\ker f^N=\ker f^{N+1}$. If $f(m)=0$, surjectivity of $f^N$ gives $u$ with $f^N(u)=m$. Then $f^{N+1}(u)=0$, so $u\in\ker f^N$ and $m=0$. Hence $f$ is injective as well as surjective; its inverse is automatically $A$-linear. This proves **$f$ is an isomorphism**, the statement that [Noetherian modules are Hopfian](../../../../../noetherian-modules-are-hopfian.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
