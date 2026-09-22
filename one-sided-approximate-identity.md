# One-sided approximate identity

↑ **Parent:** [Approximate identity](approximate-identity.md)

Let nonnegative [integrable functions](lebesgue-integrable-function.md) $k_n$ on $[0,b]$ satisfy $\int_0^b k_n\to1$ and $\int_\delta^b k_n\to0$ for every $0<\delta<b$. If $f$ is a [bounded function](bounded-function.md) and [continuous](continuous-function.md) at zero, and the products are integrable, then $\int_0^b f(x)k_n(x)\,dx\to f(0)$. To prove this, subtract $f(0)\int k_n$ and split the difference integral at $\delta$. The first piece is bounded by $\sup_{[0,\delta]}|f-f(0)|\int k_n$; the second by $2\|f\|_\infty\int_\delta^b k_n$. First use [continuity](continuous-function.md) to choose $\delta$, then pass to the [limit](limit-of-a-function.md) in $n$. The normalization term $f(0)(\int k_n-1)$ also vanishes.

For $b=1$, the [Gaussian integral](gaussian-integral.md) shows that $k_n(x)=2ne^{-n^2x^2}/\sqrt\pi$ has these properties. The factor two compensates for retaining only the nonnegative half of the full normalized Gaussian profile. Replacing it by $n/\sqrt\pi$ would instead give limiting mass $1/2$.

## ↑ Ancestors (7)

1. [Approximate identity](approximate-identity.md)
2. [Convolution](convolution.md)
3. [Fourier analysis](fourier-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2023/prelims/mathematics-ii/7/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2023/prelims/mathematics-ii/7/c/solution.md)
