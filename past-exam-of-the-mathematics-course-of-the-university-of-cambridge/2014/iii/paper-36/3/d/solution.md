<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Define the sufficient data sums, all over $0\leq t\leq n-2$,

$$
A=1+\sum x_{t+1}^2,\quad D=1+\sum x_t^2,\quad C=\sum x_{t+1}x_t,\quad
r=\sum x_{t+1}x_{t+2},\quad s=\sum x_tx_{t+2}.
$$

Multiplying the [likelihood function](../../../../../../likelihood-function.md) by the independent standard-normal priors and collecting the quadratic terms gives

$$
\pi(a,b)\propto\exp\left[-\frac12(Aa^2+2Cab+Db^2-2ra-2sb)\right].
$$

Let $\Lambda=\begin{pmatrix}A&C\\C&D\end{pmatrix}$ and $\Delta=AD-C^2$. This precision matrix is $I+\sum v_tv_t^T$, where $v_t=(x_{t+1},x_t)^T$, so it is positive definite even for a short or singular design. Completing the square proves

$$
\boxed{\begin{pmatrix}a\\b\end{pmatrix}\Bigm|x\sim N_2(\mu,\Sigma),\quad
\Sigma=\frac1\Delta\begin{pmatrix}D&-C\\-C&A\end{pmatrix},\quad
\mu=\frac1\Delta\begin{pmatrix}Dr-Cs\\As-Cr\end{pmatrix}.}
$$

The fully normalized [posterior](../../../../../../bayesian-posterior.md) density is

$$
\boxed{\pi(a,b)=\frac{\sqrt\Delta}{2\pi}\exp\left[-\frac12\left(\begin{pmatrix}a\\b\end{pmatrix}-\mu\right)^T\Lambda\left(\begin{pmatrix}a\\b\end{pmatrix}-\mu\right)\right].}
$$

This is [Gaussian conjugacy for an initialized AR(2) regression](../../../../../../gaussian-conjugacy-for-an-initialized-ar-2-regression.md).

Completing each one-dimensional square, or using the supplied conditional-normal identity, gives

$$
\boxed{b\mid a,x\sim N\left(\frac{s-Ca}{D},\frac1D\right),\qquad
a\mid b,x\sim N\left(\frac{r-Cb}{A},\frac1A\right).}
$$

When $n=2$, all regressor sums vanish and the [posterior](../../../../../../bayesian-posterior.md) remains the independent standard-normal prior. No stationary-parameter restriction is imposed: the specified prior is on all of $\mathbb R^2$, and the finite initialized chain is defined for all $(a,b)$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
