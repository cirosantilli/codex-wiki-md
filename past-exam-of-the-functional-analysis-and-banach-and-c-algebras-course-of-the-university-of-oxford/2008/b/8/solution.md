<h1 id="b/8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

First suppose $x$ is a [positive linear functional](../../../../positive-linear-functional.md), without assuming boundedness. Every [Hermitian C-star element](../../../../hermitian-element-of-a-c-star-algebra.md) $h$ is a difference of positive elements, since $\|h\|1\pm h\geq0$. Thus $x(h)$ is real. For a [Hermitian C-star element](../../../../hermitian-element-of-a-c-star-algebra.md) $h$ of [norm](../../../../norm.md) at most one, $-1\leq h\leq1$ gives $|x(h)|\leq x(1)$.

For arbitrary $a$, choose a scalar $\zeta$ of modulus one so that $\zeta x(a)=|x(a)|$. The [real part](../../../../real-part.md) of $\zeta a$ is a [Hermitian C-star element](../../../../hermitian-element-of-a-c-star-algebra.md) and has [norm](../../../../norm.md) at most $\|a\|$. Since $x$ is real on [Hermitian C-star elements](../../../../hermitian-element-of-a-c-star-algebra.md), it respects real parts, giving

$$
|x(a)|=x(\operatorname{Re}(\zeta a))\leq x(1)\|a\|.
$$

This proves boundedness and $\|x\|\leq x(1)$. Evaluation at the unit gives the reverse inequality, so **positivity implies $\|x\|=x(1)$**.

Conversely let $x$ be bounded with $x(1)=\|x\|=c\geq0$. If $c=0$, $x=0$ is positive. Otherwise normalize to $c=1$. For a [Hermitian C-star element](../../../../hermitian-element-of-a-c-star-algebra.md) $h$ and real $t$, the [C-star identity](../../../../c-star-identity.md) gives

$$
|1+itx(h)|\leq\|1+ith\|\leq\sqrt{1+t^2\|h\|^2}.
$$

Writing $x(h)=a+ib$ and squaring yields $-2tb+t^2(a^2+b^2)\leq t^2\|h\|^2$. Taking $t\to0$ through positive and negative values forces $b=0$. Hence $x$ is real on [Hermitian C-star elements](../../../../hermitian-element-of-a-c-star-algebra.md). If $0\leq a\leq1$, then $1-a$ has [norm](../../../../norm.md) at most one, so $x(1-a)\leq1$ and $x(a)\geq0$. Scaling proves nonnegativity on every positive element, in particular every $b^*b$. Therefore

$$
\boxed{x\text{ positive}\iff\|x\|=x(1_A).}
$$

## ↑ Ancestors (12)

1. [8](../8.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../split.md)
5. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
