<h1 id="13b/solution">Solution</h1>

↑ **Parent:** [13B](../13b.md)

Use the positively oriented unit circle and $z=e^{i\theta}$. Writing $d=\sqrt{a^2-b^2}$, the [contour integral for a sine-squared trigonometric quotient](../../../../../contour-integral-for-a-sine-squared-trigonometric-quotient.md) becomes

$$
J=\oint_{|z|=1}-\frac{(z^2-1)^2}{2iz^2(bz^2+2az+b)}\,dz.
$$

There is a double pole at zero and simple poles at $r_\pm=(-a\pm d)/b$. Since $a>b>0$, $|r_+|<1$ and $|r_-|>1$. The coefficient of $z^{-1}$ at zero is $a/(ib^2)$. At $r=r_+$, the [residue](../../../../../residue.md) is

$$
-\frac{(r^2-1)^2}{4idr^2}=-\frac d{ib^2},
$$

because $(r-r^{-1})^2=4d^2/b^2$. The [residue theorem](../../../../../residue-theorem.md) consequently gives

$$
\boxed{J=\frac{2\pi}{b^2}\left(a-\sqrt{a^2-b^2}\right).}
$$

For the second integral, use $x=\cos(\theta/2)$ with $0\leq\theta\leq\pi$. The square root is $\sin(\theta/2)$, and reversing the integration limits gives

$$
\begin{aligned}
I&=\frac12\int_0^\pi\frac{\sin^2(\theta/2)\cos^2(\theta/2)}{1+\cos^2(\theta/2)}\,d\theta\\
&=\frac14\int_0^\pi\frac{\sin^2\theta}{3+\cos\theta}\,d\theta=\frac18J(3,1).
\end{aligned}
$$

The last factor uses the symmetry of the integrand about $\pi$ over a full period. Therefore

$$
\boxed{I=\frac\pi4(3-2\sqrt2).}
$$

## ↑ Ancestors (10)

1. [13B](../13b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
