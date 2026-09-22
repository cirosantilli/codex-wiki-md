# Two-length machine compliance separation

↑ **Parent:** [Machine compliance](machine-compliance.md)

Prepare two uniform specimens with the same material, direction and $A_0$, but different deforming lengths $L_1,L_2$. Keep grip engagement, adapters, loading window and measurement configuration equivalent. Determine $q_i=dx_i/dF$ separately by [linear regression](linear-regression-split.md) with its own displacement intercept. Subtracting the two series equations eliminates the common [machine compliance](machine-compliance.md):

$$
q_2-q_1=\frac{L_2-L_1}{EA_0},\qquad
E=\frac{L_2-L_1}{A_0(q_2-q_1)},\qquad
C_m=\frac{L_2q_1-L_1q_2}{L_2-L_1}.
$$

This is an [inverse problem](inverse-problem-split.md): one length supplies only one equation for two unknowns, while two distinct lengths separate the length-dependent specimen contribution from the constant contribution. In a graph of compliance against length, the slope is $1/(EA_0)$ and the vertical intercept is $C_m$. It is the compliance, not $k_{\mathrm{obs}}$, that is linear in $L$.

The [dimensional analysis](dimensional-analysis.md) is revealing: $[q_2-q_1]=\mathrm{m/N}$, so $[(L_2-L_1)/(A_0(q_2-q_1))]=\mathrm{N/m^2}$. For $L_2>L_1$, the ideal model requires $q_2>q_1$. A negative fitted $C_m$ challenges the common-intercept assumptions or the measurements. Two lengths determine two parameters exactly, so they cannot test the assumed straight line; three or more lengths allow [regression residuals](regression-residual.md) to reveal departures. Nearly equal lengths amplify slope errors through the small difference $q_2-q_1$. If the actual apparatus compliances differ by $\Delta C_m$, the inferred length slope becomes $1/(EA_0)+\Delta C_m/(L_2-L_1)$.

**Table of contents**

- [Worked two-length tensile compliance example](worked-two-length-tensile-compliance-example.md)

## ↑ Ancestors (9)

1. [Machine compliance](machine-compliance.md)
2. [Tensile modulus experiment](tensile-modulus-experiment.md)
3. [Young's modulus](young-s-modulus.md)
4. [Linear elasticity](linear-elasticity.md)
5. [Elasticity (physics)](elasticity-physics-split.md)
6. [Continuum mechanics](continuum-mechanics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Machine compliance](machine-compliance.md)
