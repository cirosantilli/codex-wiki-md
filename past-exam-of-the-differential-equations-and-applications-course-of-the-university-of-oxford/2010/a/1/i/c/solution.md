<h1 id="a/1/i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose a left-end solution $u(x)=e^{-x}\sin x$ and a right-end solution $v(x)=e^{-x}(\sin x+\cos x)$. They satisfy $u(0)=0$ and $v'(2\pi)=0$. Their [Wronskian](../../../../../../wronskian.md), with the order used here, is

$$
W(x)=u(x)v'(x)-u'(x)v(x)=-e^{-2x}.
$$

The [Green's function](../../../../../../green-s-function-split.md) is $u(x_<)v(x_>)/W(\xi)$, where $x_<=\min(x,\xi)$ and $x_>=\max(x,\xi)$. Explicitly,

$$
\boxed{g(x,\xi)=-e^{\xi-x}\begin{cases}
\sin x(\sin\xi+\cos\xi),&0\leq x\leq\xi,\\
\sin\xi(\sin x+\cos x),&\xi\leq x\leq2\pi.
\end{cases}}
$$

The two expressions agree at the source. Their [derivative](../../../../../../derivative.md) difference is $[u(\xi)v'(\xi)-u'(\xi)v(\xi)]/W(\xi)=1$, checking both normalization and sign. The first-order [derivative](../../../../../../derivative.md) term means the [kernel](../../../../../../kernel-of-a-linear-map-split.md) need not be symmetric under exchange of $x$ and $\xi$.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [I](../../i.md)
3. [1](../../../1.md)
4. [A](../../../../a.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the differential equations and applications course of the University of Oxford](../../../../../split.md)
7. [Differential equations and applications course of the University of Oxford](../../../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
