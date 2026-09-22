<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the forcing $8e^{-2x}$, the [method of undetermined coefficients](../../../../../method-of-undetermined-coefficients.md) gives the particular term $2e^{-2x}$. The term $e^{-x}$ is resonant with a homogeneous solution, so use $axe^{-x}$ for its forcing; substitution gives $a=1$.

Thus $y=C_1e^{2x}+C_2e^{-x}+2e^{-2x}+xe^{-x}$. The two initial conditions reduce to $C_1+C_2=3$ and $2C_1-C_2=0$, so $C_1=1$, $C_2=2$. The solution of the [initial value problem](../../../../../initial-value-problem.md) is

$$
\boxed{y(x)=e^{2x}+(x+2)e^{-x}+2e^{-2x}.}
$$

The extra factor $x$ in the resonant particular solution is essential.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Discrete mathematics, continuous mathematics and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
