# Slow and fast limits of a delayed stem-cell model

↑ **Parent:** [Stem cell](stem-cell.md)

For resting-cell recruitment $g(u)=bu/(1+u^n)$, a positive constant [equilibrium](equilibrium-point-of-a-dynamical-system.md) exists precisely when $\mu b>1$, with $u_*=(\mu b-1)^{1/n}$. On slow time $T=\epsilon t$, expand the delayed value as $u(T-\epsilon)=u-\epsilon u_T+O(\epsilon^2)$. Substitution gives $(1+g'(u))u_T=\mu g(u)-u$ to leading order. This reduction requires smooth slow motion and $1+g'(u)$ bounded away from zero.

On the original fast time, only the explicit order-$\epsilon$ terms are dropped, leaving $u'=g(u(t-1))-g(u(t))$. The unit delay remains order one and cannot be Taylor-expanded on that scale. For the biological two-compartment derivation, a fixed cell-cycle time $\tau$ and proliferating death hazard $\gamma_d$ give survival $e^{-\gamma_d\tau}$ and daughter-cell gain twice the surviving exit rate. Scaling gives $b=\beta_0\tau$, $\epsilon=\delta\tau$ and $1+\epsilon\mu=2e^{-\gamma_d\tau}$. Thus small resting-cell loss over one cycle creates the slow-fast structure.

## ↑ Ancestors (4)

1. [Stem cell](stem-cell.md)
2. [Biological cell](biological-cell-split.md)
3. [Biology](biology-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-and-the-environment-and-mathematical-physiology-course-of-the-university-of-oxford/2008/b/8/solution.md)
