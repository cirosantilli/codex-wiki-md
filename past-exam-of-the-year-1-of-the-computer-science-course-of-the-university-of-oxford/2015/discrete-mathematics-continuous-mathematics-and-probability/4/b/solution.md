<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation-split.md) has differential operator $(D-3)^2$. Put $y=e^{3x}v$ and use the [product rule](../../../../../product-rule.md) twice:

$$
y'=e^{3x}(3v+v'),\qquad
y''=e^{3x}(9v+6v'+v'').
$$

Substitution cancels the $v$ and $v'$ terms, leaving $v''=4$. Two [integrations](../../../../../integral-split.md) give $v=2x^2+C_1x+C_2$. Hence the [general solution](../../../../../general-solution.md) is

$$
\boxed{y(x)=e^{3x}(2x^2+C_1x+C_2),\qquad C_1,C_2\in\mathbb R.}
$$

The two arbitrary constants account for the order of the [differential equation](../../../../../differential-equation-split.md); the $x^2$ factor in the particular term reflects the [repeated root](../../../../../multiple-root.md) $3$ of the [characteristic polynomial](../../../../../characteristic-polynomial.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
