<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use normalized [Haar measure](../../../../haar-measure.md) $dm=dt/(2\pi)$. A [homogeneous Banach space on the circle](../../../../homogeneous-banach-space-on-the-circle.md) is a Banach subspace $B\subseteq L^1(\mathbb T)$ with $\|f\|_1\leq\|f\|_B$, such that translations $\tau_s f(t)=f(t-s)$ preserve $B$, satisfy $\|\tau_sf\|_B=\|f\|_B$, and obey $\|\tau_sf-f\|_B\to0$ as $s\to0$.

For continuous $g$, the map $s\mapsto g(s)\tau_sf$ is continuous with values in the complete space $B$. Define its Banach-valued Riemann integral, equivalently its [Bochner integral](../../../../bochner-integral.md), by

$$
f*g=\int_{\mathbb T}g(s)\tau_sf\,dm(s).
$$

The [triangle inequality](../../../../triangle-inequality.md) for Riemann sums and passage to their norm limit give the canonical estimate

$$
\boxed{\|f*g\|_B\leq\int_{\mathbb T}|g(s)|\|\tau_sf\|_B\,dm(s)=\|f\|_B\|g\|_1.}
$$

The continuous inclusion into $L^1$ carries the same Riemann sums to the ordinary [convolution](../../../../convolution.md), so this definition agrees [almost everywhere](../../../../almost-everywhere.md) with $\int f(t-s)g(s)\,dm(s)$. [Density](../../../../density.md) of [continuous functions](../../../../continuous-function.md) in $L^1$, [completeness](../../../../completeness.md) of $B$, and the estimate extend the operation uniquely to all $g\in L^1$. The ordinary $L^1$ [convolution](../../../../convolution.md) estimate identifies that extension with the same integral formula.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the real and harmonic analysis course of the University of Oxford](../../../split.md)
5. [Real and harmonic analysis course of the University of Oxford](../../../../real-and-harmonic-analysis-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
