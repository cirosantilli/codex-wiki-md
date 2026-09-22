<h1 id="28k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Conditioned on the jump-chain states, the successive holding times are independent exponentials with rates $q_{i_0},\ldots,q_{i_n}$. Hence

$$
q_{i_n}\mathbb P(J_n\leq t<J_{n+1}\mid Y_0=i_0,\ldots,Y_n=i_n)
$$

equals the [integral](../../../../../../integral.md) over $s_0,\ldots,s_{n-1}\geq0$ with $\sum_{r<n}s_r\leq t$ of

$$
\left(\prod_{r=0}^{n-1}q_{i_r}e^{-q_{i_r}s_r}\right)
q_{i_n}e^{-q_{i_n}(t-\sum_{r<n}s_r)}.
$$

This simplex [integral](../../../../../../integral.md) is unchanged by reversing the $n+1$ time portions and the rates attached to them. It is therefore

$$
q_{i_0}\mathbb P(J_n\leq t<J_{n+1}\mid Y_0=i_n,\ldots,Y_n=i_0),
$$

as required. This is [holding-time reversal along a fixed CTMC jump path](../../../../../../holding-time-reversal-along-a-fixed-ctmc-jump-path.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [28K](../../28k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
