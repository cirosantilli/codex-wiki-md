<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [Fourier amplification symbol](../../../../../../fourier-amplification-symbol.md) for the semidiscrete generator. At a mode $e^{i(k\xi+l\eta)}$, the two stencil symbols are

$$
m(\xi,\eta)=\frac{4+\cos\xi+\cos\eta}{6},\qquad
\ell(\xi,\eta)=\frac{-10+4(\cos\xi+\cos\eta)+2\cos\xi\cos\eta}{3h^2}.
$$

The mass symbol satisfies $1/3\leq m\leq1$. The numerator of $\ell$ is increasing in each cosine, since each partial [derivative](../../../../../../derivative.md) is at least two, and its maximum is zero at $(1,1)$. Hence $\ell\leq0$ and the generator $\lambda_h=\ell/m$ is real and nonpositive.

Every exact-time mode is multiplied by $e^{t\lambda_h}$, of modulus at most one. [Parseval identity](../../../../../../parseval-identity.md) therefore proves

$$
\boxed{\|U(t)\|_{\ell_h^2}\leq\|U(0)\|_{\ell_h^2},\qquad
\|U\|_{\ell_h^2}^2=h^2\sum_{k,l}|U_{k,l}|^2.}
$$

The method is stable, uniformly in the spatial mesh. This is a semidiscrete conclusion: it imposes no time-step condition until a particular time integrator is applied. For the stated merely square-integrable initial data, cell averages give a well-defined stable initialization, with $\|U(0)\|_{\ell_h^2}\leq\|v\|_{L^2}$ by Cauchy–Schwarz. Arbitrary point sampling of an L2 equivalence class is not required.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
