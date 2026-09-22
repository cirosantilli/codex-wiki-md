<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Integrating $Y''+2a\eta Y'=0$ once gives $Y'=K e^{-a\eta^2}$. A second integration expresses the solution using the [error function](../../../../error-function.md) when the value at zero is prescribed, and the [complementary error function](../../../../complementary-error-function.md) when decay at infinity is prescribed. Write $\theta_\lambda=\theta^s(\lambda)$ and take $\lambda>0$, $Le>0$. The wall condition and the interface value give

$$
\boxed{\theta^s(\eta)=\mathcal C^s(\eta)=\theta_\lambda\frac{\operatorname{erf}\eta}{\operatorname{erf}\lambda},\qquad0\leq\eta\leq\lambda.}
$$

For the exterior liquid, continuity at the interface fixes $\theta^l(\lambda)=\theta_\lambda-1+\mathcal R_\theta$ and $\mathcal C^l(\lambda)=\theta_\lambda-1$. Thus the two decaying [similarity solutions](../../../../similarity-solution.md) are

$$
\boxed{\theta^l(\eta)=(\theta_\lambda-1+\mathcal R_\theta)\frac{\operatorname{erfc}\eta}{\operatorname{erfc}\lambda},\qquad
\mathcal C^l(\eta)=(\theta_\lambda-1)\frac{\operatorname{erfc}(\sqrt{Le}\eta)}{\operatorname{erfc}(\sqrt{Le}\lambda)},\quad\eta\geq\lambda.}
$$

The factor $\sqrt{Le}$ is required because solute and heat diffuse on different length scales. Both denominators are positive for a finite positive $\lambda$. These formulas use the differential equations, wall/far-field data and continuity; the remaining three flux conditions determine their unknown constants.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the topics in fluid mechanics course of the University of Oxford](../../../split.md)
5. [Topics in fluid mechanics course of the University of Oxford](../../../../topics-in-fluid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
