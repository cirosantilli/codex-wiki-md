<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [inner product](../../../../../inner-product-split.md) $\langle f,g\rangle=\mathbb E[f(Z)g(Z)]$ for a [standard normal random variable](../../../../../standard-normal-random-variable.md) $Z$. The degree-zero [monic polynomial](../../../../../monic-polynomial.md) is $p_0=1$. Write $p_1=x+a$ and $p_2=x^2+bx+c$. The conditions

$$
0=\langle p_1,1\rangle=a,\qquad
0=\langle p_2,1\rangle=1+c,\qquad
0=\langle p_2,x\rangle=b
$$

use $\mathbb EZ=\mathbb EZ^3=0$ and $\mathbb EZ^2=1$. Hence these first three [Probabilists' Hermite polynomials](../../../../../probabilists-hermite-polynomial.md) are

$$
\boxed{p_0(x)=1,\qquad p_1(x)=x,\qquad p_2(x)=x^2-1.}
$$

The [Gaussian fourth moment](../../../../../gaussian-fourth-moment.md) is $\mathbb EZ^4=3$, so their squared [norms](../../../../../norm.md) are

$$
\boxed{h_0=1,\qquad h_1=1,\qquad
h_2=\mathbb E(Z^2-1)^2=3-2+1=2,}
\qquad
h_\ell=\int_{\mathbb R}p_\ell(x)^2\frac{e^{-x^2/2}}{\sqrt{2\pi}}\,dx.
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the random matrix theory course of the University of Oxford](../../../../split.md)
6. [Random matrix theory course of the University of Oxford](../../../../../random-matrix-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
