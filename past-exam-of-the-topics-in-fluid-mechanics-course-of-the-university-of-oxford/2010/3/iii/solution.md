<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Introduce three positive functions of the unknown front parameter:

$$
P(\lambda)=\frac{e^{-\lambda^2}}{\sqrt\pi\operatorname{erf}\lambda},\quad
Q(\lambda)=\frac{e^{-\lambda^2}}{\sqrt\pi\operatorname{erfc}\lambda},\quad
R(\lambda)=\frac{\sqrt{Le}\,e^{-Le\lambda^2}}{\sqrt\pi\operatorname{erfc}(\sqrt{Le}\lambda)}.
$$

Differentiating the [error function](../../../../error-function.md) profiles gives $\theta^{s\prime}=2P\theta_\lambda$, $\theta^{l\prime}=-2Q(\theta_\lambda-1+\mathcal R_\theta)$ and $\mathcal C^{l\prime}=-2R(\theta_\lambda-1)$ at the interface. The three flux conditions are therefore exactly

$$
\boxed{\begin{aligned}
\phi\lambda S&=P\theta_\lambda+Q(\theta_\lambda-1+\mathcal R_\theta),\\
\phi Le\lambda(\theta_\lambda-1+\mathcal R_C)&=R(\theta_\lambda-1),\\
Q(\theta_\lambda-1+\mathcal R_\theta)&=R(\theta_\lambda-1).
\end{aligned}}
$$

These undivided equations are the safest description of the [constant-fraction mushy-layer similarity solution](../../../../constant-fraction-mushy-layer-similarity-solution.md), including degenerate parameter choices. In the nondegenerate case the third equation first gives

$$
\boxed{\theta_\lambda=1+\frac{Q(\lambda)\mathcal R_\theta}{R(\lambda)-Q(\lambda)}.}
$$

The second then gives the [solid fraction](../../../../solid-fraction.md)

$$
\boxed{\phi=\frac{R(\lambda)(\theta_\lambda-1)}{Le\lambda(\theta_\lambda-1+\mathcal R_C)}.}
$$

Use the third equation to replace the $Q$ term in the first, and eliminate $\phi$. The front parameter is a positive root of the single [transcendental equation](../../../../transcendental-equation.md)

$$
\boxed{\frac{S R(\lambda)(\theta_\lambda-1)}{Le(\theta_\lambda-1+\mathcal R_C)}-P(\lambda)\theta_\lambda-R(\lambda)(\theta_\lambda-1)=0,\qquad
\theta_\lambda=1+\frac{Q(\lambda)\mathcal R_\theta}{R(\lambda)-Q(\lambda)}.}
$$

Then substitute back for $\theta_\lambda,\phi$ and $h(t)=2\lambda\sqrt{\kappa t}$. Since the physical parameters have not been assigned numbers, an implicit scalar equation is the appropriate determination of $\lambda$.

The divided formulas require $R\ne Q$ and $\theta_\lambda-1+\mathcal R_C\ne0$. If either vanishes, return to the boxed three-equation system. For example $Le=1$ gives $R=Q$, so the last equation demands $\mathcal R_\theta=0$; otherwise this proposed [similarity solution](../../../../similarity-solution.md) cannot exist. A physical branch must also have $\lambda>0$ and $0\leq\phi\leq1$. The algebra alone does not establish existence or uniqueness of such a branch for arbitrary parameters.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
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
