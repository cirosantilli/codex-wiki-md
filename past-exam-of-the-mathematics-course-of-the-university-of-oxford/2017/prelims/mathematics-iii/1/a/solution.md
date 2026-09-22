<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

After division by $x^2$, the [linear ordinary differential equation](../../../../../../linear-ordinary-differential-equation-split.md) becomes

$$
y'-\frac{y}{x^2}=\frac{e^{-1/x}}{x^2}.
$$

The [integrating factor](../../../../../../integrating-factor.md) is $e^{1/x}$. Thus

$$
\frac{d}{dx}\left(e^{1/x}y\right)=\frac1{x^2},\qquad e^{1/x}y=-\frac1x+C.
$$

The [initial condition](../../../../../../initial-condition.md) $y(1)=1$ gives $C=e+1$, so

$$
\boxed{y(x)=\left(e+1-\frac1x\right)e^{-1/x},\qquad x>0.}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Mathematics III](../../../mathematics-iii-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
