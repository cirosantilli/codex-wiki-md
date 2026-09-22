<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [characteristic equation of a constant-coefficient differential equation](../../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md) here is $r^2-3r+2=(r-1)(r-2)=0$. Its [homogeneous solution](../../../../../homogeneous-solution.md) is $C_1e^x+C_2e^{2x}$. Because the forcing $e^x$ is already a homogeneous mode, the [method of undetermined coefficients](../../../../../method-of-undetermined-coefficients.md) requires $y_p=Axe^x$ rather than $Ae^x$.

Here $y_p'=A(x+1)e^x$ and $y_p''=A(x+2)e^x$, so $y_p''-3y_p'+2y_p=-Ae^x$. Thus $A=-1$, and the [general solution](../../../../../general-solution.md) is

$$
\boxed{y(x)=C_1e^x+C_2e^{2x}-xe^x.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Discrete mathematics, continuous mathematics and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
