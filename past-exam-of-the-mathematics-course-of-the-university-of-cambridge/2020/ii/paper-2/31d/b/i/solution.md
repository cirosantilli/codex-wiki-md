<h1 id="31d/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $a=1+\epsilon$ and, for $m\geq2$, define

$$
I_m(\epsilon)=\int_0^\infty(1+\epsilon t)^{-m}e^{-at}\,dt.
$$

One [integration by parts](../../../../../../../integration-by-parts.md) gives

$$
I_m(\epsilon)=\frac1a-\frac{m\epsilon}{a}I_{m+1}(\epsilon).
$$

Starting with $I=I_2$ and iterating $N+1$ times yields

$$
I(\epsilon)
=\sum_{n=0}^N
(-1)^n(n+1)!\frac{\epsilon^n}{(1+\epsilon)^{n+1}}
+R_N(\epsilon),
$$

where

$$
R_N(\epsilon)
=(-1)^{N+1}(N+2)!
\frac{\epsilon^{N+1}}{(1+\epsilon)^{N+1}}I_{N+3}(\epsilon).
$$

Since $0<I_{N+3}(\epsilon)\leq(1+\epsilon)^{-1}$, the remainder is $O(\epsilon^{N+1})$, which is little-$o$ of the last retained term. Therefore

$$
\boxed{
I(\epsilon)\sim
\sum_{n=0}^{\infty}
(-1)^n(n+1)!\frac{\epsilon^n}{(1+\epsilon)^{n+1}}
}
\qquad(\epsilon\to0^+).
$$

The displayed terms form an [asymptotic sequence](../../../../../../../asymptotic-sequence.md) because the ratio of successive magnitudes tends to zero.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [31D](../../../31d.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
