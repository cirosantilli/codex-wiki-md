<h1 id="29k/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the [European call option](../../../../../../european-call-option.md), risk-neutral valuation gives

$$
\begin{aligned}
x
&=(1+r)^{-N}\mathbb E_Q[(S_N-K)^+]\\
&=(1+r)^{-N}\mathbb E_Q[S_N\mathbf1_{\{S_N>K\}}]
-K(1+r)^{-N}Q(S_N>K).
\end{aligned}
$$

Define the [stock-numeraire measure in a binomial market](../../../../../../stock-numeraire-measure-in-a-binomial-market.md) by

$$
\widehat Q(A)
=\frac{\mathbb E_Q[S_N\mathbf1_A]}{S_0(1+r)^N}.
$$

It is a probability measure because the risk-neutral martingale property gives $\mathbb E_QS_N=S_0(1+r)^N$. Consequently

$$
\boxed{
x=S_0\widehat Q(S_N>K)
-K(1+r)^{-N}Q(S_N>K)}.
$$

Tilting one up move by its stock factor changes its probability to

$$
\boxed{
\widehat q=\frac{q(1+b)}{1+r}
=\frac{(1+b)(r-a)}{(1+r)(b-a)}}.
$$

Similarly $1-\widehat q=(1-q)(1+a)/(1+r)$. Thus under $\widehat Q$ the number of up moves is binomial with parameter $\widehat q$, and

$$
\boxed{\widehat Q\!\left(S_N=S_0(1+b)^i(1+a)^{N-i}\right)
=\binom Ni\widehat q^{\,i}(1-\widehat q)^{N-i}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [29K](../../29k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
