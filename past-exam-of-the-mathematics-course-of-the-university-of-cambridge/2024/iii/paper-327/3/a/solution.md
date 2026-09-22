<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [phase function](../../../../../../phase-function.md) is a real [smooth function](../../../../../../smooth-function.md) $\Phi$ on $X\times(\mathbb R^k\setminus\{0\})$ that is [positively homogeneous](../../../../../../positively-homogeneous-function-degree-one.md) of degree one in $\theta$ and has nonzero total differential $d_{x,\theta}\Phi$. The [symbol class](../../../../../../symbol-class.md)

$$
\operatorname{Sym}(X,\mathbb R^k;N)
$$

consists of smooth amplitudes for which, for every compact $K\subset X$ and all [multi-indices](../../../../../../multi-index-notation.md) $\alpha,\beta$,

$$
|D_x^\alpha D_\theta^\beta a(x,\theta)|
\leq C_{K,\alpha,\beta}\langle\theta\rangle^{N-|\beta|}.
$$

Choose a [smooth cutoff function](../../../../../../smooth-cutoff-function.md) $\chi$ equal to one near zero. The associated [oscillatory integral](../../../../../../oscillatory-integral.md) is defined on a [test function](../../../../../../test-function.md) $f$ by

$$
\langle I_\Phi(a),f\rangle
=\lim_{\varepsilon\downarrow0}
\int_X\int_{\mathbb R^k}
e^{i\Phi(x,\theta)}a(x,\theta)f(x)
\chi(\varepsilon\theta)\,d\theta\,dx.
$$

On the compact $x$-support of $f$, use an integration-by-parts operator $L$ satisfying $Le^{i\Phi}=e^{i\Phi}$. Repeated application of its formal adjoint lowers the effective symbol order until the integral is absolutely convergent. The resulting bounds involve only finitely many derivatives of $f$, prove that the limit is independent of $\chi$, and give the seminorm estimate required for

$$
\boxed{I_\Phi(a)\in\mathcal D'(X)}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 327](../../../paper-327-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
