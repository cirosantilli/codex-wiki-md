# Fourier transform of a function with reciprocal tails

↑ **Parent:** [Fourier transform](fourier-transform.md)

Suppose $w$ is locally integrable and

$$
w(x)=\frac{c_+}{x}+O(x^{-2})\quad(x\to+\infty),
\qquad
w(x)=\frac{c_-}{x}+O(x^{-2})\quad(x\to-\infty).
$$

Then $\widehat w(\lambda)+(c_+-c_-)\log|\lambda|$ has finite limits at zero from both sides. With the convention $\widehat w(\lambda)=\int e^{-i\lambda x}w(x)dx$, the positive-frequency limit minus the negative-frequency limit is

$$
-i\pi(c_++c_-).
$$

Subtracting suitable reflected copies of $x^{-1}\mathbf1_{(1,\infty)}(x)$ leaves an $L^1$ function, whose Fourier transform is continuous; the jump then follows from the [Dirichlet integral](dirichlet-integral.md).

## ↑ Ancestors (5)

1. [Fourier transform](fourier-transform.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-327/1/b/vi/solution.md)
