<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Choose the [potential right-censoring times](../../../../../../potential-right-censoring-time.md) to include every observed [right censoring](../../../../../../right-censoring.md) time up to $t$, and also the endpoints 0 and $t$. Then no individual is censored strictly inside $(c_{k-1},c_k)$. Use an explicit endpoint convention: let $r_k$ count individuals still event-free after any events at $c_k$, but before censoring at $c_k$. If $d_k$ events occur in $(c_{k-1},c_k]$, the number at the beginning of that interval, after censoring at its left endpoint, is $r_k+d_k$.

The no-censoring interval estimate from the preceding parts is therefore $r_k/(r_k+d_k)$. The possible event mass at zero contributes $r_0/(r_0+d_0)$. Multiplying yields

$$
\boxed{\widetilde F(t)=\frac{r_0}{r_0+d_0}\prod_{k=1}^h\frac{r_k}{r_k+d_k}.}
$$

For a continuous event-time distribution, normally $d_0=0$. Within interval $k$, put $b_k=r_k+d_k$ and let its successive event counts be $e_1,\ldots,e_m$. Its [Kaplan–Meier estimator](../../../../../../kaplan-meier-estimator.md) factors telescope:

$$
\prod_{j=1}^m\left(1-\frac{e_j}{b_k-\sum_{\ell<j}e_\ell}\right)
=\frac{b_k-\sum_j e_j}{b_k}=\frac{r_k}{r_k+d_k}.
$$

The same calculation at zero proves

$$
\boxed{\widetilde F(t)=\widehat F(t).}
$$

The paper's phrase “at risk at $c_k$” does not specify its side of an event at that endpoint. If it denotes the conventional pre-event [risk set](../../../../../../risk-set.md) size $r_k^-$ instead, and $e_k$ events occur exactly at $c_k$, substitute $r_k=r_k^--e_k$. The interval factor is then $(r_k^--e_k)/(r_k^-+d_k-e_k)$; at zero it is $(r_0^--d_0)/r_0^-$. This keeps the events-before-censoring convention consistent. After an empty [risk set](../../../../../../risk-set.md), stop the product; if the fitted survival has reached zero, retain zero rather than creating a $0/0$ factor.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
