<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For constant [barotropic equation of state](../../../../../../barotropic-equation-of-state.md) $P=w\rho$, the [cosmological perfect-fluid continuity equation](../../../../../../cosmological-perfect-fluid-continuity-equation.md) gives $\bar\rho\propto a^{-3(1+w)}$. In conformal time the flat [Friedmann equation](../../../../../../friedmann-equations.md) becomes $\mathcal H^2=(8\pi G/3)a^2\bar\rho$, where $\mathcal H=a'/a$. Integration, for $w\ne-1/3$, gives

$$
\boxed{a\propto|\eta-\eta_B|^{2/(1+3w)},\qquad a^2\bar\rho\propto(\eta-\eta_B)^{-2}.}
$$

Choose the conformal-time origin so that $\eta_B=0$ and work on the appropriate expansion branch. Write $\beta=2/(1+3w)$, so $\mathcal H=\beta/\eta$ and $2\mathcal H'+(1+3w)\mathcal H^2=0$.

Combining the supplied energy and momentum constraints gives the [comoving-gauge density contrast](../../../../../../comoving-gauge-density-contrast.md) Poisson relation

$$
\nabla^2\phi=4\pi Ga^2\bar\rho[\delta-3\mathcal H(1+w)v]
=4\pi Ga^2\bar\rho\Delta.
$$

For this barotropic fluid $\delta P=w\bar\rho\delta$. Substitute the energy constraint into the pressure equation to obtain

$$
\phi''+3(1+w)\mathcal H\phi'
+[2\mathcal H'+(1+3w)\mathcal H^2]\phi-w\nabla^2\phi=0,
$$

so the bracket vanishes and the coefficient of $\phi'/\eta$ is $A=6(1+w)/(1+3w)$.

Because $a^2\bar\rho=C\eta^{-2}$, the Poisson relation gives $\Delta=(\eta^2/(4\pi GC))\nabla^2\phi$. Apply the same potential equation to $F=\eta^2\nabla^2\phi$: differentiating $\eta^{-2}F$ gives

$$
F''+\frac{A-4}{\eta}F'+\frac{6-2A}{\eta^2}F-w\nabla^2F=0.
$$

Since $F$ is a constant multiple of $\Delta$, the [constant-equation-of-state comoving density equation](../../../../../../constant-equation-of-state-comoving-density-equation.md) is

$$
\boxed{\Delta''+\frac{2(1-3w)}{(1+3w)\eta}\Delta'
-\frac{6(1-w)}{(1+3w)\eta^2}\Delta-w\nabla^2\Delta=0.}
$$

The primes here denote conformal-time derivatives, corresponding to the overdots in the question. A pure vacuum fluid $w=-1$ has zero enthalpy and no independent fluid velocity or nonzero-wave-number density perturbation; its formal equation should be interpreted with that degeneracy in mind.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
