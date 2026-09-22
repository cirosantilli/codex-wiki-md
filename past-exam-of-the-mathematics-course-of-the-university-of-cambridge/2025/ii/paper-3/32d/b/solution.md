<h1 id="32d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let

$$
H=-\partial_x^2-2\chi^2\operatorname{sech}^2(\chi x),
\qquad
A=\partial_x+\chi\tanh(\chi x).
$$

On $L^2(\mathbb R)$, $A^\dagger=-\partial_x+\chi\tanh(\chi x)$. The [supersymmetric factorization of the one-soliton potential](../../../../../../supersymmetric-factorization-of-the-one-soliton-potential.md) is

$$
A^\dagger A=H+\chi^2,
\qquad
AA^\dagger=-\partial_x^2+\chi^2.
$$

In particular, $A^\dagger A$ is nonnegative, so every eigenvalue of $H$ satisfies

$$
E\geq-\chi^2.
$$

Equality is attained precisely when $A\psi=0$. Solving that first-order equation gives

$$
\psi_0(x)=C\operatorname{sech}(\chi x),
$$

which is square-integrable. With unit normalization, $C=\sqrt{\chi/2}$, and

$$
H\psi_0=-\chi^2\psi_0.
$$

It remains to exclude another bound state. Since this [Pöschl-Teller potential](../../../../../../poschl-teller-potential.md) tends to zero at infinity, a bound-state energy must have $E<0$. If $H\psi=E\psi$, then applying $A$ to

$$
A^\dagger A\psi=(E+\chi^2)\psi
$$

gives

$$
-\partial_x^2(A\psi)=E(A\psi).
$$

The free one-dimensional Schrodinger operator has no nonzero square-integrable eigenfunction with $E<0$. Consequently $A\psi=0$, and the state must be proportional to $\psi_0$. Thus there is exactly one bound state, with

$$
\boxed{E_0=-\chi^2}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [32D](../../32d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
