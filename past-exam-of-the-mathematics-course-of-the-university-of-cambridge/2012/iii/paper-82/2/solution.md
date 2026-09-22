<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**The printed interval has a typo:** its right endpoint must be $2/3+\delta$, rather than $1/3+\delta$. Keep $\phi$ as an unnormalized [indicator function](../../../../../indicator-function.md); only $\psi$ is normalized to have [integral](../../../../../integral.md) one. Thus use

$$
\phi=\mathbf1_{[1/3-\delta,\,2/3+\delta]},\qquad
\psi=(2\delta)^{-1}\mathbf1_{[-\delta,\delta]},\qquad f=\phi*\psi.
$$

With the [Boolean literal](../../../../../boolean-literal.md) printed interval, the [convolution](../../../../../convolution.md) vanishes at $2/3$, so a sequence consisting entirely of $2/3$ is already a counterexample to the proposed majorization. For the corrected interval and every $t\in[1/3,2/3]$, all $t-s$ with $|s|\le\delta$ belong to the [support](../../../../../support.md) of $\phi$. Hence $f(t)=1$ there. Everywhere $0\le f\le1$, giving $S_N\le\sum_{n\le N}f(u_n)$, including interval endpoints.

Put $L=1/3+2\delta$. For $k\ne0$, direct integration and the [convolution theorem](../../../../../convolution-theorem.md) give the exact [Fourier coefficients](../../../../../fourier-coefficient.md)

$$
\widehat\phi(k)=e^{-\pi ik}\frac{\sin(\pi kL)}{\pi k},\qquad
\widehat\psi(k)=\frac{\sin(2\pi k\delta)}{2\pi k\delta},\qquad
\widehat f(k)=e^{-\pi ik}\frac{\sin(\pi kL)\sin(2\pi k\delta)}{2\pi^2\delta k^2},
\quad\widehat f(0)=L.
$$

In particular,

$$
|\widehat f(k)|\le\min\{L,1/(\pi|k|)\}\min\{1,1/(2\pi\delta|k|)\}
\le\frac1{2\pi^2\delta k^2}.
$$

This also supplies the required justification of the [Fourier series](../../../../../fourier-series-split.md). The [convolution](../../../../../convolution.md) $f$ is [continuous](../../../../../continuous-function.md): it is the overlap length of two moving intervals, divided by $2\delta$. Its [Fourier coefficients](../../../../../fourier-coefficient.md) are absolutely summable, so the corresponding [Fourier series](../../../../../fourier-series-split.md) converges uniformly to a [continuous function](../../../../../continuous-function.md) $g$. Termwise integration gives $\widehat g(k)=\widehat f(k)$; the permitted uniqueness assertion applied to $f-g$ yields $g=f$.

Let $A_k=\sum_{n\le N}e^{2\pi iku_n}$. Split the absolutely convergent [Fourier series](../../../../../fourier-series-split.md) at the arbitrary real cutoff $M>1$:

$$
\sum_{n\le N}f(u_n)-\frac N3
=2\delta N+\sum_{0<|k|<M}\widehat f(k)A_k+\sum_{|k|\ge M}\widehat f(k)A_k.
$$

There are fewer than $2M$ low-frequency terms and each coefficient has magnitude at most $L<1$. For the tail, $|A_k|\le N$ and $\sum_{|k|\ge M}k^{-2}\le C/M$. Therefore

$$
\boxed{S_N-\frac N3\le C\left(\delta N+\frac{N}{\delta M}+M\max_{0<|k|<M}|A_k|\right).}
$$

This proves the requested [interval discrepancy](../../../../../interval-discrepancy.md) estimate without an unjustified sharp truncation of the [Fourier series](../../../../../fourier-series-split.md).

For a nonzero integer $b$, let $a$ be the nearest integer to $b\sqrt2$. The integer $a^2-2b^2$ is nonzero, and $|a|\le\sqrt2|b|+1/2$. The suggested factorization yields

$$
1\le|a^2-2b^2|=|a-b\sqrt2|\,|a+b\sqrt2|
\le4|b|\,|a-b\sqrt2|,
\qquad\boxed{\|b\sqrt2\|_{\mathbb R/\mathbb Z}\ge\frac1{4|b|}.}
$$

This is stronger than the stated lower bound for the fractional part, since the distance to the nearest integer is at most that fractional part. For $u_n=n\sqrt2$, the [geometric series](../../../../../geometric-series.md) and $|\sin(\pi t)|\ge2\|t\|_{\mathbb R/\mathbb Z}$ give

$$
|A_k|\le\frac2{|1-e^{2\pi ik\sqrt2}|}
=\frac1{|\sin(\pi k\sqrt2)|}\le2|k|.
$$

Thus the low-frequency contribution is $O(M^2)$. Choose $M=\lceil100N^{2/5}\rceil$ and $\delta=(2\sqrt M)^{-1}$; these choices satisfy $0<\delta<1/10$ for every $N\ge1$. Both $\delta N$ and $N/(\delta M)$ are $O(N^{4/5})$, and so is $M^2$. Hence

$$
\boxed{S_N-\frac N3\le C'N^{4/5}.}
$$

## ↑ Ancestors (11)

1. [2](../2.md)
2. [Section A](../section-a.md)
3. [Paper 82](../../paper-82-split.md)
4. [Iii](../../split.md)
5. [2012](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
