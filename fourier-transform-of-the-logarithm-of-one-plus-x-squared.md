# Fourier transform of the logarithm of one plus x squared

↑ **Parent:** [Fourier transform of a tempered distribution](fourier-transform-of-a-tempered-distribution.md)

For $u(x)=\tfrac12\log(1+x^2)$, the angular-frequency transform is the [tempered distribution](tempered-distribution.md)

$$
\langle\widehat u,\varphi\rangle
=-\pi\int_{\mathbb R}\frac{\varphi(\xi)-\varphi(0)}{|\xi|}e^{-|\xi|}\,d\xi.
$$

The numerator cancels the singularity at zero and makes this integral absolutely convergent. Differentiating $u$ and using $\widehat{(1+x^2)^{-1}}=\pi e^{-|\xi|}$ determines this expression up to a [Dirac delta distribution](dirac-delta-function.md). That delta coefficient is zero: testing with the expanding Gaussian $\varphi_n(x)=(2\sqrt\pi)^{-1}e^{-x^2/(4n)}$ makes both the proposed expression and $\langle u,\widehat\varphi_n\rangle$ tend to zero, while $\varphi_n(0)$ stays fixed. Changing the subtraction convention would change the delta coefficient.

## ↑ Ancestors (8)

1. [Fourier transform of a tempered distribution](fourier-transform-of-a-tempered-distribution.md)
2. [Tempered distribution](tempered-distribution.md)
3. [Schwartz space](schwartz-space.md)
4. [Fourier analysis](fourier-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-327/1/solution.md)
