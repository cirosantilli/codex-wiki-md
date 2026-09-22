<h1 id="13a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

It helps to separate the [tangent](../../../../../../tangent.md) and the squaring map. Put $t=\tan(z/2)$, with $z=x+iy$. The identity

$$
t=\frac{\sin x+i\sinh y}{\cos x+\cosh y},\qquad |t|^2=\frac{\cosh y-\cos x}{\cosh y+\cos x}
$$

shows that $0<x<\pi/2$ gives $\operatorname{Re}t>0$ and $|t|<1$. To see that every point of this right half-disc occurs, set

$$
R=\frac{1+it}{1-it},\qquad \operatorname{Re}R=\frac{1-|t|^2}{|1-it|^2}>0,\qquad \operatorname{Im}R=\frac{2\operatorname{Re}t}{|1-it|^2}>0.
$$

Then $z=-i\operatorname{Log}R$ has $0<\operatorname{Re}z<\pi/2$ and satisfies $\tan(z/2)=t$. The [principal complex logarithm](../../../../../../principal-complex-logarithm.md) is unambiguous because $R$ is in the first quadrant.

Squaring maps this right half-disc bijectively onto the [unit disc](../../../../../../unit-disc.md) with the interval $(-1,0]$ removed: the argument of $t$ lies between $-\pi/2$ and $\pi/2$, and doubles into $(-\pi,\pi)$. Thus **the desired image is**

$$
\boxed{\{w:|w|<1\}\setminus(-1,0].}
$$

Neither derivative vanishes in the domain, so the composition is also a [conformal map](../../../../../../conformal-map.md) onto that slit disc.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [13A](../../13a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
