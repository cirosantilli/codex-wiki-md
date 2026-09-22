<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [dominant balance for algebraic roots](../../../../../../dominant-balance-for-algebraic-roots.md) to separate the three scales. On writing $x=\epsilon X$, the equation becomes $X^3-X^2+2\epsilon X+2\epsilon^3=0$. Its nonzero simple limiting root is $X=1$, so one root has $x_1\sim\epsilon$.

For the two remaining roots put $x=\epsilon^2Y$. Division by $\epsilon^5$ gives $\epsilon Y^3-Y^2+2Y+2\epsilon=0$. The nonzero limiting root is $Y=2$, giving $x_2\sim2\epsilon^2$. Finally $x=\epsilon^3Z$ gives, after division by $\epsilon^6$,

$$
\epsilon^3Z^3-\epsilon Z^2+2Z+2=0.
$$

Its simple limiting root is $Z=-1$. These three distinct balances account for all roots of the cubic, and

$$
\boxed{x_1\sim\epsilon,\qquad x_2\sim2\epsilon^2,\qquad x_3\sim-\epsilon^3.}
$$

For the root of smallest magnitude, set $Z=-1+b\epsilon+O(\epsilon^2)$. The order-$\epsilon$ coefficient is $-1+2b$, so $b=1/2$. Hence

$$
\boxed{x_3=-\epsilon^3+\tfrac12\epsilon^4+O(\epsilon^5).}
$$

Each rescaled root is simple at $\epsilon=0$, justifying the [regular perturbation of a simple algebraic root](../../../../../../regular-perturbation-of-a-simple-algebraic-root.md) rather than treating the original triple root as an ordinary regular perturbation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
