# Gaussian sum truncation bound

↑ **Parent:** [Gaussian Poisson summation identity](gaussian-poisson-summation-identity.md)

For $b>0$ and a nonnegative [integer](integer-split.md) $N$, define the symmetric [partial sum](partial-sum.md) and its positive remainder by

$$
S_N(b)=1+2\sum_{n=1}^{N}e^{-\pi bn^2},\qquad R_N(b)=S(b)-S_N(b).
$$

Successive omitted terms have ratio $e^{-\pi b(2n+1)}\leq e^{-\pi b(2N+3)}$ for $n\geq N+1$. Bounding them by a [geometric series](geometric-series.md) gives

$$
0<R_N(b)\leq B_N(b):=\frac{2e^{-\pi b(N+1)^2}}{1-e^{-\pi b(2N+3)}}.
$$

Consequently the physical approximation to $S(a)$ has error at most $B_N(a)$, while the dual approximation $a^{-1/2}S_N(1/a)$ has error at most $a^{-1/2}B_N(1/a)$. The prefactor must be included when setting an absolute error tolerance.

For a truncation error below $10^{-12}$, at $a=0.04$ the physical side first passes this bound with $N=15$: $31$ lattice points give $B_{15}(0.04)<2.172\times10^{-14}$, whereas $N=14$ gives $B_{14}(0.04)>10^{-12}$. The dual side needs only $k=0$. At $a=25$ the physical side needs only $n=0$, whereas the dual side first passes the bound with $N=14$: $29$ lattice points give $25^{-1/2}B_{14}(0.04)<2.146\times10^{-13}$. These counts measure symmetric lattice terms; using the [even function](even-function.md) symmetry reduces the distinct [exponential function](exponential-function.md) evaluations to $N+1$. Truncation bounds do not include rounding error in a numerical implementation.

<a id="image-positive-gaussian-tails-and-rigorous-bounds-versus-retained-lattice-points-showing-the-efficient-side-at-reciprocal-scales"></a>
![](poisson-gaussian-tail-error-work.png)

**[Figure 4](#image-positive-gaussian-tails-and-rigorous-bounds-versus-retained-lattice-points-showing-the-efficient-side-at-reciprocal-scales). Positive Gaussian tails and rigorous bounds versus retained lattice points, showing the efficient side at reciprocal scales**.

## ↑ Ancestors (7)

1. [Gaussian Poisson summation identity](gaussian-poisson-summation-identity.md)
2. [Poisson summation formula](poisson-summation-formula.md)
3. [Fourier analysis](fourier-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Gaussian Poisson summation identity](gaussian-poisson-summation-identity.md)
