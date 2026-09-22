<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the usual localized, [compact support](../../../../../../compact-support.md) construction of an [interval-adapted wavelet basis](../../../../../../interval-adapted-wavelet-basis.md), including [boundary wavelets](../../../../../../boundary-wavelet.md) with the stated [vanishing moments](../../../../../../vanishing-moment.md), and order the [linear N-term approximation](../../../../../../linear-n-term-approximation.md) by increasing resolution. Also interpret a [piecewise polynomial function](../../../../../../piecewise-polynomial-function.md) as having finitely many pieces. These conventions matter: regularity and [vanishing moments](../../../../../../vanishing-moment.md) alone, or an arbitrary enumeration, do not establish the asserted rates.

At scale $j$, a [wavelet](../../../../../../wavelet.md) whose support lies in one polynomial piece has zero coefficient because $p<q$. Only a bounded number $B$ of [wavelets](../../../../../../wavelet.md) per scale can meet a partition point. Their $L^1$ [norms](../../../../../../norm.md) are bounded by $C2^{-j/2}$, and $f$ is bounded. Thus $|c_{j,k}|\le C_f2^{-j/2}$ and

$$
\sum_k|c_{j,k}|^2\le C_f'2^{-j}.
$$

Retain the fixed number of coarse [scaling function](../../../../../../scaling-function.md) coefficients and every nonzero coefficient through level $J$. This uses at most $B(J+1)+B_0$ terms, leaving squared error at most $C2^{-J}$. The optimal [best N-term approximation](../../../../../../best-n-term-approximation.md) is no worse; choose $J$ proportional to $N$ to obtain $O(\omega^N)$ for some $\omega\in(0,1)$. In contrast, retaining all [wavelets](../../../../../../wavelet.md) through level $J$ costs $\asymp2^J$ terms. Choosing the last complete level before $N$ gives

$$
\boxed{\|f-f_N^n\|_2^2=O(\omega^N),\qquad \|f-f_N^l\|_2^2=O(N^{-1}).}
$$

These are squared errors; the corresponding $L^2$ errors are $O(\omega^{N/2})$ and $O(N^{-1/2})$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
