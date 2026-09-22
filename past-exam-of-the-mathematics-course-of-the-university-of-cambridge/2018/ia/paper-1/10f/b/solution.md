<h1 id="10f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [mean value theorem](../../../../../../mean-value-theorem.md) says that if $f$ is continuous on $[a,b]$ and differentiable on $(a,b)$, then $f(b)-f(a)=f'(c)(b-a)$ for some $c\in(a,b)$.

For $F(t)=\cos(e^{-t})$ and $t\geq0$,

$$
|F'(t)|=e^{-t}|\sin(e^{-t})|\leq1.
$$

The mean value theorem gives **$|\cos(e^{-x})-\cos(e^{-y})|\leq|x-y|$**.

For the second inequality put $t=\sqrt{1+x}\geq1$. It becomes $2\log t\leq t-t^{-1}$. The difference $G(t)=t-t^{-1}-2\log t$ satisfies $G(1)=0$ and

$$
G'(t)=1+t^{-2}-2t^{-1}=\frac{(t-1)^2}{t^2}\geq0.
$$

Thus **$\log(1+x)\leq x/\sqrt{1+x}$**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10F](../../10f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
