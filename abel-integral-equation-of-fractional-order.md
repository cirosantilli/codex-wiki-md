# Abel integral equation of fractional order

↑ **Parent:** [Abel integral equation](abel-integral-equation.md)

For an absolutely continuous $f$ with $f(0)=0$, this causal [Abel integral equation](abel-integral-equation.md) has inversion

$$
\Phi(t)=\frac1{\Gamma(\alpha)\Gamma(1-\alpha)}\int_0^tf'(\tau)(t-\tau)^{\alpha-1}d\tau.
$$

Under Laplace-transform growth hypotheses, the [convolution theorem for Laplace transforms](convolution-theorem-for-laplace-transforms.md) converts the original kernel into $\Gamma(1-\alpha)s^{\alpha-1}$. Since $\mathcal L[f']=s\mathcal L[f]$, the transformed inverse is $s^{-\alpha}\mathcal L[f']/\Gamma(1-\alpha)$, giving the formula. It also holds locally in the corresponding integrable convolution class: convolving the two power kernels produces the constant $B(\alpha,1-\alpha)=\Gamma(\alpha)\Gamma(1-\alpha)$ by the [beta-gamma identity](beta-gamma-identity.md), so substitution recovers $\int_0^tf'=f(t)$. The same convolution identity proves uniqueness in that class. For example $f(t)=t$ gives $\Phi=t^\alpha/[\Gamma(\alpha+1)\Gamma(1-\alpha)]$.

## ↑ Ancestors (6)

1. [Abel integral equation](abel-integral-equation.md)
2. [Integral equation](integral-equation.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2009/paper-2/5/solution.md)
