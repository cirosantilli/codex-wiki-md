<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For fixed $x$, put $z=r-r_0$. The [polyhedral uncertainty set](../../../../../../../polyhedral-uncertainty-set.md) is equivalent to $-\mathbf1\le Pz\le\mathbf1$, so the inner problem is the [linear program](../../../../../../../linear-programming.md)

$$
\boxed{\inf_{z\in\mathbb R^n}\ r_0^Tx+x^Tz\quad\text{subject to }Pz\le\mathbf1,\ -Pz\le\mathbf1.}
$$

The variable $z$ is unrestricted in sign. The point $z=0$ is strictly feasible. If the optimum is finite, it is attained, so the infimum is a minimum. The use of an infimum also covers possible unbounded cases permitted by the printed assumptions; strict feasibility alone does not guarantee a finite objective.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 339](../../../../paper-339-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
