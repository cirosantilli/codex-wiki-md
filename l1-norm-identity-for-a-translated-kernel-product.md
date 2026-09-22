# L1 norm identity for a translated kernel product

↑ **Parent:** [Convolution kernel](convolution-kernel.md)

Let $k$ be a [Borel measurable function](borel-measurable-function.md) in [L1 space](l1-space.md) on $\mathbb R$, and let $g$ be [Lebesgue integrable](lebesgue-integrable-function.md). The [function](function-split.md) $f(x,y)=k(x-y)g(y)$ is measurable. [Tonelli's theorem](tonelli-theorem.md) for $|f|$ and [translation invariance of Lebesgue measure](translation-invariance-of-lebesgue-measure.md) give

$$
\int_{\mathbb R^2}|k(x-y)g(y)|\,dx\,dy
=\int_{\mathbb R}|g(y)|\left(\int_{\mathbb R}|k(x-y)|\,dx\right)dy
=\|k\|_1\|g\|_1.
$$

Finiteness justifies [Fubini's theorem](fubini-s-theorem.md) for the signed product, yielding $\int_{\mathbb R^2}f=(\int k)(\int g)$. In particular an integrable [odd function](odd-function.md) $k$ makes this signed total zero while the joint [L1 norm](l1-norm.md) can remain positive. The [triangle inequality for an integral](integral-triangle-inequality.md) also gives the usual [convolution](convolution.md) estimate $\|k*g\|_1\leq\|k\|_1\|g\|_1$.

## ↑ Ancestors (7)

1. [Convolution kernel](convolution-kernel.md)
2. [Convolution](convolution.md)
3. [Fourier analysis](fourier-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-integration-course-of-the-university-of-oxford/2015/3/b/solution.md)
