<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $c$ be the center and $\ell$ the side length of $Q$. The zero integral of $f$ lets us subtract a constant kernel value:

$$
T(f)(x)=\int_Q\bigl[K(x-y)-K(x-c)\bigr]f(y)\,dy.
$$

Choose $L=4\sqrt d$. For $x$ outside the concentric [cube](../../../../../../cube.md) $\widehat Q$ of side length $L\ell$, and for $y\in Q$,

$$
|x-c|\geq\frac{L\ell}{2}=2\sqrt d\,\ell,
\qquad 2|y-c|\leq\sqrt d\,\ell.
$$

Thus the domain of integration in $x$ is contained in $\{|x-c|>2|y-c|\}$. After the translations $X=x-c$ and $Y=y-c$, the [Hörmander integral kernel condition](../../../../../../hormander-integral-kernel-condition.md) gives

$$
\int_{\widehat Q^c}|K(x-y)-K(x-c)|\,dx\leq C.
$$

If $Y=0$ the difference is zero and the same inequality holds. Apply the [triangle inequality](../../../../../../triangle-inequality.md) and [Tonelli theorem](../../../../../../tonelli-theorem.md) to obtain the [cancellation estimate outside a dilated cube](../../../../../../cancellation-estimate-outside-a-dilated-cube.md):

$$
\boxed{\int_{\widehat Q^c}|T(f)(x)|\,dx\leq C\int_Q|f(y)|\,dy=C\|f\|_1.}
$$

In particular the constant on the right is the same $C$ as in the hypothesis; only the dilation $L$ depends on the dimension.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
