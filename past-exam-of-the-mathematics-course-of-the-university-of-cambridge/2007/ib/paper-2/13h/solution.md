<h1 id="13h/solution">Solution</h1>

↑ **Parent:** [13H](../13h.md)

For the first assertion, fix $x_0\in[0,1]$ and $\varepsilon>0$. By [uniform convergence](../../../../../uniform-convergence.md), choose $N$ such that $|f_N(x)-f(x)|<\varepsilon/3$ for every $x$. By continuity of $f_N$ at $x_0$, there is $\delta>0$ such that $|f_N(x)-f_N(x_0)|<\varepsilon/3$ whenever $|x-x_0|<\delta$. The [triangle inequality](../../../../../triangle-inequality.md) then gives

$$
|f(x)-f(x_0)|\le|f(x)-f_N(x)|+|f_N(x)-f_N(x_0)|+|f_N(x_0)-f(x_0)|<\varepsilon.
$$

Thus **a uniform limit of [continuous](../../../../../continuous-function.md) functions is [continuous](../../../../../continuous-function.md)**, including at the endpoints with their relative neighborhoods.

The converse implication involving integrals is **false**. Set $f_1=0$ and, for $n\ge2$, use the [shrinking continuous spikes with vanishing integral](../../../../../shrinking-continuous-spikes-with-vanishing-integral.md)

$$
f_n(x)=\max\{1-n^2|x-1/n|,0\}.
$$

Their supports are $[1/n-1/n^2,1/n+1/n^2]$. For each $x>0$ they eventually vanish at $x$, and they vanish at zero for every $n$. Hence $f_n\to0$ pointwise, with [continuous](../../../../../continuous-function.md) limit. Each triangular area is $1/n^2$, so $\int_0^1f_n\to0=\int_0^10$. Yet $\sup|f_n|=1$, excluding [uniform convergence](../../../../../uniform-convergence.md).

The final assertion is also **false**. Take $f_n(x)=x^n$. Then the [pointwise limit](../../../../../pointwise-limit.md) is

$$
f(x)=\begin{cases}0,&0\le x<1,\\1,&x=1.\end{cases}
$$

This limit is discontinuous at one but is [Riemann integrable](../../../../../riemann-integrable-function.md), with integral zero. Each $f_n$ is [continuous](../../../../../continuous-function.md) and $\int_0^1f_n=1/(n+1)\to0$. Thus convergence of the integrals to the integral of an integrable [pointwise limit](../../../../../pointwise-limit.md) does not enforce its continuity.

## ↑ Ancestors (10)

1. [13H](../13h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
