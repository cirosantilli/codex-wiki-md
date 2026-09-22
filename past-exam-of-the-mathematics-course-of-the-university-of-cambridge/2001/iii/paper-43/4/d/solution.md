<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $T_0=T_i-T_\infty>0$, $S_0=S_i-S_\infty>0$ and $R_0=\beta S_0/(\alpha T_0)$. At steady volume, the weir outflow equals the inflow $Q$. The well-mixed [heat](../../../../../../heat.md) and salt balances give

$$
Q(T_i-T)=AF_T,\qquad Q(S_i-S)=AF_S.
$$

With $\theta=(T_i-T)/T_0$ and $\eta=(S_i-S)/S_0$, the flux ratio implies **$\eta_s=q\theta_s$**, where $q=R_F/R_0$. The actual interface ratios are $\Delta T=T_0(1-\theta)$, $\Delta S=S_0(1-\eta)$ and $R_\rho=R_0(1-\eta)/(1-\theta)$.

The original PDF uses $R_\rho^{-2}$ in the heat-flux law; the converted TeX's exponent $-3$ is a transcription error. Using the PDF yields

$$
F_T=\frac{b\alpha^{1/3}T_0^{4/3}}{R_0^2}
\frac{(1-\theta)^{10/3}}{(1-\eta)^2}.
$$

Substitute this into the heat balance to obtain the [double-diffusive overflow reservoir](../../../../../../double-diffusive-overflow-reservoir.md) relations

$$
\boxed{\eta_s=\frac{R_F}{R_0}\theta_s,\qquad
\theta_s=C\frac{(1-\theta_s)^{10/3}}{(1-\eta_s)^2},\qquad
C=\frac{Ab(\alpha T_0)^{1/3}}{Q R_0^2}.}
$$

For the usual heat-dominated positive upward [buoyancy flux](../../../../../../buoyancy-flux.md), $0\leq R_F<1$ and $R_0>1$ give $0\leq q<1$. Then the right-hand side after substituting $\eta_s=q\theta_s$ decreases from $C$ to zero as $\theta_s$ runs from zero to one; there is a unique physical steady root. The net upward [buoyancy flux](../../../../../../buoyancy-flux.md) is $B_0=g\alpha F_T(1-R_F)$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
