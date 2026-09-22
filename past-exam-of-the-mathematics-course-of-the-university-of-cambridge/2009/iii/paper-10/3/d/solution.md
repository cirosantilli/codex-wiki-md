<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $\phi(g)=a+ib$ with $a,b\in\mathbb R$, where $g$ is real valued. The normalization and the [operator norm](../../../../../../operator-norm.md) bound imply, for every real $t$,

$$
|1+it\phi(g)|^2\leq\|1+itg\|_\infty^2=1+t^2\|g\|_\infty^2.
$$

The left side is $(1-tb)^2+t^2a^2$, so

$$
-2tb+t^2(a^2+b^2-\|g\|_\infty^2)\leq0.
$$

Divide by $t>0$ and let $t\downarrow0$ to obtain $b\geq0$. Divide by $t<0$, reversing the inequality, and let $t\uparrow0$ to obtain $b\leq0$. Thus **$\boxed{\operatorname{Im}\phi(g)=0}$** for every real-valued $g$. The first-order term in $t$ is what forces reality; this is the complex-functional step in the [unital contraction positivity criterion](../../../../../../unital-contraction-positivity-criterion.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
