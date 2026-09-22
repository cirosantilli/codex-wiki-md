# Fourier series of a noninteger-frequency cosine

↑ **Parent:** [Fourier series](fourier-series-split.md)

Extend $\cos(\mu x)$ from $[-\pi,\pi]$ with period $2\pi$. It is an [even function](even-function.md), so all sine [Fourier coefficients](fourier-coefficient.md) vanish. The product-to-sum identity gives

$$
a_0=\frac{2\sin(\pi\mu)}{\pi\mu},\qquad
a_n=\frac{2\mu(-1)^n\sin(\pi\mu)}{\pi(\mu^2-n^2)}\quad(n\geq1).
$$

Indeed, integrate $\cos(\mu x)\cos(nx)$ on $[0,\pi]$ and use $\sin(\pi(\mu\pm n))=(-1)^n\sin(\pi\mu)$. Thus

$$
f(x)=\frac{\sin(\pi\mu)}{\pi\mu}
+\frac{2\mu\sin(\pi\mu)}\pi\sum_{n=1}^\infty\frac{(-1)^n\cos(nx)}{\mu^2-n^2}.
$$

The coefficients are $O(n^{-2})$, so the series converges absolutely and uniformly. The [Dirichlet-Jordan convergence theorem](dirichlet-jordan-convergence-theorem.md) identifies it with the periodic function everywhere, including the endpoints because the two endpoint values agree. Substituting a noninteger rational frequency and a convenient $x$ yields explicit [series](series-mathematics.md) sums. Integer frequencies require taking removable limits rather than substituting into a zero denominator.

## ↑ Ancestors (5)

1. [Fourier series](fourier-series-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2/15/solution.md)
