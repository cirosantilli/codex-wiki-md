<h1 id="33a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

To first order in $F$, [time-dependent perturbation theory](../../../../../../time-dependent-perturbation-theory.md) replaces the state on the right-hand side by its unperturbed value $e^{-iE_0t/\hbar}|0\rangle$. The bound state is even, while the [position operator](../../../../../../position-operator.md) $x$ is odd. The [parity](../../../../../../parity.md) selection rule therefore gives

$$
\langle k,+|x|0\rangle=0,
$$

so $\dot b_k=0$ and, with no initial continuum component,

$$
\boxed{b_k(t)=0}.
$$

Projection onto the odd state gives

$$
\dot c_k(t)
=\frac{iF}{\hbar}\langle k,-|x|0\rangle
e^{i(E_k-E_0-\hbar\omega)t/\hbar}.
$$

Writing $\Omega_k=(E_k-E_0-\hbar\omega)/\hbar$ and integrating from zero to $t$ yields

$$
\boxed{
c_k(t)=\frac{iF}{\hbar}\langle k,-|x|0\rangle
e^{i\Omega_kt/2}
\frac{\sin(\Omega_kt/2)}{\Omega_k/2}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [33A](../../33a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
