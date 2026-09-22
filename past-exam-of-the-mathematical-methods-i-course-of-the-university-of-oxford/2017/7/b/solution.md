<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Using the [complex forcing method for a real differential equation](../../../../complex-forcing-method-for-a-real-differential-equation.md), $\operatorname{Im}[(4x+2i)e^{ix}]=4x\sin x+2\cos x$, a suitable complex forcing is $f(x)=(4x+2i)e^{ix}$. Solve $u''+2u=f$ and take its [imaginary part](../../../../imaginary-part.md). Writing $u=p(x)e^{ix}$ reduces the equation to

$$
p''+2ip'+p=4x+2i.
$$

A linear polynomial $p=ax+b$ gives $a=4$ and $b=-6i$. Thus

$$
\boxed{y_p(x)=\operatorname{Im}[(4x-6i)e^{ix}]=4x\sin x-6\cos x.}
$$

For a direct check, $(4x\sin x)''+2(4x\sin x)=8\cos x+4x\sin x$, while $(-6\cos x)''+2(-6\cos x)=-6\cos x$. Their sum is the required forcing. Adding $A\cos(\sqrt2x)+B\sin(\sqrt2x)$ gives the full real solution if needed.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
