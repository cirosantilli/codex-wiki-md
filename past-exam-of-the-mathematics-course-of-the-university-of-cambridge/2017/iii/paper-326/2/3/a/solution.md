<h1 id="2/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [Volterra operator](../../../../../../../volterra-operator.md), the identity $K^\dagger f=f'$ requires $f(0)=0$ in addition to the printed $C^2$ hypothesis. The constant function $f=1$ is a counterexample to the unrestricted domain assertion: it is not in $\mathcal D(K^\dagger)$. The estimate below is valid for derivatives of every $C^2$ function, and estimates the Moore–Penrose reconstruction when this missing boundary condition holds.

Let $e=f^\delta-f$. Apply $|a-b|^2\leq2|a|^2+2|b|^2$ separately to the two halves defining [differentiation by one-sided difference quotients](../../../../../../../differentiation-by-one-sided-difference-quotients.md):

$$
\|D_he\|_2^2\leq\frac2{h^2}\left[\|e\|_2^2+\int_h^{1/2+h}|e(t)|^2dt+\int_{1/2-h}^{1-h}|e(t)|^2dt\right]\leq\frac6{h^2}\|e\|_2^2.
$$

The two translated intervals cover each point at most twice; this proves the factor six. The shifts act on almost-everywhere equivalence classes, so no undefined pointwise data sampling is involved.

For exact data, write the forward difference as $h^{-1}\int_0^h f'(x+t)dt$ and the backward difference as $h^{-1}\int_0^h f'(x-t)dt$. If $M=\|f''\|_\infty$, either differs from $f'(x)$ by at most $h^{-1}\int_0^h Mt\,dt=Mh/2$. The interval has length one, so this also bounds the $L^2$ approximation error. The [triangle inequality](../../../../../../../triangle-inequality.md) proves the [error bound for one-sided differentiation](../../../../../../../error-bound-for-one-sided-differentiation.md):

$$
\boxed{\|D_hf^\delta-f'\|_2\leq\frac{\sqrt6\delta}{h}+\frac M2h.}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2](../../../2.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
