<h1 id="1/d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The integrand is positive, so the [minimum-variance importance distribution](../../../../../minimum-variance-importance-distribution.md) is its target-weighted [probability density function](../../../../../probability-density-function.md), normalized by $\theta=\sqrt e$:

$$
\boxed{q^\star(z)=\frac{e^{-z_1}p(z)}{\sqrt e}.}
$$

By [completing the square](../../../../../completing-the-square.md),

$$
-z_1-\frac12z_1^2-\frac12=-\frac12(z_1+1)^2.
$$

Thus $q^\star$ is the [multivariate normal distribution](../../../../../multivariate-normal-distribution.md) $N(-e_1,I_d)$, where $e_1=(1,0,\ldots,0)$ is the first [standard basis](../../../../../standard-basis.md) vector. Its [importance weight](../../../../../importance-weight.md) and weighted integrand are

$$
\boxed{w^\star(z)=e^{z_1+1/2},\qquad
w^\star(z)e^{-z_1}=\sqrt e,\qquad
\min_q\operatorname{Var}(\widehat\theta_n^{\mathrm{IS}})=0.}
$$

A [variance](../../../../../variance-split.md) cannot be negative, and this proposal makes every summand constant, proving optimality directly. It is admissible under the arbitrary-proposal condition even though its [mean vector](../../../../../mean-vector.md) is not zero. Although optimal proposals usually involve an unknown normalizing integral, here both that integral and the resulting [normal distribution](../../../../../normal-distribution.md) are explicit.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
