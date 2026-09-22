<h1 id="34b/solution">Solution</h1>

↑ **Parent:** [34B](../34b.md)

For a nonzero normalized or unnormalized trial function in the Hamiltonian's quadratic-form domain, the [Rayleigh-Ritz variational principle](../../../../../rayleigh-ritz-variational-principle.md) gives $E_0\leq\langle\psi,H\psi\rangle/\langle\psi,\psi\rangle$. Expanding in energy eigenstates, or using the spectral measure, makes the quotient a weighted average of spectral energies, all at least $E_0$. For an even one-dimensional potential, the [ground state](../../../../../ground-state.md) is even and the first excited [bound state](../../../../../bound-state.md) is odd by the nodal ordering theorem. Restricting to odd trial functions therefore gives an upper bound on the lowest odd energy and on $E_1$ when that [bound state](../../../../../bound-state.md) exists; a negative odd quotient also certifies its existence.

Here $\hbar^2/(2m)=1$. For the Gaussian trial function, [integration by parts](../../../../../integration-by-parts.md) gives kinetic quotient $\int|\psi'|^2/\int|\psi|^2=a/2$, and the potential quotient is $-V_0\sqrt{a/(1+a)}$. Therefore

$$
\boxed{E_0\leq E(a)=\frac a2-V_0\sqrt{\frac a{1+a}}.}
$$

For $a>0$, its zero obeys $a(1+a)=4V_0^2$, giving the unique positive zero

$$
\boxed{a_z=\frac{\sqrt{1+16V_0^2}-1}{2}.}
$$

Also $E'(a)=1/2-V_0/[2\sqrt a(1+a)^{3/2}]$, so its stationary points satisfy $a(1+a)^3=V_0^2$. The left side increases strictly from zero to infinity, proving that there is exactly one stationary point, a minimum.

<a id="34b/image-gaussian-variational-energy-with-its-negative-minimum-and-positive-zero"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-1-gaussian-variational-bound.png)

**[Figure 2](#34b/image-gaussian-variational-energy-with-its-negative-minimum-and-positive-zero). Gaussian variational energy with its negative minimum and positive zero**.

As $a\downarrow0$, $E(a)=-V_0\sqrt a+O(a)$ approaches zero from below; as $a\to\infty$, it tends to infinity. The sketch and variational inequality therefore give a negative energy for every $V_0>0$. Since this decaying potential has [essential spectrum](../../../../../essential-spectrum-of-a-closed-operator.md) beginning at zero, **at least one [bound state](../../../../../bound-state.md) exists for every positive well depth**.

For small $V_0$, the minimizer is $a_*=V_0^2-3V_0^4+O(V_0^6)$. Substitution gives $E(a_*)=-V_0^2/2+V_0^4/2+O(V_0^6)$. Meanwhile the potential is strictly greater than $-V_0$ except at a single point and the [kinetic energy](../../../../../kinetic-energy.md) is nonnegative, so a normalized bound-state expectation is strictly greater than $-V_0$. Thus

$$
\boxed{-V_0<E_0\leq\epsilon(V_0),\qquad
\epsilon(V_0)=-\frac12V_0^2+O(V_0^4).}
$$

## ↑ Ancestors (10)

1. [34B](../34b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
