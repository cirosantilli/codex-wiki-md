<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [homogeneous linear differential equation](../../../../../../homogeneous-linear-differential-equation.md) $y''+y=0$ has [general solution](../../../../../../general-solution.md) $C_1\cos x+C_2\sin x$. For a [particular solution](../../../../../../particular-solution.md), use [variation of parameters](../../../../../../variation-of-parameters.md) with $y_1=\cos x$, $y_2=\sin x$ and [Wronskian](../../../../../../wronskian.md) one:

$$
y_p=-\cos x\int x\sin^2x\,dx+\sin x\int x\sin x\cos x\,dx.
$$

The [double-angle formulas](../../../../../../double-angle-formula.md) and [integration by parts](../../../../../../integration-by-parts.md) give

$$
\int x\sin^2x\,dx=\frac{x^2}{4}-\frac{x\sin2x}{4}-\frac{\cos2x}{8},\qquad
\int x\sin x\cos x\,dx=-\frac{x\cos2x}{4}+\frac{\sin2x}{8}.
$$

Substitution simplifies to $-x^2\cos x/4+x\sin x/4+\cos x/8$. Absorb the last term into the [homogeneous linear differential equation](../../../../../../homogeneous-linear-differential-equation.md) solution. Therefore

$$
\boxed{y(x)=C_1\cos x+C_2\sin x+\frac{x\sin x-x^2\cos x}{4}.}
$$

Indeed, applying $d^2/dx^2+1$ to $x\sin x$ gives $2\cos x$, and applying it to $x^2\cos x$ gives $2\cos x-4x\sin x$; their difference divided by four is the required $x\sin x$.

## ↑ Ancestors (12)

1. [C](../c.md)
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
