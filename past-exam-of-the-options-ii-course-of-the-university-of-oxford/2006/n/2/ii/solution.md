<h1 id="n/2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

[Independent increments](../../../../../independent-increments.md) give independent Poisson variables $N[0,s]$ and $N(s,t]$ with means $\lambda s$ and $\lambda(t-s)$. Dividing their joint probability by $\mathbb P(N[0,t]=n)$ yields

$$
\mathbb P(N[0,s]=k\mid N[0,t]=n)
=\binom nk(s/t)^k(1-s/t)^{n-k},\quad0\leq k\leq n.
$$

Thus the [conditional distribution](../../../../../conditional-distribution.md) is [binomial distribution](../../../../../binomial-distribution.md) with parameters $n,s/t$.

The event $T_i>s$ means that at most $i-1$ events have occurred by $s$. Consequently

$$
\boxed{\mathbb P(T_i>s\mid N[0,t]=n)
=\sum_{k=0}^{\min(i-1,n)}\binom nk(s/t)^k(1-s/t)^{n-k}.}
$$

For $1\leq i\leq n$, the conditional event time lies in $[0,t]$. Integrate its [survival function](../../../../../survival-function.md) and substitute $u=s/t$:

$$
\mathbb E(T_i\mid N[0,t]=n)
=t\sum_{k=0}^{i-1}\binom nk\int_0^1u^k(1-u)^{n-k}du
=t\sum_{k=0}^{i-1}\frac1{n+1}
=\boxed{\frac{it}{n+1}}.
$$

The index range $i\leq n$ is implicit in the source's last assertion. For $i>n$, the $i$th event is after $t$, and independent future increments instead give expectation $t+(i-n)/\lambda$; the displayed $it/(n+1)$ formula does not apply.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [N](../../../n.md)
4. [2006](../../../../2006-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
