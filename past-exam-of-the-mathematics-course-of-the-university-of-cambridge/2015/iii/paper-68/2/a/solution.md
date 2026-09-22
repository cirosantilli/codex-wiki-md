<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Dirichlet Laplacian eigenvalues](../../../../../../dirichlet-laplacian-eigenvalue.md) and [eigenfunctions](../../../../../../eigenfunction.md) on $(-1,1)$:

$$
e_j(x)=\sin\frac{j\pi(x+1)}2,\qquad \lambda_j=\left(\frac{j\pi}2\right)^2,\qquad j\geq1.
$$

An expansion $u=\sum_jq_j(t)e_j$ reduces the [wave equation](../../../../../../wave-equation-split.md) to independent [ordinary differential equations](../../../../../../ordinary-differential-equation.md)

$$
 q_j''=(\alpha-\lambda_j)q_j.
$$

When $\alpha<\lambda_1$, put $\omega_j=\sqrt{\lambda_j-\alpha}$; each coefficient is

$$
 q_j(t)=\phi_j\cos(\omega_jt)+\frac{\psi_j}{\omega_j}\sin(\omega_jt).
$$

For finite-energy data $\phi\in H_0^1(-1,1)$ and $\psi\in L^2(-1,1)$, a uniform spatial bound follows from the [energy method](../../../../../../energy-method.md), rather than from unjustified absolute summation of the [Fourier series](../../../../../../fourier-series-split.md). The conserved quantity is

$$
 E=\frac12\left(\|u_t\|_2^2+\|u_x\|_2^2-\alpha\|u\|_2^2\right).
$$

The [Poincaré inequality](../../../../../../poincare-inequality.md) gives $\|u\|_2^2\leq\lambda_1^{-1}\|u_x\|_2^2$. Hence $2E\geq c_\alpha\|u_x\|_2^2$ with $c_\alpha=1-\alpha/\lambda_1>0$ for $0\leq\alpha<\lambda_1$, and with $c_\alpha=1$ for $\alpha<0$. Since the [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) gives $u(x,t)=\int_{-1}^xu_x(s,t)\,ds$, the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) yields

$$
\sup_{t\geq0}\|u(\cdot,t)\|_\infty\leq 2\sqrt{E/c_\alpha}<\infty.
$$

At $\alpha=\lambda_1$, the first coefficient is $q_1(t)=\phi_1+t\psi_1$, which is unbounded for some admissible data. For $\alpha>\lambda_1$, that coefficient has an exponentially growing component for some admissible data. Thus [all-time boundedness of a wave equation with a reaction term](../../../../../../all-time-boundedness-of-a-wave-equation-with-a-reaction-term.md) requires

$$
\boxed{\alpha<\pi^2/4.}
$$

At equality, boundedness for a particular data set requires $\psi_1=0$; the remaining modes are bounded by their [spectral gap](../../../../../../spectral-gap.md). Above the threshold, every unstable mode must have its growing component canceled, and any zero-frequency mode must have zero initial velocity. There is no condition on $\alpha$ alone for arbitrary specially chosen data.

The printed reference to a limit needs qualification. Bounded oscillations generally have no limit as $t\to\infty$. If actual existence of that limit for every admissible initial datum is required, **no real $\alpha$ works**: for every $\alpha$, choose $j$ with $\lambda_j>\alpha$ and nonzero pure oscillatory data in that [eigenfunction](../../../../../../eigenfunction.md). The boxed inequality answers the intended long-time boundedness question.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [Section A](../../section-a.md)
4. [Paper 68](../../../paper-68-split.md)
5. [Iii](../../../split.md)
6. [2015](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
