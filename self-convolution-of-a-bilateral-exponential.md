# Self-convolution of a bilateral exponential

↑ **Parent:** [Convolution theorem](convolution-theorem.md)

For $a>0$ and $x\geq0$, split the [convolution](convolution.md) integral at $y=0$ and $y=x$. The three contributions are $e^{-ax}/(2a)$, $xe^{-ax}$ and $e^{-ax}/(2a)$. Evenness gives the displayed answer for all real $x$.

With [Fourier transform](fourier-transform-split.md) convention $\widetilde f(k)=\int f(x)e^{-ikx}dx$, one has $\widetilde f(k)=2a/(a^2+k^2)$. The [convolution theorem](convolution-theorem.md) and [Fourier inversion theorem](fourier-inversion-theorem.md) therefore yield

$$
\boxed{\int_{\mathbb R}\frac{e^{ikx}}{(a^2+k^2)^2}dk=\frac{\pi}{2a^3}(1+a|x|)e^{-a|x|}.}
$$

The value at $x=0$ is $\pi/(2a^3)$. Multiplying $f$ by $a/2$ instead gives a normalized [Laplace distribution](laplace-distribution.md); its self-convolution is the density $a(1+a|x|)e^{-a|x|}/4$.

## ↑ Ancestors (7)

1. [Convolution theorem](convolution-theorem.md)
2. [Convolution](convolution.md)
3. [Fourier analysis](fourier-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-2/5/solution.md)
