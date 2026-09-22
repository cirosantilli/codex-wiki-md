<h1 id="2/e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For real nonnegative envelopes, put $\Omega=\sqrt{\Omega_1^2+\Omega_2^2}$ and choose a continuous $\theta=\operatorname{atan2}(\Omega_1,\Omega_2)$. The state $|D\rangle=\cos\theta|1\rangle-\sin\theta|3\rangle$ is dark because its two amplitudes feeding $|2\rangle$ cancel: $\Omega_1\cos\theta-\Omega_2\sin\theta=0$. The orthogonal bright combination $|B\rangle=\sin\theta|1\rangle+\cos\theta|3\rangle$ couples to $|2\rangle$ with strength $\Omega$. Thus the other [eigenstates](../../../../../../../eigenstate.md) are $(|B\rangle\pm|2\rangle)/\sqrt2$ with energies $\pm\Omega$.

Start with $\Omega_1=0$ and $\Omega_2\ne0$, so $\theta=0$ and $|D\rangle=|1\rangle$. Slowly increase $\Omega_1/\Omega_2$ to infinity while maintaining a nonzero gap; end with $\Omega_2=0$ and $\Omega_1\ne0$, so $|D\rangle=-|3\rangle$. This target-to-intermediate pulse first is the counterintuitive ordering of [stimulated Raman adiabatic passage](../../../../../../../stimulated-raman-adiabatic-passage.md). Its quantitative slowness condition is

$$
\boxed{\hbar|\dot\theta|\ll\Omega,\qquad
\dot\theta=\frac{\Omega_2\dot\Omega_1-\Omega_1\dot\Omega_2}{\Omega_1^2+\Omega_2^2}.}
$$

It follows from $|\langle\pm|\dot D\rangle|=|\dot\theta|/\sqrt2$ and the gap $\Omega$. Avoid switching both envelopes off while $\theta$ is changing; switch off together only after the transfer angle has become stationary. The dark [eigenvalue](../../../../../../../eigenvalue.md) is zero, so there is no dynamical phase; with this real [eigenvector](../../../../../../../eigenvector.md) $\langle D|\dot D\rangle=0$ as well. The ideal [adiabatic quantum control](../../../../../../../adiabatic-quantum-control.md) therefore transfers $|1\rangle$ to $-|3\rangle$, physically the same target ray.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [E](../../e.md)
3. [2](../../../2.md)
4. [Paper 61](../../../../paper-61-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
