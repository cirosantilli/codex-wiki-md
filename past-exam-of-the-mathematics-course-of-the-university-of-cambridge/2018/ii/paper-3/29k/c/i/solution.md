<h1 id="29k/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Condition (i) says that each discounted risky price $X^i$ is an integrable $\mathbb Q$-martingale. For a bounded predictable risky holding process $\theta$, self-financing gives the [discounted wealth equation in discrete time](../../../../../../../discounted-wealth-equation-in-discrete-time.md)

$$
V_t=V_0+\sum_{s=1}^t
\theta_s\mathbin{\cdot}(X_s-X_{s-1}).
$$

Each increment is integrable and

$$
\mathbb E_{\mathbb Q}[
\theta_s\mathbin{\cdot}(X_s-X_{s-1})
\mid\mathcal F_{s-1}]
=\theta_s\mathbin{\cdot}
\mathbb E_{\mathbb Q}[X_s-X_{s-1}\mid\mathcal F_{s-1}]
=0.
$$

Hence $V$ is a $\mathbb Q$-martingale, proving **(i) $\Rightarrow$ (ii)**.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [29K](../../../29k.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
