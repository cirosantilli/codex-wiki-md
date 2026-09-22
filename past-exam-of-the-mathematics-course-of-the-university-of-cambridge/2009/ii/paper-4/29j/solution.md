<h1 id="29j/solution">Solution</h1>

↑ **Parent:** [29J](../29j.md)

The terminal wealth of portfolio $\psi$ is the scalar [normal distribution](../../../../../normal-distribution.md) $\psi\cdot X$, with mean $\psi\cdot\mu$ and [variance](../../../../../variance-split.md) $\psi\cdot V\psi$. Its Gaussian exponential moment gives

$$
E[U(\psi\cdot X)]=-\exp\left(-\gamma\psi\cdot\mu+\frac{\gamma^2}{2}\psi\cdot V\psi\right)
=-e^{-\gamma q(\psi)}.
$$

Since $-e^{-\gamma q}$ is strictly increasing in $q$, **strict preference is exactly $q(\psi)>q(\theta)$**. The nonsingular [covariance matrix](../../../../../covariance-matrix.md) is positive definite. Completing the square gives

$$
q(\psi)=\frac1{2\gamma}\mu^TV^{-1}\mu
-\frac\gamma2\left(\psi-\gamma^{-1}V^{-1}\mu\right)^TV\left(\psi-\gamma^{-1}V^{-1}\mu\right),
$$

so the unique optimum is $\boxed{\psi^*=\gamma^{-1}V^{-1}\mu}$.

Paying the deterministic transaction cost reduces the certainty equivalent of the new portfolio by $\epsilon\|z\|_1$. Put $g=\mu-\gamma V\theta$. Its gain over the current portfolio is exactly

$$
q(\theta+z)-q(\theta)-\epsilon\|z\|_1
=g\cdot z-\frac\gamma2z^TVz-\epsilon\|z\|_1.
$$

If every $|g_i|\le\epsilon$, then $g\cdot z\le\epsilon\|z\|_1$, so every nonzero trade has strictly negative gain, by positive definiteness. Conversely, if $|g_i|>\epsilon$, choose $z=t\operatorname{sign}(g_i)e_i$. Its gain is

$$
t(|g_i|-\epsilon)-\frac\gamma2t^2V_{ii}>0
$$

for $0<t<2(|g_i|-\epsilon)/(\gamma V_{ii})$. Therefore

$$
\boxed{\text{No beneficial trade exists}\quad\Longleftrightarrow\quad|\mu_i-\gamma(V\theta)_i|\le\epsilon\text{ for all }i.}
$$

## ↑ Ancestors (10)

1. [29J](../29j.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
