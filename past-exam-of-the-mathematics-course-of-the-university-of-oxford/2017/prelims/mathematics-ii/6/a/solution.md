<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [function](../../../../../../function-split.md) $f$ is [differentiable](../../../../../../differentiable-function.md) at $c$ if the finite [limit of a function](../../../../../../limit-of-a-function.md)

$$
f'(c)=\lim_{x\to c,\ x\ne c}\frac{f(x)-f(c)}{x-c}
$$

exists. If it exists, put $L=f'(c)$ and define

$$
\epsilon(x)=\begin{cases}\dfrac{f(x)-f(c)}{x-c}-L,&x\ne c,\\0,&x=c.\end{cases}
$$

The definition of [derivative](../../../../../../derivative.md) gives $\epsilon(x)\to0$ as $x\to c$. For $x\ne c$, rearrangement gives the desired [local linear approximation](../../../../../../local-linear-approximation.md)

$$
f(x)=f(c)+L(x-c)+\epsilon(x)(x-c).
$$

At $x=c$, this identity holds because both terms containing $x-c$ vanish. Conversely, if such an identity holds, then for $x\ne c$ its [difference quotient](../../../../../../difference-quotient.md) is $L+\epsilon(x)\to L$. Hence $f$ is [differentiable](../../../../../../differentiable-function.md) at $c$, and necessarily $\boxed{L=f'(c)}$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [Mathematics II](../../../mathematics-ii-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
