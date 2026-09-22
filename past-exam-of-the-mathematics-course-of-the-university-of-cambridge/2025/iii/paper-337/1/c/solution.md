<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $H|n\rangle=E_n|n\rangle$, $\beta=1/T$, $Z=\sum_ne^{-\beta E_n}$, and $A_{nm}=\langle n|A|m\rangle$. Inserting two energy resolutions into the commutator and carrying out the one-sided Fourier integral gives the [Lehmann representation](../../../../../../lehmann-representation.md)

$$
\boxed{
G_{AA}^R(\omega)=\frac1Z\sum_{n,m}
\frac{(e^{-\beta E_n}-e^{-\beta E_m})A_{nm}A_{mn}}
{\omega+E_n-E_m+i0^+}.}
$$

If the trace in the question is intentionally unnormalized, the same formula holds without $1/Z$.

For $H=\varepsilon a^\dagger a$,

$$
a^\dagger(t)=e^{i\varepsilon t}a^\dagger.
$$

Therefore

$$
[a^\dagger(t),a^\dagger(0)]=0
$$

and the Green function requested literally for $A=a^\dagger$ is

$$
\boxed{G_{a^\dagger a^\dagger}^R(\omega)=0.}
$$

Physically, a number-conserving oscillator has no anomalous response connecting two creation operators. The nonzero normal retarded propagator pairs annihilation with creation: $G_{aa^\dagger}^R(\omega)=1/(\omega-\varepsilon+i0^+)$, whose pole is the one-quantum excitation at energy $\varepsilon$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 337](../../../paper-337-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
