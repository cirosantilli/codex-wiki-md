<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Differentiating the assumed primitive identity and using [Cartan's magic formula](../../../../../../cartan-s-magic-formula.md) gives

$$
d\dot F_t=\rho_t^*\mathcal L_{X_t}\lambda
=\rho_t^*\bigl(d(\iota_{X_t}\lambda)-\iota_{X_t}\omega\bigr).
$$

Apply the [pullback of a differential form](../../../../../../pullback-of-a-differential-form.md) by $\rho_t^{-1}$ and rearrange:

$$
\boxed{\iota_{X_t}\omega=dH_t,\qquad
H_t=\iota_{X_t}\lambda-\dot F_t\circ\rho_t^{-1}.}
$$

This smooth family of [Hamiltonian functions](../../../../../../hamiltonian-function.md) proves that $\rho_t$ is a [Hamiltonian isotopy](../../../../../../hamiltonian-isotopy.md) in the convention of part (b).

To connect this with the preceding assertion that every $\rho_t^*\lambda-\lambda$ is an [exact differential form](../../../../../../exact-differential-form.md), the smooth choice of primitives causes no additional obstruction. Fix $p_0\in M$ and normalize $F_t(p_0)=0$. Define $F_t(p)$ by the [line integral](../../../../../../line-integral.md) of $\rho_t^*\lambda-\lambda$ from $p_0$ to $p$. The [fundamental theorem for line integrals](../../../../../../fundamental-theorem-for-line-integrals.md) makes this independent of the path. Near any $p$, use one fixed path to a nearby chart center followed by coordinate line segments; this expression is smooth jointly in $t,p$. Thus these normalized primitives form the required smooth family.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 140](../../../paper-140-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
