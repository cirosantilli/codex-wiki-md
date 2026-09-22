<h1 id="38c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Insert a smooth exact function into the [multistep method](../../../../../../linear-multistep-method.md) and expand its residual about $t_n$. Define

$$
c_0=\sum_{i=0}^s\rho_i,\qquad c_k=\sum_{i=0}^s\rho_i i^k-k\sum_{i=0}^s\sigma_i i^{k-1}\quad(k\ge1).
$$

The residual is $\sum_{k\ge0}h^kc_k y^{(k)}(t_n)/k!$. Therefore order at least $p$ is equivalent to $c_0=\cdots=c_p=0$. Applying the residual to the monomials $(t-t_n)^k$, $k\le p$, gives exactly those conditions. Linearity then makes them equivalent to exactness on every polynomial of degree at most $p$, as asserted. For exact rather than at-least order $p$, the next coefficient must not vanish.

If an $s$-step formula were exact for degree $2s+1$, use [Hermite interpolation](../../../../../../hermite-interpolation.md) to choose $Q$ with $Q(t_{n+i})=0$ for $i<s$, $Q(t_{n+s})=1$, and $Q'(t_{n+i})=0$ for every $i$. Its degree is at most $2s+1$. The purported identity would then read $\rho_s=0$, contradicting $\rho_s=1$. **No $s$-step method has order $2s+1$ or higher.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [38C](../../38c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
