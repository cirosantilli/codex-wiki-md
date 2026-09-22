<h1 id="5d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The endpoint agreement $f(1)=f(0)=0$ makes the boundary terms vanish when integrating the [Fourier coefficients](../../../../../../fourier-coefficient.md) of $f'$ by parts. If $a'_n,b'_n$ denote these coefficients, then

$$
a'_n=2\pi n\,b_n=0,\qquad
b'_n=-2\pi n\,a_n=\frac2{\pi n},\qquad a'_0=0.
$$

These are exactly the coefficients obtained by differentiating the preceding [Fourier series](../../../../../../fourier-series-split.md):

$$
\boxed{G(x)=\frac2\pi\sum_{n=1}^\infty\frac{\sin(2\pi nx)}n.}
$$

On every compact subinterval of $(0,1)$ the differentiated series converges uniformly by the [Dirichlet test](../../../../../../dirichlet-test.md), since partial sums of the sine factors are uniformly bounded there. The [Termwise differentiation of a Fourier series](../../../../../../termwise-differentiation-of-a-fourier-series.md) is therefore valid away from integers and gives $1-2x$ on $(0,1)$. At an integer the periodic original has a corner, so the differentiated series is not asserting the existence of an ordinary derivative there.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5D](../../5d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
