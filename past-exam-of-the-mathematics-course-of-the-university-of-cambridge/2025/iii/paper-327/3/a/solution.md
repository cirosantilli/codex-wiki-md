<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [phase function](../../../../../../phase-function.md) is a real smooth function $\Phi$ on $X\times(\mathbb R^k\setminus\{0\})$, positively homogeneous of degree one in $\theta$, with $d_{x,\theta}\Phi\ne0$. The [symbol class](../../../../../../symbol-class.md)

$$
\operatorname{Sym}(X,\mathbb R^k;N)
$$

consists of smooth amplitudes satisfying, on each compact $K\subset X$,

$$
|D_x^\alpha D_\theta^\beta a(x,\theta)|
\leq C_{K,\alpha,\beta}\langle\theta\rangle^{N-|\beta|}.
$$

To define the [oscillatory integral](../../../../../../oscillatory-integral.md), insert a cutoff $\chi(\varepsilon\theta)$ equal to one near zero and set

$$
\langle I_\Phi(a),f\rangle
=\lim_{\varepsilon\downarrow0}
\int_X\int_{\mathbb R^k}
e^{i\Phi(x,\theta)}a(x,\theta)f(x)
\chi(\varepsilon\theta)\,d\theta\,dx.
$$

Repeated integration by parts with an operator $L$ satisfying $Le^{i\Phi}=e^{i\Phi}$ makes the integral absolutely convergent after enough iterations and shows that the limit defines a distribution.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 327](../../../paper-327-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
