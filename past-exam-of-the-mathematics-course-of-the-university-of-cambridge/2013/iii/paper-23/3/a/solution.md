<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Riemann xi function](../../../../../../riemann-xi-function.md) is the [entire function](../../../../../../entire-function.md)

$$
\xi(s)=\frac12s(s-1)\pi^{-s/2}\Gamma(s/2)\zeta(s),\qquad \xi(0)=\xi(1)=\frac12,
$$

with $\xi(s)=\xi(1-s)$. Its [Hadamard factorization](../../../../../../hadamard-factorization-theorem.md) is

$$
\xi(s)=\frac12e^{Bs}\prod_{\rho}\left(1-\frac{s}{\rho}\right)e^{s/\rho},
\qquad B=\frac{\xi'(0)}{\xi(0)},
$$

where the [Nontrivial zeros of the Riemann zeta function](../../../../../../nontrivial-zero-of-the-riemann-zeta-function.md) are repeated by multiplicity and the factors are canonical genus-one factors.

Here is the growth estimate needed for the [Jensen zero-count bound](../../../../../../jensen-zero-count-bound.md). For $|s|\le2T$, functional symmetry reduces to $\Re s\ge1/2$. Euler summation truncated at $T^2$ bounds $(s-1)\zeta(s)$ by a fixed power of $T$, uniformly in that region; the multiplication cancels the [pole](../../../../../../pole.md) at one. The logarithmic gamma estimate bounds $\log|\Gamma(s/2)|$ by $O(T\log T)$, including the bounded small-$s$ part separately. The remaining elementary factors obey the same bound. Thus

$$
\max_{|s|\le2T}\log|\xi(s)|\le C T\log T.
$$

For a zero with $|\rho|\le T$, its contribution in [Jensen's formula](../../../../../../jensen-s-formula.md) on radius $2T$ is at least $\log2$. Consequently

$$
n_\xi(T)\log2\le\frac1{2\pi}\int_0^{2\pi}\log|\xi(2Te^{i\theta})|\,d\theta-\log|\xi(0)|
\ll T\log T.
$$

If a zero lies on the integration circle, use nearby radii and [continuity](../../../../../../continuous-function.md) of the zero-count estimate. Hence $n_\xi(T)=O(T\log T)$ for $T>2$. The growth also gives order at most one and justifies the stated [Hadamard factorization](../../../../../../hadamard-factorization-theorem.md); the zero-count bound gives convergence of its genus-one factors.

The printed logarithmic Stirling hint drops the term $-\tfrac12\log z$. The correct expansion is $(z-\tfrac12)\log z-z+\tfrac12\log(2\pi)+O(|z|^{-1})$ in a fixed sector. Its consequence $\log|\Gamma(z)|=O(|z|\log(2+|z|))$ is all that the argument needs.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
