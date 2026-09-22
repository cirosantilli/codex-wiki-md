<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The second-order remainder form of [Taylor's theorem](../../../../../taylor-s-theorem.md) gives, for a point $\xi_x$ between $0$ and $x$,

$$
f(x)=-5+3x+\tfrac12f''(\xi_x)x^2.
$$

For $x\ne0$, the given curvature bounds imply

$$
-5+3x+x^2\leq f(x)<-5+3x+\tfrac32x^2.
$$

In particular $f(1)<-1/2<0$ and $f(2)\geq5>0$. Differentiability implies [continuity](../../../../../continuous-function.md), so the [intermediate value theorem](../../../../../intermediate-value-theorem.md) gives a root in $(1,2)$.

The [mean value theorem](../../../../../mean-value-theorem.md) applied to $f'$ gives $f'(x)=3+xf''(\eta_x)\geq3+2x>0$ for $x\in(1,2)$. Thus $f$ is strictly increasing there, and it cannot have two roots. **There is exactly one root in $(1,2)$.**

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
