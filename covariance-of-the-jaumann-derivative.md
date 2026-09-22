# Covariance of the Jaumann derivative

↑ **Parent:** [Jaumann derivative](jaumann-derivative.md)

Use the derivative-index-first [velocity gradient](velocity-gradient.md) $G_{ij}=\partial_i u_j$ and $\omega=G-G^T$. For an [objective time derivative](objective-time-derivative.md) the [tensor](tensor.md) transformation $A^*=QAQ^T$ under $x^*=Q(t)x+c(t)$ must imply $\mathcal D A^*/\mathcal Dt=Q(\mathcal D A/\mathcal Dt)Q^T$. If $R=\dot Q Q^T$, then $G^*=QGQ^T-R$ and

$$
D_t A^*=Q(D_t A)Q^T+RA^*-A^*R,\qquad
\omega^*=Q\omega Q^T-2R.
$$

Consequently the extra terms cancel in $D_t A+\tfrac12(\omega A-A\omega)$, proving covariance. With the component-index-first gradient $L_{ij}=\partial_j u_i$, the same physical rate is $D_t A-WA+AW$, with [spin tensor](spin-tensor.md) $W=(L-L^T)/2=-\omega/2$. Changing the gradient convention without changing the commutator sign destroys objectivity.

## ↑ Ancestors (10)

1. [Jaumann derivative](jaumann-derivative.md)
2. [Objective time derivative](objective-time-derivative.md)
3. [Conformation tensor](conformation-tensor.md)
4. [Viscoelasticity](viscoelasticity.md)
5. [Non-Newtonian fluid](non-newtonian-fluid.md)
6. [Rheology](rheology-split.md)
7. [Fluid mechanics](fluid-mechanics-split.md)
8. [Branches of physics](branches-of-physics.md)
9. [Physics](physics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-342/2/a/solution.md)
