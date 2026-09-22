<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume without loss of generality that $\mu(f)-\nu(f)=r\sigma$ and let $m=(\mu(f)+\nu(f))/2$. By [Chebyshev inequality](../../../../../../chebyshev-inequality.md),

$$
\mu(f<m)\leq\frac4{r^2},
\qquad
\nu(f\geq m)\leq\frac4{r^2}.
$$

Using the event $\{f\geq m\}$ in the variational definition of [total variation distance](../../../../../../total-variation-distance.md) gives

$$
\lVert\mu-\nu\rVert_{\mathrm{TV}}
\geq1-\frac8{r^2}.
$$

Start the lazy hypercube walk at $0^n$ and write

$$
\Phi(x)=\sum_{i=1}^n(-1)^{x_i}=n-2\sum_{i=1}^nx_i.
$$

This is an eigenfunction with eigenvalue $1-1/n$, so

$$
\mathbb E_0\Phi(X_t)=n(1-1/n)^t,
\qquad \mathbb E_\pi\Phi=0.
$$

The stated variance estimates allow the preceding lemma with $\sigma=\sqrt n$ and

$$
r=\sqrt n(1-1/n)^t.
$$

For $t=\tfrac12n\log n-Cn$, $r^2$ is bounded below by a constant multiple of $e^{2C}$, uniformly for all sufficiently large $n$. Choosing $C=C(\varepsilon)$ so that $1-8/r^2>\varepsilon$, and absorbing finitely many small $n$ into the constant, proves

$$
\boxed{t_{\mathrm{mix}}(\varepsilon)geq\frac12n\log n-C(\varepsilon)n.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
