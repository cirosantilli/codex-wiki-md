<h1 id="30k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Suppose inductively that

$$
x_{t-1}\mid W_{t-1}\sim
N(\widehat x_{t-1},V_{t-1}).
$$

The observation innovation is

$$
y_t-\widehat x_{t-1}
=(x_{t-1}-\widehat x_{t-1})+\eta_{t-1},
$$

so its conditional variance is $V_{t-1}+1$ and its conditional covariance with $x_{t-1}$ is $V_{t-1}$. The [scalar static-state Kalman update](../../../../../../scalar-static-state-kalman-update.md) therefore gives

$$
\boxed{h_t=\frac{V_{t-1}}{V_{t-1}+1}},
\qquad
V_t=\frac{V_{t-1}}{V_{t-1}+1}.
$$

Adding the known control $u_{t-1}$ shifts the conditional mean but not the variance, giving exactly

$$
\widehat x_t
=\widehat x_{t-1}+u_{t-1}
+h_t(y_t-\widehat x_{t-1}).
$$

Since $V_0=1$, induction yields

$$
\boxed{V_t=\frac1{t+1},\qquad h_t=\frac1{t+1}.}
$$

Every update is an affine conditioning operation on jointly [Gaussian random variables](../../../../../../gaussian-random-variable.md), so

$$
\boxed{x_t\mid W_t\sim N(\widehat x_t,1/(t+1)).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [30K](../../30k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
