<h1 id="2f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Since the positive series converges, $a_n\to0$. We construct the subsequence recursively. Choose $n(1)$ arbitrarily. Once $n(1)<\cdots<n(k-1)$ have been chosen, write the reduced partial sums as

$$
s_j=\sum_{r=1}^j a_{n(r)}=\frac{p_j}{q_j}
\qquad(1\leq j<k).
$$

Choose $n(k)>n(k-1)$ so far out that

$$
0<a_{n(k)}<2^{-k}min_{1\leq j<k}q_j^{-j}.
$$

This is possible because $a_n\to0$.

Let

$$
\alpha=\sum_{k=1}^{\infty}a_{n(k)}.
$$

For every fixed $j$, each later choice includes $q_j^{-j}$ in its minimum, so

$$
0<\alpha-s_j
<q_j^{-j}\sum_{k=j+1}^{\infty}2^{-k}
=2^{-j}q_j^{-j}.
$$

First, $\alpha$ is irrational. If $\alpha=u/v$ were reduced and rational, the strictly increasing rational sequence $s_j\to\alpha$ would have unbounded denominators $q_j$; only finitely many reduced fractions in a bounded interval have bounded denominator. Choose $j>2$ with $q_j>v$. Part (b) would give

$$
|\alpha-s_j|>q_j^{-2},
$$

contrary to $|\alpha-s_j|<2^{-j}q_j^{-j}<q_j^{-2}$.

If $\alpha$ were algebraic of degree $d$, part (a) would give a constant $c>0$ with

$$
|\alpha-s_j|>c q_j^{-d}.
$$

For $j>d$ our construction instead gives

$$
|\alpha-s_j|<2^{-j}q_j^{-j}
\leq2^{-j}q_j^{-d},
$$

which contradicts the lower bound once $2^{-j}<c$. Hence $\alpha$ is transcendental. This proves the [transcendental subseries of a positive rational convergent series](../../../../../../transcendental-subseries-of-a-positive-rational-convergent-series.md) construction.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2F](../../2f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
