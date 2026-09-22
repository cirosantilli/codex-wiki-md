<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [critical point of an elementary embedding](../../../../../../critical-point-of-an-elementary-embedding.md) $j$ is the least [ordinal](../../../../../../ordinal.md) $\alpha$ for which $j(\alpha)\ne\alpha$.

We first prove by [transfinite induction](../../../../../../transfinite-induction.md) that $j(\alpha)=\alpha$ for every $\alpha<\kappa$. Suppose this is known below $\alpha<\kappa$. If $[f]\mathrel E[\operatorname{const}_\alpha]$, then

$$
A=\{\xi<\kappa:f(\xi)<\alpha\}\in U.
$$

The sets $A_\beta=\{\xi\in A:f(\xi)=\beta\}$ for $\beta<\alpha$ partition $A$ into fewer than $\kappa$ pieces. A [kappa-complete filter](../../../../../../kappa-complete-filter.md) that is an [ultrafilter](../../../../../../ultrafilter.md) must contain one cell $A_\beta$: otherwise all their complements would belong to $U$, and their intersection would contradict $A\in U$. Hence $[f]=[\operatorname{const}_\beta]$. The predecessors of $j(\alpha)$ are consequently exactly the already-fixed ordinals below $\alpha$, so $j(\alpha)=\alpha$.

Now let $\operatorname{id}(\xi)=\xi$. An identical argument shows that the predecessors of $[\operatorname{id}]$ in the ultrapower are exactly $[\operatorname{const}_\beta]$ for $\beta<\kappa$, so

$$
\pi([\operatorname{id}])=\kappa.
$$

Since $\{\xi<\kappa:\xi<\kappa\}=\kappa\in U$, one has $[\operatorname{id}]\mathrel E[\operatorname{const}_\kappa]$. After collapsing, $\kappa\in j(\kappa)$, and therefore $j(\kappa)>\kappa$. Thus $\operatorname{crit}(j)=\kappa$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 116](../../../paper-116-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
