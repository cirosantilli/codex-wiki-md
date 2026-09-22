<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $f_s=(-1)^{1/2-s}$ for $s=\pm1/2$, so $f_{-s}=-f_s$. Under the [antiunitary operator](../../../../../../antiunitary-operator.md) $\hat T$, the coefficients and exponentials in the [mode expansion of a Dirac field](../../../../../../mode-expansion-of-a-dirac-field.md) are conjugated as well as the [creation and annihilation operators](../../../../../../creation-and-annihilation-operators.md) being transformed. Thus

$$
\hat T\psi(x)\hat T^{-1}=\sum_{p,s}f_s\left[b^{-s}(p_T)u^{s*}(p)e^{ip\cdot x}+d^{-s\dagger}(p_T)v^{s*}(p)e^{-ip\cdot x}\right].
$$

Relabel $q=p_T$ and $r=-s$. The stated [Dirac spinor](../../../../../../dirac-spinor.md) identities imply

$$
f_{-r}u^{-r*}(q_T)=-\gamma^5Cu^r(q),\qquad f_{-r}v^{-r*}(q_T)=-\gamma^5Cv^r(q).
$$

Also $q_T\cdot x=-q\cdot x_T$. Substitution reconstructs the original [Dirac field](../../../../../../dirac-field.md) at the reflected time:

$$
\boxed{\hat T\psi(x)\hat T^{-1}=B\psi(x_T),\qquad B=-\gamma^5C.}
$$

The minus sign comes from reversing the spin label, not from anticommuting field operators. This is the relation between the time-reversal matrix and the [charge-conjugation matrix](../../../../../../charge-conjugation-matrix.md) in the supplied spin phases and intrinsic phase convention. Rephasing the [charge-conjugation matrix](../../../../../../charge-conjugation-matrix.md) or the intrinsic time-reversal phase can change its displayed form. It proves [time reversal of a Dirac field](../../../../../../time-reversal-of-a-dirac-field.md) without identifying an [antiunitary operator](../../../../../../antiunitary-operator.md) with its finite-dimensional spinor matrix.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 305](../../../paper-305-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
