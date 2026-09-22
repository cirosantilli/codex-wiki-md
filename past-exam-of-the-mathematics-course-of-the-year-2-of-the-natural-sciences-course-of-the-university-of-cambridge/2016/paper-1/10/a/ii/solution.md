<h1 id="10/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume $H$ is [self-adjoint](../../../../../../self-adjoint-operator.md) on its specified [operator domain](../../../../../../operator-domain.md), and the admissible variations preserve that domain and any [boundary conditions](../../../../../../boundary-condition.md), so no boundary terms spoil self-adjointness. Let $N=\langle\phi,\phi\rangle>0$. The first variation of the [Rayleigh quotient](../../../../../../rayleigh-quotient.md) is

$$
\delta F=\frac{\langle\delta\phi,(H-F[\phi])\phi\rangle+\langle(H-F[\phi])\phi,\delta\phi\rangle}{N}=\frac{2\operatorname{Re}\langle\delta\phi,(H-F[\phi])\phi\rangle}{N}.
$$

At $\phi=\psi_n$, the residual vanishes, so $\boxed{\delta F[\psi_n]=0}$. More explicitly, for a normalized $\psi_n$ and $\phi=\psi_n+\eta$,

$$
F[\psi_n+\eta]-E_n=\frac{\langle\eta,(H-E_n)\eta\rangle}{1+2\operatorname{Re}\langle\psi_n,\eta\rangle+\|\eta\|^2}.
$$

For a fixed admissible direction scaled by a small parameter, the change is second order. This is stationarity, and is not necessarily a minimum for an excited state.

Conversely, vanishing first variation for every admissible complex direction yields the stationary equation

$$
\boxed{(H-F[\phi])\phi=0\quad\text{at a stationary }\phi.}
$$

At the original stationary point, this is $(H-F[\psi_n])\psi_n=0$. **The printed equation with an arbitrary perturbed $\phi$ in the final factor is not generally true.** Taking $\phi=\psi_n+\epsilon\psi_m$ with $E_m\neq E_n$ gives $(H-E_n)\phi=\epsilon(E_m-E_n)\psi_m\neq0$, even though the first-order change in $F$ is zero. Thus the valid claim is the stationary equation at the extremal state, not an exact [eigenvalue](../../../../../../eigenvalue.md) equation for every variation.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [10](../../../10.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
