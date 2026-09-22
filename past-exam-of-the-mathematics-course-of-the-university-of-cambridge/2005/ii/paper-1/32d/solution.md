<h1 id="32d/solution">Solution</h1>

↑ **Parent:** [32D](../32d.md)

The commutator gives $a(a^\dagger)^n=(a^\dagger)^na+n(a^\dagger)^{n-1}$. Hence $a|n\rangle=\sqrt n|n-1\rangle$ and $a^\dagger|n\rangle=\sqrt{n+1}|n+1\rangle$. Starting with the normalized vacuum, repeated application gives $\langle0|a^n(a^\dagger)^n|0\rangle=n!$, proving unit norm. The [number operator](../../../../../number-operator.md) then has [eigenvalue](../../../../../eigenvalue.md) $n$, so

$$
\boxed{E_n=\hbar\omega(n+\tfrac12).}
$$

Different levels are orthogonal because the [Hamiltonian](../../../../../hamiltonian.md) is self-adjoint and their [eigenvalues](../../../../../eigenvalue.md) are distinct.

For the perturbation, the ground-state diagonal [matrix](../../../../../matrix.md) element is zero, while $V|0\rangle=\hbar\omega\sqrt{r!}|r\rangle$. The nondegenerate second-order perturbation formula consequently gives

$$
\boxed{\Delta E_0=-\lambda^2\hbar\omega\frac{r!}{r}+O(\lambda^3)=-\lambda^2\hbar\omega(r-1)!+O(\lambda^3).}
$$

For $r=1$, $V|1\rangle=\hbar\omega(|0\rangle+\sqrt2|2\rangle)$. The lower and upper intermediate levels contribute respectively $+\lambda^2\hbar\omega$ and $-2\lambda^2\hbar\omega$, giving **$\Delta E_1=-\lambda^2\hbar\omega$ to second order**.

For $r=1$ the exact completion of the square is

$$
H_\lambda=\hbar\omega\left[(a^\dagger+\lambda)(a+\lambda)+\tfrac12-\lambda^2\right].
$$

The shifted operators $b=a+\lambda$, $b^\dagger=a^\dagger+\lambda$ have the same commutator and are unitarily related to the original ones by a displacement operator. Their vacuum is the [coherent state](../../../../../coherent-state.md) with amplitude $-\lambda$. Therefore **every exact level shifts by $-\lambda^2\hbar\omega$**.

The [stability of monomial ladder-operator perturbations](../../../../../stability-of-monomial-ladder-operator-perturbations.md) gives a necessary qualification to the request for a lowest level for every $r$. For $r>2$ and real nonzero $\lambda$, a [coherent state](../../../../../coherent-state.md) of amplitude $Re^{i\theta}$ has [energy](../../../../../energy.md) expectation $\hbar\omega[R^2+1/2+2\lambda R^r\cos(r\theta)]$. Choose the phase so the last term is negative. As $R\to\infty$ the expectation tends to minus infinity, so the perturbed [Hamiltonian](../../../../../hamiltonian.md) has no true ground state. The displayed second-order answer is then the formal perturbative coefficient of the branch from the unperturbed vacuum, not an exact lowest [eigenvalue](../../../../../eigenvalue.md). For $r=2$ [stability](../../../../../stability-of-a-numerical-method.md) requires $|\lambda|<1/2$; for $r=1$ the completed-square [Hamiltonian](../../../../../hamiltonian.md) is bounded below for every real $\lambda$.

## ↑ Ancestors (10)

1. [32D](../32d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
