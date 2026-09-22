# Fourth-order Green kernel with two decay scales

↑ **Parent:** [Green's function](green-s-function-split.md)

For $0<a<b$, the displayed decaying [Green function](green-s-function-split.md) solves $(-\partial_x^2+a^2)(-\partial_x^2+b^2)K=\delta_0$ on the real line. Its [Fourier transform](fourier-transform-split.md) is

$$
\widetilde K(k)=\frac1{(k^2+a^2)(k^2+b^2)}
=\frac1{b^2-a^2}\left(\frac1{k^2+a^2}-\frac1{k^2+b^2}\right).
$$

Invert each term using the [one-dimensional modified Helmholtz Green function](one-dimensional-modified-helmholtz-green-function.md). Then a decaying solution with forcing $h$ is the [convolution](convolution.md) $K*h$. For $a=1,b=2$, this gives $K=e^{-|x|}/6-e^{-2|x|}/12$ for the operator $\partial_x^4-5\partial_x^2+4$. Its first-derivative jump cancels, while its third-derivative jump is one, providing the unit [Dirac delta distribution](dirac-delta-function.md) required by the fourth-order operator.

## ↑ Ancestors (5)

1. [Green's function](green-s-function-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-2/5/b/solution.md)
