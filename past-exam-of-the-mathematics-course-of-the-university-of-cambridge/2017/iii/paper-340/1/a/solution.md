<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Fourier transform](../../../../../../fourier-transform.md) convention $\widehat f(\xi)=\int_{\mathbb R}f(x)e^{-ix\xi}\,dx$. An [orthonormal](../../../../../../orthonormal-set.md) [multiresolution analysis](../../../../../../multiresolution-analysis.md) is a family of closed [vector subspaces](../../../../../../vector-subspace.md) $V_j\subset L^2(\mathbb R)$, indexed by [integers](../../../../../../integer.md), with $V_j\subset V_{j+1}$, $\overline{\bigcup_jV_j}=L^2(\mathbb R)$, and $\bigcap_jV_j=\{0\}$. Its dilation condition is $f\in V_j$ if and only if $f(2\mathord\cdot)\in V_{j+1}$. The space $V_0$ is invariant under [integer](../../../../../../integer.md) [function translations](../../../../../../translation-of-a-function.md) and admits a [scaling function](../../../../../../scaling-function.md) $\varphi$ whose [integer](../../../../../../integer.md) [function translations](../../../../../../translation-of-a-function.md) form an [orthonormal basis](../../../../../../orthonormal-basis.md). Consequently $\varphi_{j,k}=2^{j/2}\varphi(2^j\mathord\cdot-k)$ form an [orthonormal basis](../../../../../../orthonormal-basis.md) of $V_j$.

Since $\varphi\in V_1$, expansion in that [orthonormal basis](../../../../../../orthonormal-basis.md) gives the [scaling refinement equation](../../../../../../scaling-refinement-equation.md)

$$
\varphi(x)=\sqrt2\sum_{k\in\mathbb Z}h_k\varphi(2x-k),\qquad h_k=\langle\varphi,\varphi_{1,k}\rangle.
$$

The [series](../../../../../../series-mathematics.md) converges in the [L2 norm](../../../../../../l2-norm.md). The associated [low-pass filter of a multiresolution analysis](../../../../../../low-pass-filter-of-a-multiresolution-analysis.md) is the periodic [Fourier series](../../../../../../fourier-series-split.md) symbol

$$
\boxed{m(\xi)=\frac1{\sqrt2}\sum_{k\in\mathbb Z}h_ke^{-ik\xi},\qquad\widehat\varphi(2\xi)=m(\xi)\widehat\varphi(\xi).}
$$

Initially the symbol is defined almost everywhere. [Orthonormal](../../../../../../orthonormal-set.md) [integer](../../../../../../integer.md) [function translations](../../../../../../translation-of-a-function.md) give the [quadrature mirror filter](../../../../../../quadrature-mirror-filter.md) identity $|m(\xi)|^2+|m(\xi+\pi)|^2=1$ almost everywhere. For a [Lebesgue integrable](../../../../../../lebesgue-integrable-function.md) [scaling function](../../../../../../scaling-function.md), its [Fourier transform](../../../../../../fourier-transform.md) is [continuous](../../../../../../continuous-function.md) and $|\widehat\varphi(0)|=1$; choosing a constant phase makes $\widehat\varphi(0)=1$ and the [continuous](../../../../../../continuous-function.md) representative near zero has $m(0)=1$. Different conventions absorb $\sqrt2$ into the refinement coefficients; the displayed convention fixes that ambiguity.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
