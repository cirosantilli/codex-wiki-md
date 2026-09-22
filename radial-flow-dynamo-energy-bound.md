# Radial-flow dynamo energy bound

↑ **Parent:** [Dynamo action](dynamo-action.md)

Let a [solenoidal](solenoidal-vector-field.md) flow be confined to a sphere $V$, with the [insulating boundary condition for the radial magnetic scalar](insulating-boundary-condition-for-the-radial-magnetic-scalar.md). Define $N=\int_VP^2$, $D=\int_{\mathbb R^3}|\nabla P|^2$, $M=\int_{\mathbb R^3}|\mathbf B|^2$ and $q=\max_V|\mathbf u\cdot\mathbf x|$. [Integration by parts](integration-by-parts.md) inside and outside the sphere gives

$$
\frac12N'=-\int_VQ\,\mathbf B\cdot\nabla P-\eta D\leq q\sqrt{MD}-\eta D.
$$

The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) therefore makes $q^2\geq\eta^2D/M$ necessary whenever $N'\geq0$ and $D>0$. A uniform strict violation with a positive gap forces decay, using a [Sobolev inequality](sobolev-inequality.md) to bound $N$ by a constant times $D$. A bounded statistically steady field instead requires $q_*^2\geq\eta^2\langle D\rangle/\langle M\rangle$, with $q_*=\sup_tq(t)$. This is a necessary condition for [dynamo action](dynamo-action.md), not a sufficient criterion or a pointwise assertion at every instant of an arbitrary time-dependent solution.

// Target: analysis.bigb

## ↑ Ancestors (8)

1. [Dynamo action](dynamo-action.md)
2. [Resistive magnetohydrodynamics](resistive-magnetohydrodynamics.md)
3. [Magnetohydrodynamics](magnetohydrodynamics.md)
4. [Astrophysical fluid dynamics](astrophysical-fluid-dynamics-split.md)
5. [Fluid mechanics](fluid-mechanics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-74/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-74/1/iii/solution.md)
- [Poloidal magnetic energy bound by the radial scalar gradient](poloidal-magnetic-energy-bound-by-the-radial-scalar-gradient.md)
