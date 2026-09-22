<h1 id="31c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Suppose first that the unique interior minimum is nondegenerate, $\phi''(c)>0$, and $f(c)\ne0$. Outside a small neighbourhood of $c$ the phase exceeds $\phi(c)$ by a fixed positive amount, so that region is exponentially smaller. Inside, expand

$$
\phi(t)=\phi(c)+\tfrac12\phi''(c)(t-c)^2+O((t-c)^3),\qquad
f(t)=f(c)+O(t-c).
$$

The rescaling $s=\sqrt{\lambda\phi''(c)}(t-c)$ and a dominated local Gaussian calculation give the [Laplace method](../../../../../../laplace-s-method.md)

$$
\boxed{I(\lambda)\sim f(c)e^{-\lambda\phi(c)}
\sqrt{\frac{2\pi}{\lambda\phi''(c)}}.}
$$

If the minimum is at $a$ and $\phi'(a)>0$, the scale is $t-a=O(\lambda^{-1})$, giving $f(a)e^{-\lambda\phi(a)}/[\lambda\phi'(a)]$. At $b$ with $\phi'(b)<0$, replace the denominator by $\lambda|\phi'(b)|$. A stationary quadratic endpoint gives half the interior Gaussian factor.

The printed assumptions do not guarantee nondegeneracy or $f(c)\ne0$. More generally, if $\phi(t)-\phi(c)\sim A|t-c|^m$ with $A>0$ and even $m$ at an interior minimum, the leading phase scale is $\lambda^{-1/m}$ and, for $f(c)\ne0$, the factor is

$$
\frac{2f(c)\Gamma(1/m)}{m(A\lambda)^{1/m}}e^{-\lambda\phi(c)}.
$$

At a one-sided endpoint the factor two is absent and the first positive one-sided phase power need not be even. If the amplitude vanishes, expand it to its first contributing term; parity can cancel interior terms. A phase flat to all orders requires its actual local behavior rather than a nonexistent quadratic Taylor coefficient.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [31C](../../31c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
