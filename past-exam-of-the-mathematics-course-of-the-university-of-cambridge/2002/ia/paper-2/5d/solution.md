<h1 id="5d/solution">Solution</h1>

↑ **Parent:** [5D](../5d.md)

An [integrating factor for a differential one-form](../../../../../integrating-factor-for-a-differential-one-form.md) is a nonzero function $\mu(x,y)$ for which $\mu(dy+f\,dx)$ is an [exact differential](../../../../../exact-differential.md), say $dF$. Then solutions lie on [level sets](../../../../../level-set.md) $F=\text{constant}$. Locally, the compatibility condition is $\partial_x\mu=\partial_y(\mu f)$.

Here multiplication by $2ye^x$, which is nonzero for $y>0$, produces

$$
2ye^x\,dy+e^x(2x+x^2+y^2)\,dx=d\left[e^x(x^2+y^2)\right].
$$

The [initial condition](../../../../../initial-condition.md) makes this [first integral](../../../../../first-integral.md) equal to $a^2$. Taking the positive branch yields **the solution**

$$
\boxed{y(x)=\sqrt{a^2e^{-x}-x^2},}
$$

on the connected interval containing zero where the radicand is positive. This domain restriction matters because the original [differential equation](../../../../../differential-equation-split.md) is singular at $y=0$.

Completing the square gives $2x+x^2=(x+1)^2-1\ge-1$. As $y>0$, the [differential equation](../../../../../differential-equation-split.md) consequently implies

$$
y'=-\frac{2x+x^2+y^2}{2y}\le\frac{1-y^2}{2y}.
$$

At $x=0$, $y'=-a/2<0$. Thus, moving a little to the left from $y(0)=a\ge1$, the curve rises above $a$. Throughout $y>1$ every segment of the [direction field](../../../../../direction-field.md) points downwards as $x$ increases, by the inequality above. Tracing backwards therefore makes $y$ rise further, so it cannot return to $y=1$. This graphical barrier argument proves $y>a\ge1$ and $y'<0$ for every $x<0$ on the solution. The explicit [first integral](../../../../../first-integral.md) also shows this branch extends throughout $x<0$: writing $t=-x>0$, the minimum of $e^t/t^2$ is $e^2/4>1$, so $a^2e^t-t^2>0$ for $a\ge1$. Including the initial point, **$y'<0$ for all $x\le0$.**

For $a=1$ the curve is $y=\sqrt{e^{-x}-x^2}$ on $(-\infty,b)$, where the strictly increasing function $x^2e^x$ has the unique positive root $x^2e^x=1$ at $b\simeq0.703467$. The curve decreases through $(0,1)$ with slope $-1/2$ and reaches $(b,0)$ only as a limiting endpoint. Its derivative is

$$
y'=\frac{-e^{-x}-2x}{2\sqrt{e^{-x}-x^2}}.
$$

As $x\to-\infty$, $y\sim e^{-x/2}$ and $y'\sim-\tfrac12e^{-x/2}\to-\infty$. As $x\uparrow b$, the numerator tends to $-b^2-2b<0$ and the denominator to zero from above, so again $y'\to-\infty$. More precisely, $y\sim\sqrt{b(b+2)(b-x)}$ at the endpoint. **Both ends have the requested unbounded negative slope.**

<a id="5d/image-the-positive-solution-for-initial-value-one-with-the-horizontal-barrier-and-the-steep-limiting-endpoint"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-2-integrating-factor.png)

**[Figure 2](#5d/image-the-positive-solution-for-initial-value-one-with-the-horizontal-barrier-and-the-steep-limiting-endpoint). The positive solution for initial value one, with the horizontal barrier and the steep limiting endpoint**.

## ↑ Ancestors (10)

1. [5D](../5d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
