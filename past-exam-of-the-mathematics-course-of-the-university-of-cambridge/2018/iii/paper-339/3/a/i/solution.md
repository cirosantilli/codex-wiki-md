<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First address the positivity request in part (a), which has no separate Solution heading in the stub. For $x\in[0,1]$, each $x^k(1-x)^{n-k}$ and each coefficient $c_k$ is nonnegative. Their sum is therefore nonnegative, including at the endpoints:

$$
\boxed{f(x)\ge0\quad(0\le x\le1).}
$$

This is the elementary direction of the [positive Bernstein coefficients for a strictly positive polynomial](../../../../../../../positive-bernstein-coefficients-for-a-strictly-positive-polynomial.md) criterion; the converse developed later needs strict positivity.

For completeness, the convergence fact listed as (i) also has a short proof. If $K\sim\operatorname{Bin}(n,x)$, the [Bernstein polynomial](../../../../../../../bernstein-polynomial.md) is $B_n(f)(x)=\mathbb E[f(K/n)]$. Its mean argument is $x$ and $\operatorname{Var}(K/n)=x(1-x)/n\le1/(4n)$. Given $\epsilon>0$, [uniform continuity](../../../../../../../uniform-continuity.md) of $f$ on the compact interval supplies $\delta>0$ such that $|f(s)-f(t)|<\epsilon$ whenever $|s-t|\le\delta$. By [Chebyshev's inequality](../../../../../../../chebyshev-inequality.md), uniformly in $x$,

$$
|B_n(f)(x)-f(x)|\le\epsilon+2\|f\|_\infty\Pr(|K/n-x|>\delta)
\le\epsilon+\frac{\|f\|_\infty}{2n\delta^2}.
$$

Letting $n\to\infty$ and then $\epsilon\downarrow0$ proves $\boxed{\|B_n(f)-f\|_\infty\to0}$. The two numbered items in the source are assumptions supplied for later parts, not additional exam questions; their stub sections contain these supporting derivations.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 339](../../../../paper-339-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
