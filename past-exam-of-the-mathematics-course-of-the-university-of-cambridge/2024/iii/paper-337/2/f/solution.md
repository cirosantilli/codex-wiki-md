<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The [Fluctuation-dissipation theorem](../../../../../../fluctuation-dissipation-theorem.md) in this convention reads

$$
S(\omega,k)=\frac{\varrho(\omega,k)}{1-e^{-\omega/T}}.
$$

In the [classical limit](../../../../../../classical-limit.md) $|\omega|\ll T$, this becomes

$$
S(\omega,k)\simeq\frac{T}{\omega}\varrho(\omega,k)
=\frac{\pi T}{s\omega_k}
\left[\delta(\omega-\omega_k)+\delta(\omega+\omega_k)\right].
$$

The inverse temporal [Fourier transform](../../../../../../fourier-transform.md) is therefore

$$
\boxed{C(t,k)=\int\frac{d\omega}{2\pi}e^{-i\omega t}S(\omega,k)
=\frac{T}{s\omega_k}\cos(\omega_kt)
=\frac{T}{\rho_sk^2}\cos(\omega_kt).}
$$

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Paper 337](../../../paper-337-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
