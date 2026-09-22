<h1 id="28j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For positive $S_0,K,T,\sigma$, the [Black-Scholes formula](../../../../../../black-scholes-formula.md) uses

$$
\boxed{d_1=\frac{\log(S_0/K)+(r+\sigma^2/2)T}{\sigma\sqrt T},\qquad d_2=d_1-\sigma\sqrt T.}
$$

To hedge the sold [European call option](../../../../../../european-call-option.md), buy $\Phi(d_1)$ shares and borrow $K e^{-rT}\Phi(d_2)$ in cash. This long [replicating strategy](../../../../../../replicating-strategy.md) has initial value $S_0\Phi(d_1)-Ke^{-rT}\Phi(d_2)$, financed by the option premium. The share holding must subsequently be rebalanced according to the option's [option delta](../../../../../../option-delta.md) in a [self-financing strategy](../../../../../../self-financing-portfolio.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [28J](../../28j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
