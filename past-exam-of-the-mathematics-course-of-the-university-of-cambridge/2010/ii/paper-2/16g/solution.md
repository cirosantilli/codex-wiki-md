<h1 id="16g/solution">Solution</h1>

↑ **Parent:** [16G](../16g.md)

The map $\beta\mapsto\omega^\beta$ is strictly increasing and continuous at limit [ordinals](../../../../../ordinal.md). Also $\omega^\beta\geq\beta$, so the set $S=\{\beta:\omega^\beta\leq\alpha\}$ is nonempty and bounded by $\alpha$. If $\sup S$ is a successor, it is already in $S$; if it is a limit, continuity gives $\omega^{\sup S}=\sup_{\beta\in S}\omega^\beta\leq\alpha$. Thus **$S$ has a greatest element $\beta$.**

The initial segment of the [well-order](../../../../../well-order.md) $\alpha$ of order type $\omega^\beta$ leaves a tail of some order type $\gamma$, giving $\omega^\beta+\gamma=\alpha$. For fixed left summand, [ordinal addition](../../../../../ordinal-addition.md) is strictly increasing in its right argument, so this $\gamma$ is unique.

Maximality gives $\alpha<\omega^{\beta+1}=\omega^\beta\omega$. Choose the least positive integer $m$ such that $\alpha<\omega^\beta m$. Then $m\geq2$ and $\omega^\beta(m-1)\leq\alpha$. If $\gamma\geq\omega^\beta(m-1)$, monotonicity of [ordinal addition](../../../../../ordinal-addition.md) would give $\alpha=\omega^\beta+\gamma\geq\omega^\beta m$, a contradiction. Hence **$\gamma<\omega^\beta(m-1)\leq\alpha$.** If $\alpha$ is not a power of $\omega$, both $\omega^\beta$ and $\gamma$ are nonzero and smaller than $\alpha$, proving decomposability.

Conversely, prove by [transfinite induction](../../../../../transfinite-induction.md) that any two ordinals below $\omega^\beta$ have sum below $\omega^\beta$. For $\beta=0$ the only smaller ordinal is zero. For $\beta=\delta+1$, choose finite $m,n$ with $x<\omega^\delta m$ and $y<\omega^\delta n$. Monotonicity gives $x+y<\omega^\delta(m+n)<\omega^{\delta+1}$. For limit $\beta$, choose $\delta<\beta$ sufficiently large that $x,y<\omega^\delta$, and apply the induction hypothesis. Thus **the nonzero indecomposable ordinals are exactly the powers of $\omega$.**

## ↑ Ancestors (10)

1. [16G](../16g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
