<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The kernel $k(x,y)=e^{-|x-y|}$ is real and symmetric. For $f,g\in L^2[0,1]$, [Fubini's theorem](../../../../../../fubini-s-theorem.md) gives

$$
\langle Kf,g\rangle
=\int_0^1\int_0^1k(x,y)f(y)\overline{g(x)}\,dy\,dx
=\langle f,Kg\rangle,
$$

so $K$ is self-adjoint. It is linear, and because $k\in L^2([0,1]^2)$ it is a [Hilbert-Schmidt operator](../../../../../../hilbert-schmidt-operator.md), hence bounded, with

$$
\boxed{\|K\|\leq\|k\|_{L^2([0,1]^2)}<\infty.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
