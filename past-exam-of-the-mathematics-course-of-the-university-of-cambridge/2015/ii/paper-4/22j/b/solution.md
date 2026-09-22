<h1 id="22j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Weak convergence](../../../../../../weak-convergence.md) $X_k\Rightarrow X$ means that $\mathbb E f(X_k)\to\mathbb E f(X)$ for every bounded continuous real function $f$ on $\mathbb R^d$; it is a statement about their distributions, not their coupling.

The [central limit theorem](../../../../../../central-limit-theorem.md) says that for independent identically distributed real variables of finite mean $\mu$ and variance $\sigma^2$, $\sqrt n(\bar X_n-\mu)\Rightarrow N(0,\sigma^2)$. For $\sigma>0$ this is equivalent to convergence of $(\sum X_j-n\mu)/(\sigma\sqrt n)$ to the standard [normal distribution](../../../../../../normal-distribution.md). For $\sigma=0$, every variable equals $\mu$ almost surely and the limit is the point mass at zero.

For the proof when $\sigma>0$, put $Y=(X-\mu)/\sigma$. Its [characteristic function](../../../../../../characteristic-function.md) has expansion $\varphi_Y(t)=1-t^2/2+o(t^2)$. To justify this using only a second moment, subtract the first two Taylor terms of $e^{itY}$ and use [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md), with the second-order remainder bounded by a constant times $t^2Y^2$. Independence gives the characteristic function of the normalized sum as $[\varphi_Y(t/\sqrt n)]^n\to e^{-t^2/2}$. The [Lévy continuity theorem](../../../../../../levy-continuity-theorem.md) says that pointwise convergence of characteristic functions to a characteristic function continuous at zero implies [weak convergence](../../../../../../weak-convergence.md). Since $e^{-t^2/2}$ is the characteristic function of $N(0,1)$, the result follows.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [22J](../../22j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
