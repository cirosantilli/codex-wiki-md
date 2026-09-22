<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

[Moser's trick](../../../../../moser-s-trick.md) states that if $M$ is compact and $\omega_t$, $0\leq t\leq1$, is a smooth family of [symplectic forms](../../../../../symplectic-form.md) whose [de Rham cohomology](../../../../../de-rham-cohomology.md) class is independent of $t$, then there is an [isotopy](../../../../../isotopy.md) $\phi_t$ with

$$
\phi_t^*\omega_t=\omega_0.
$$

Since $[\dot\omega_t]=0$, choose a smooth family of one-forms $\sigma_t$ with $\dot\omega_t=d\sigma_t$. Nondegeneracy of $\omega_t$ uniquely determines a vector field $X_t$ by

$$
\iota_{X_t}\omega_t=-\sigma_t.
$$

Compactness makes its flow $\phi_t$ exist for the whole interval. [Cartan's magic formula](../../../../../cartan-s-magic-formula.md) and $d\omega_t=0$ give

$$
\frac d{dt}\phi_t^*\omega_t
=\phi_t^*(\dot\omega_t+\mathcal L_{X_t}\omega_t)
=\phi_t^*(d\sigma_t+d\iota_{X_t}\omega_t)=0,
$$

which proves the theorem.

Smooth degree-$d$ hypersurfaces form the complement of the discriminant in the projective space of degree-$d$ homogeneous polynomials. This complement is path connected, so $X$ and $X'$ lie in a smooth one-parameter family. The [Ehresmann fibration theorem](../../../../../ehresmann-fibration-theorem.md) identifies the fibers smoothly. Under such an identification, the restrictions of the [Fubini-Study form](../../../../../fubini-study-form.md) form a family $\omega_t$ whose cohomology class is the fixed restricted hyperplane class. Moser's trick therefore gives the [symplectic equivalence of smooth projective hypersurfaces](../../../../../symplectic-equivalence-of-smooth-projective-hypersurfaces.md).

It remains to construct the finite subgroup for one convenient hypersurface. On the [Fermat hypersurface](../../../../../fermat-hypersurface.md)

$$
X_F=\{z_0^d+\cdots+z_n^d=0\}\subset\mathbb{CP}^n,
$$

the group $(\mu_d)^{n+1}$ acts by diagonal coordinate multiplication. It preserves both $X_F$ and the Fubini-Study form. The kernel of its projective action is the diagonal subgroup $\mu_d$, so the effective [Fermat hypersurface diagonal symmetry](../../../../../fermat-hypersurface-diagonal-symmetry.md) group is

$$
(\mathbb Z/d\mathbb Z)^{n+1}/\langle(1,\ldots,1)\rangle
\cong(\mathbb Z/d\mathbb Z)^n.
$$

Conjugating this action by a symplectomorphism $X_F\to X$ gives the required subgroup of $\operatorname{Symp}(X,\omega_{FS}|_X)$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 146](../../paper-146-split.md)
3. [Iii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
