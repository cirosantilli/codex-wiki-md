<h1 id="5/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $K(p)=\mathcal L[k](p)$ and $F(p)=\mathcal L[f](p)$. Apply the [Laplace transform of a derivative](../../../../../laplace-transform-of-a-derivative.md) twice and use the two zero [initial conditions](../../../../../initial-condition.md). The [differential equation](../../../../../differential-equation-split.md) becomes

$$
(p^2+1)F(p)=K(p),\qquad
\boxed{F(p)=\frac{K(p)}{p^2+1}.}
$$

The factor $1/(p^2+1)$ is the [Laplace transform](../../../../../laplace-transform.md) of $\sin x$. The [convolution theorem for Laplace transforms](../../../../../convolution-theorem-for-laplace-transforms.md) therefore gives

$$
\boxed{f(x)=(\sin*k)(x)=\int_0^x\sin(x-t)k(t)\,dt.}
$$

This is a causal [convolution](../../../../../convolution.md): the value at $x$ uses only the forcing up to $x$. For ordinary continuous $k$, direct [differentiation](../../../../../differentiation.md) gives $f'(x)=\int_0^x\cos(x-t)k(t)\,dt$ and $f''(x)=k(x)-f(x)$, verifying both the [differential equation](../../../../../differential-equation-split.md) and the [initial conditions](../../../../../initial-condition.md). For an impulsive $k$, the same formula is interpreted using [distributions](../../../../../distribution-mathematical-analysis.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
