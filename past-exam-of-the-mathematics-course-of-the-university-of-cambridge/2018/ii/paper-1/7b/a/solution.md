<h1 id="7b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In the integral defining the [Beta function](../../../../../../beta-function.md), put $t=(1+x)/2$ and then $u=x^2$. Symmetry gives

$$
\begin{aligned}
B(z,z)
&=2^{1-2z}\int_{-1}^{1}(1-x^2)^{z-1}\,dx\\
&=2^{2-2z}\int_0^1(1-x^2)^{z-1}\,dx\\
&=2^{1-2z}\int_0^1u^{-1/2}(1-u)^{z-1}\,du\\
&=2^{1-2z}B(z,\tfrac12).
\end{aligned}
$$

This proves the identity for $\operatorname{Re}z>0$. Both sides extend by [analytic continuation](../../../../../../analytic-continuation.md) to the same [meromorphic function](../../../../../../meromorphic-function.md), equivalently by the [beta--gamma identity](../../../../../../beta-gamma-identity.md) and the [Gamma duplication formula](../../../../../../gamma-duplication-formula.md). **The identity holds meromorphically for every $z\in\mathbb C$; both sides are finite for $z\notin\{0,-1,-2,\ldots\}$ and have matching poles at the excluded points.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7B](../../7b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
