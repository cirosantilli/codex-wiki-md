<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use $\kappa=(\mu-r)/\sigma$ and $\gamma_M$ from Question 1, and take the finite-value case $\gamma_M>0$. After retirement the value is $V_M(w)=\gamma_M^{-R}w^{1-R}/(1-R)$. Working for an infinitesimal extra interval while using the retired portfolio and consumption produces a gain $\varepsilon V_M'(w)-\lambda$. Its zero is

$$
w_{\mathrm{myopic}}=\gamma_M^{-1}(\varepsilon/\lambda)^{1/R}.
$$

This proves **the instantaneous indifference level** appearing in the question. For the stated irreversible [optimal stopping](../../../../../optimal-stopping.md) problem it is generally a lower bound on the retirement boundary, rather than the boundary itself: retaining the opportunity to keep working has value. The following explicit [wealth-variable Legendre dual](../../../../../wealth-variable-legendre-dual.md) calculation exhibits the correction. In particular, imposing continuity of $V''$ at retirement would discard that option value; [smooth fit](../../../../../smooth-pasting.md) requires continuity of $V'$.

Assume the usual borrowing-against-income solvency condition: $w> -\varepsilon/r$ while working, with nonnegative wealth after retirement, and take $r>0$, $\rho>0$, $\kappa\ne0$. The question does not specify a tighter borrowing constraint. Let $J(z)=\sup_w\{V(w)-zw\}$, so $w=-J'(z)$ and $V=J-zJ'$. The working [Hamilton-Jacobi-Bellman equation](../../../../../hamilton-jacobi-bellman-equation.md) becomes the linear [Cauchy-Euler equation](../../../../../cauchy-euler-equation.md)

$$
\tfrac12\kappa^2z^2J''+(\rho-r)zJ'-\rho J+
\frac{R}{1-R}z^{1-1/R}+\varepsilon z-\lambda=0.
$$

The retired dual is $J_M(z)=Rz^{1-1/R}/[(1-R)\gamma_M]$. Let $m<0$ be the negative root of

$$
\tfrac12\kappa^2m(m-1)+(\rho-r)m-\rho=0.
$$

The other root exceeds one. Its growing term is excluded by the solvency asymptotic as $z\to\infty$. Therefore the working dual has the form

$$
J(z)=J_M(z)+\frac{\varepsilon}{r}z-\frac{\lambda}{\rho}+Dz^m.
$$

Retirement corresponds to $z\leq z_*$, where $J=J_M$. Value matching and [smooth fit](../../../../../smooth-pasting.md) give

$$
\frac{\varepsilon z_*}{r}-\frac{\lambda}{\rho}+Dz_*^m=0,\qquad
\frac{\varepsilon}{r}+Dmz_*^{m-1}=0.
$$

Consequently the [retirement boundary with an income option](../../../../../retirement-boundary-with-an-income-option.md) is

$$
\boxed{z_* =\frac{\lambda r}{\varepsilon\rho}\frac{m}{m-1},\qquad
D=-\frac{\varepsilon}{rm}z_*^{1-m}>0,\qquad
\overline w=\gamma_M^{-1}z_*^{-1/R}.}
$$

Using the root equation, $z_*/(\lambda/\varepsilon)=1+\kappa^2m/(2\rho)$, which lies strictly between zero and one. Thus $\overline w>w_{\mathrm{myopic}}$ for a nonzero risk premium. For example, $r=\rho=\varepsilon=\lambda=\kappa=1$ and $R=2$ give $m=-1$, $\gamma_M=9/8$, and

$$
\overline w=\frac{8\sqrt2}{9},\qquad w_{\mathrm{myopic}}=\frac89.
$$

These parameters give an explicit counterexample to identifying the printed level with the irreversible retirement boundary.

For $-\varepsilon/r<w<\overline w$, find the unique $z>z_*$ from

$$
w=\gamma_M^{-1}z^{-1/R}-\frac{\varepsilon}{r}-Dmz^{m-1}.
$$

This right side decreases strictly from $\overline w$ to $-\varepsilon/r$, since $J''>0$. Recover the value and controls by

$$
\boxed{V(w)=J(z)+zw,\qquad c^*(w)=z^{-1/R},\qquad
\theta^*(w)=\frac{\mu-r}{\sigma^2}zJ''(z).}
$$

For $w\geq\overline w$, retire immediately and use the Merton controls. Along the working strategy, $z_t$ satisfies $dz_t=(\rho-r)z_tdt-\kappa z_tdW_t$, and the optimal retirement time is its first hitting time of $z_*$, equivalently wealth's first hitting time of $\overline w$.

To check the [optimal stopping](../../../../../optimal-stopping.md) inequalities, write $h=J-J_M$. It satisfies $h(z_*)=h'(z_*)=0$ and $h''(z)=Dm(m-1)z^{m-2}>0$ for $z>z_*$. Hence continuation has positive option value there. On $z\leq z_*$ the stopping candidate has working residual $\varepsilon z-\lambda\leq0$. The matched dual is continuously differentiable, so the [Itô formula](../../../../../ito-s-lemma.md) introduces no boundary local-time term. Localization, the state-price budget, and the appropriate infinite-horizon transversality justify verification.

If nonnegative financial wealth is imposed during employment as an additional constraint, the working dual also has an upper boundary, and that extra constraint must be included in the free-boundary problem. It cannot be recovered by assuming the printed myopic equality.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
