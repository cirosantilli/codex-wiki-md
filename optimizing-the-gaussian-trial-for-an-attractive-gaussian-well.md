# Optimizing the Gaussian trial for an attractive Gaussian well

↑ **Parent:** [Gaussian variational bound for an attractive Gaussian well](gaussian-variational-bound-for-an-attractive-gaussian-well.md)

For $E(a)=a/2-V_0\sqrt{a/(1+a)}$ with $a,V_0>0$, differentiation gives $E'(a)=1/2-V_0/[2\sqrt a(1+a)^{3/2}]$. The positive stationarity equation has a unique solution because its left side increases strictly. Moreover $E''(a)=V_0(1+4a)/[4a^{3/2}(1+a)^{5/2}]>0$, so it is the global minimum. Substituting the stationarity equation gives the displayed negative energy. The only positive zero is $(\sqrt{1+16V_0^2}-1)/2$; $a=0$ is only a limiting zero, since the limiting constant trial is not a [square-integrable function](square-integrable-function.md). The [Rayleigh-Ritz variational principle](rayleigh-ritz-variational-principle.md) therefore proves a negative-energy [bound state](bound-state.md) for every positive well depth. For weak depth, the simpler choice $a=V_0^2$ yields an explicit upper bound $E_0\leq-V_0^2/2+\varepsilon$ with

$$
\varepsilon=\frac{V_0^4}{\sqrt{1+V_0^2}(\sqrt{1+V_0^2}+1)}=\frac12V_0^4+O(V_0^6).
$$

This is a variational upper bound, not an equality for the exact weak-depth coefficient.

## ↑ Ancestors (9)

1. [Gaussian variational bound for an attractive Gaussian well](gaussian-variational-bound-for-an-attractive-gaussian-well.md)
2. [Rayleigh-Ritz variational principle](rayleigh-ritz-variational-principle.md)
3. [Rayleigh quotient](rayleigh-quotient.md)
4. [Operator theory](linear-operator-theory-split.md)
5. [Linear algebra](linear-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
