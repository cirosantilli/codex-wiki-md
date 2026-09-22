<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take the principal [complex logarithm](../../../../../../complex-logarithm.md) and deform the interval upwards, where $e^{ixt}$ decays for $x>0$. The small indentation at zero contributes nothing because $r\log r\to0$; the distant horizontal segment vanishes exponentially. The two vertical edges therefore give the exact representation

$$
g(x)=i\int_0^\infty\left(\log s+\frac{i\pi}{2}\right)e^{-xs}\,ds-i e^{ix}\int_0^\infty\log(1+is)e^{-xs}\,ds.
$$

This is an endpoint [steepest descent contour](../../../../../../steepest-descent-contour.md), with distinct contributions from the singular endpoint and the smooth endpoint. Setting $u=xs$ in the first integral and using the given logarithmic moment gives

$$
i\int_0^\infty\left(\log s+\frac{i\pi}{2}\right)e^{-xs}\,ds
=\frac{-\pi/2-i(\log x+\gamma)}{x}.
$$

For the second edge, the Taylor series at $s=0$ is $\log(1+is)=\sum_{n\ge1}(-1)^{n+1}(is)^n/n$. [Watson's lemma](../../../../../../watson-s-lemma.md) integrates it term by term as an [asymptotic expansion](../../../../../../asymptotic-expansion.md), using $\int_0^\infty s^ne^{-xs}\,ds=n!/x^{n+1}$. Consequently

$$
\boxed{g(x)\sim\frac{-\pi/2-i(\log x+\gamma)}x-e^{ix}\sum_{k=0}^\infty\frac{k!}{(ix)^{k+2}}.}
$$

Here $\gamma$ is the [Euler--Mascheroni constant](../../../../../../euler-s-constant.md). The first smooth-endpoint terms are

$$
g(x)\sim\frac{-\pi/2-i(\log x+\gamma)}x
+e^{ix}\left(\frac1{x^2}-\frac{i}{x^3}-\frac2{x^4}+\frac{6i}{x^5}+\cdots\right).
$$

For every fixed $N\ge1$, retaining $k=0,\ldots,N-1$ leaves $O(x^{-N-2})$. The factorial series is an asymptotic series, not a convergent sum. Treating the logarithmic endpoint by an ordinary smooth-endpoint integration formula would lose the leading logarithm; this is the [logarithmic endpoint Fourier asymptotics](../../../../../../logarithmic-endpoint-fourier-asymptotics.md) mechanism.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
