# Discrete cosine transform from an even-reflected discrete Fourier transform

↑ **Parent:** [Discrete cosine transform](discrete-cosine-transform.md)

Reflect $x$ evenly to length $2N$ by $y_n=x_n$ and $y_{2N-1-n}=x_n$. If $Y$ is the discrete Fourier transform of $y$, then

$$
Z_k=\frac12e^{-\pi ik/(2N)}Y_k.
$$

This reduction computes the cosine transform with one fast Fourier transform and $O(N)$ additional work.

## ↑ Ancestors (7)

1. [Discrete cosine transform](discrete-cosine-transform.md)
2. [Discrete Fourier transform](discrete-fourier-transform.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
