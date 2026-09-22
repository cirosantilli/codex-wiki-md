<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a twice continuously differentiable function, [Itô's formula](../../../../ito-s-lemma.md) in this stopped diffusion reads

$$
f(Y_t)=f(1)+\int_0^{t\wedge\tau}f'(y_s)\,dW_s+
\frac12\int_0^{t\wedge\tau}\left(f''(y_s)+\frac{k-1}{y_s}f'(y_s)\right)ds.
$$

For $f(x)=x^{2-d}$,

$$
f'(x)=(2-d)x^{1-d},\qquad
\frac12\left(f''(x)+\frac{k-1}{x}f'(x)\right)=\frac{(2-d)(k-d)}2x^{-d}.
$$

Setting $d=k$ eliminates the drift. Moreover $f'$ is bounded on $[\alpha,\beta]$, so the stochastic integral is square-integrable on each finite horizon by the [Itô isometry](../../../../ito-isometry.md). Hence **$f(Y_t)$ is a true martingale**, not merely a local one. The process itself is bounded on the stopped interval. For $k=2$, this particular function is the constant one; the logarithmic scale function will supply the nontrivial hitting identity.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the stochastic differential equations course of the University of Oxford](../../../split.md)
5. [Stochastic differential equations course of the University of Oxford](../../../../stochastic-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
