<h1 id="34d/solution">Solution</h1>

↑ **Parent:** [34D](../34d.md)

The classical one-particle [partition function](../../../../../canonical-partition-function.md), with phase-space cell $h^3$, is

$$
Z_1=\frac1{h^3}\int d^3p\,d^3x\,
e^{-[p^2/(2m)+U(x)]/(kT)}
=\left(\frac{2\pi mkT}{h^2}\right)^{3/2}
\int e^{-U/(kT)}\,d^3x.
$$

For the homogeneous trap, rescale $r=V^{1/3}(kT)^{1/(2n)}u$. The spatial measure contributes $V(kT)^{3/(2n)}$, so

$$
\boxed{Z_1=VI_n(kT)^a,\qquad
a=\frac32+\frac3{2n}=\frac{3(n+1)}{2n}}.
$$

Here $I_n=(2m\pi/h^2)^{3/2}\int_0^\infty4\pi u^2e^{-u^{2n}}\,du$, as specified; the last integral is $2\pi\Gamma(3/(2n))/n$.

Using the printed convention $Z_N=Z_1^N$, the [free energy](../../../../../thermodynamic-free-energy.md) is

$$
\boxed{F=-NkT[\log V+a\log(kT)+\log I_n]}.
$$

This convention treats the particles as labeled. For indistinguishable classical particles, $Z_N=Z_1^N/N!$ adds $kT\log N!$ to $F$. It changes the [entropy](../../../../../entropy.md) by $-k\log N!$ but leaves the following force, [energy](../../../../../energy.md) and [heat capacities](../../../../../heat-capacity.md) unchanged. This normalization qualification is required to distinguish the printed expression from the usual Gibbs-corrected gas [free energy](../../../../../thermodynamic-free-energy.md).

The generalized force conjugate to the external parameter $V$ is $P=-(\partial F/\partial V)_T$, hence

$$
\boxed{P=\frac{NkT}{V},\qquad PV=NkT}.
$$

It is the same equation of state as a hard-wall ideal gas, although $V$ now dilates a soft confining potential rather than being the occupied geometric volume.

Writing $L=\log V+a\log(kT)+\log I_n$, thermodynamic differentiation gives

$$
\boxed{S=Nk(L+a),\qquad E=F+TS=aNkT,\qquad C_V=aNk}.
$$

The mean [kinetic energy](../../../../../kinetic-energy.md) is $3NkT/2$ and the trap potential contributes $3NkT/(2n)$. At fixed $P$, $V=NkT/P$, so $\partial_TL|_P=(a+1)/T$. Consequently

$$
\boxed{C_P=T(\partial S/\partial T)_P=(a+1)Nk=C_V+Nk}.
$$

The same result follows from [enthalpy](../../../../../enthalpy.md) $E+PV=(a+1)NkT$. These identities describe the [classical ideal gas in a homogeneous soft trap](../../../../../classical-ideal-gas-in-a-homogeneous-soft-trap.md).

## ↑ Ancestors (10)

1. [34D](../34d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
