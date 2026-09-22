<h1 id="3b/solution">Solution</h1>

↑ **Parent:** [3B](../3b.md)

The integrand has an order-two [pole](../../../../../pole.md) at $0$ and a simple pole at $2$. Write it near zero as $h(z)/z^2$, where

$$
h(z)=\frac{z^2+e^z}{z-2}.
$$

Its [residue](../../../../../residue.md) at zero is

$$
h'(0)=\left.\frac{(2z+e^z)(z-2)-(z^2+e^z)}{(z-2)^2}\right|_{z=0}
=-\frac34.
$$

At $z=2$ the residue is

$$
\frac{2^2+e^2}{2^2}=1+\frac{e^2}{4}.
$$

The [residue theorem](../../../../../residue-theorem.md) now gives

$$
\boxed{
g(x)=\begin{cases}
-\dfrac{3\pi i}{2},&0<x<2,\\[4pt]
\dfrac{\pi i}{2}(1+e^2),&x>2.
\end{cases}}
$$

## ↑ Ancestors (10)

1. [3B](../3b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
