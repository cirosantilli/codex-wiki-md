<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $Y_0$ and $Y_1$ be the aggregate counts in the control and treated groups. Assuming independent physicians, their [Poisson distributions](../../../../../../poisson-distribution.md) have [means](../../../../../../expected-value.md) $12\lambda$ and $12\lambda e^\beta$. Condition on $E=\{Y_0+Y_1=m\}$. By [independent Poisson conditioning](../../../../../../independent-poisson-conditioning.md),

$$
Y_1\mid E\sim\operatorname{Bin}\left(m,p\right),\qquad
p=\frac{12\lambda e^\beta}{12\lambda+12\lambda e^\beta}
=\frac{e^\beta}{1+e^\beta}.
$$

The PDF's full table gives $Y_0=67$, $Y_1=133$ and $m=200$. Thus the [Two-group Poisson ratio conditional likelihood](../../../../../../two-group-poisson-ratio-conditional-likelihood.md) is

$$
\boxed{L_c(p)=\binom{200}{133}p^{133}(1-p)^{67},\qquad0<p<1.}
$$

Conditioning the individual observations instead gives a multinomial distribution with cell probabilities $(1-p)/12$ in the first group and $p/12$ in the second; its parameter-dependent [likelihood](../../../../../../likelihood-function.md) is the same. No factor involves $\lambda$. The conditional estimates are $\widehat p=133/200$ and $\widehat\beta=\log(133/67)\simeq0.6857$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
