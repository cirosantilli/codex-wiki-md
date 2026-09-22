<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $L=L^*(X)$ and $\mu=\mathbb E L$. Since $L$ is a function of $X$, the [chain rule for information entropy](../../../../../../chain-rule-for-information-entropy.md) and part (c) give

$$
H(X)=H(L)+H(X\mid L)\leq H(L)+\mu.
$$

Part (a), applied to the nonnegative integer-valued random variable $L$, yields

$$
H(L)\leq(1+\mu)h\left(\frac1{1+\mu}\right)
=\log(1+\mu)+\mu\log\left(1+\frac1\mu\right).
$$

The [logarithm inequality](../../../../../../logarithm-inequality.md) $\log(1+t)\leq t\log e$ implies $\mu\log(1+1/\mu)\leq\log e$. Thus

$$
H(X)\leq\mu+\log(1+\mu)+\log e.
$$

Part (c) also gives $\mu\leq H(X)$, so monotonicity of the [logarithm](../../../../../../logarithm.md) lets us replace $\log(1+\mu)$ by $\log(H(X)+1)$. Rearranging proves

$$
\boxed{\mathbb E[L^*(X)]
\geq H(X)-\log[H(X)+1]-\log e.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
