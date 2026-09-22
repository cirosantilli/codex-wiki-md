<h1 id="b2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Eliminate the juvenile variable from the [stage-structured population model](../../../../../stage-structured-population-model.md). Since $y_{t+1}=2z_t$,

$$
z_{t+2}=\tfrac34 y_{t+1}+\tfrac12z_{t+1}
=\tfrac32z_t+\tfrac12z_{t+1}.
$$

The [characteristic polynomial](../../../../../characteristic-polynomial.md) of this [linear recurrence](../../../../../linear-recurrence-relation.md) is

$$
q^2-\tfrac12q-\tfrac32=(q-\tfrac32)(q+1),
$$

so $z_t=A(3/2)^t+B(-1)^t$. The [initial conditions](../../../../../initial-condition.md) give $z_0=0$ and $z_1=(3/4)10=15/2$, hence $A+B=0$ and $(3/2)A-B=15/2$. Therefore

$$
\boxed{z_t=3\left[\left(\frac32\right)^t-(-1)^t\right],\qquad t=0,1,2,\ldots}.
$$

The alternating term records the initial imbalance between life stages; the growing $(3/2)^t$ term dominates eventually.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [B2](../../b2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
