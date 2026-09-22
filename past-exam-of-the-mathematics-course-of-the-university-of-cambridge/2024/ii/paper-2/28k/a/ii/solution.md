<h1 id="28k/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For ordered birth times $0<s_1<\cdots<s_n<t$, with $s_0=0$, the joint density of births at those times followed by no further birth before $t$ is

$$
\left[\prod_{k=1}^n k\lambda
e^{-k\lambda(s_k-s_{k-1})}\right]
e^{-(n+1)\lambda(t-s_n)}
=n!\lambda^n e^{\lambda\sum_ks_k-(n+1)\lambda t}.
$$

Also

$$
\mathbb P(X_t=n+1)
=e^{-\lambda t}(1-e^{-\lambda t})^n
=e^{-(n+1)\lambda t}(e^{\lambda t}-1)^n.
$$

Division gives

$$
n!\prod_{k=1}^n
\frac{\lambda e^{\lambda s_k}}{e^{\lambda t}-1},
$$

which is exactly the joint density of the order statistics of $n$ independent variables with the stated density. This proves the [conditional Yule birth times](../../../../../../../conditional-yule-birth-times.md) result.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [28K](../../../28k.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
