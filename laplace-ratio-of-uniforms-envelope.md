# Laplace ratio-of-uniforms envelope

↑ **Parent:** [Ratio-of-uniforms method](ratio-of-uniforms-method.md)

For the unnormalized [Laplace distribution](laplace-distribution.md) [probability density function](probability-density-function.md) $h(x)=e^{-|x-1|/2}$, the [ratio-of-uniforms method](ratio-of-uniforms-method.md) uses $0<u\leq\sqrt{h(v/u)}$. The maximum of $h$ is one. On $x\leq0$, the maximum of $x^2h(x)$ occurs at $x=-4$ and equals $16e^{-5/2}$. On $x\geq0$, it occurs at $x=4$ and equals $16e^{-3/2}$. Thus the displayed rectangle contains the region. Its area is $4(e^{-3/4}+e^{-5/4})$, while the target region has area $\tfrac12\int h=2$. Uniform proposals in the rectangle, accepted when $u^2\leq h(v/u)$, therefore return the correct [Laplace distribution](laplace-distribution.md) with acceptance [probability](probability.md) $[2(e^{-3/4}+e^{-5/4})]^{-1}$.

## ↑ Ancestors (7)

1. [Ratio-of-uniforms method](ratio-of-uniforms-method.md)
2. [Rejection sampling](rejection-sampling.md)
3. [Monte Carlo method](monte-carlo-method.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/1/a/iii/solution.md)
