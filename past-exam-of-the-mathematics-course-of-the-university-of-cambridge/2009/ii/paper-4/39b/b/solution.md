<h1 id="39b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $s=2$, part (a) gives $\rho(w)=\tfrac32w^2-2w+\tfrac12$ and the right-side [polynomial](../../../../../../polynomial-split.md) is $w^2$. On the scalar test equation $y'=\lambda y$, put $z=h\lambda$. Its characteristic equation is

$$
(\tfrac32-z)w^2-2w+\tfrac12=0,
\qquad w_\pm=\frac{2\pm\sqrt{1+2z}}{3-2z}.
$$

The [linear stability domain](../../../../../../linear-stability-domain.md) contains every $z$ for which both roots have modulus strictly less than one. For real $-1/2\le z<0$, the roots are positive; their larger numerator is less than three while their denominator exceeds three, so both are less than one. At $z=-1/2$ the repeated root is $1/2$, also strictly inside the [unit circle](../../../../../../complex-unit-circle.md). For $z<-1/2$, the roots are [complex conjugates](../../../../../../complex-conjugate.md) and their product is

$$
|w_\pm|^2=\frac1{3-2z}<1.
$$

Thus in every case both roots lie strictly inside the [unit disk](../../../../../../unit-disk.md). Repeated roots there are allowed, since [polynomial](../../../../../../polynomial-split.md) factors times their powers still tend to zero. Therefore

$$
\boxed{(-\infty,0)\text{ lies in the linear stability domain of the two-step BDF method}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [39B](../../39b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
