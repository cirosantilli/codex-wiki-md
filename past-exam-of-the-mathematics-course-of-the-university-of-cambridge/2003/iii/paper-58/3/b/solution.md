<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the [matter power spectrum](../../../../../../matter-power-spectrum.md) by the [Fourier transform](../../../../../../fourier-transform.md) convention

$$
\delta(\mathbf x,\tau)=\int\frac{d^3k}{(2\pi)^3}\delta_{\mathbf k}(\tau)e^{i\mathbf k\cdot\mathbf x},\qquad
\langle\delta_{\mathbf k}\delta_{\mathbf k'}^*\rangle=(2\pi)^3\delta^3(\mathbf k-\mathbf k')P_\delta(k,\tau).
$$

Statistical isotropy then gives

$$
\langle\delta^2\rangle=\int d\log k\,\frac{k^3P_\delta(k,\tau)}{2\pi^2}.
$$

For the growing mode found above, write $P_\delta(k,\tau)=\tau^4P_A(k)$. At [cosmological horizon entry](../../../../../../cosmological-horizon-entry.md), $\tau_H\propto k^{-1}$, so the variance contribution per logarithmic interval is proportional to $k^3k^{-4}P_A(k)=P_A(k)/k$. Making it independent of $k$ requires $P_A(k)\propto k$. Hence

$$
\boxed{P_\delta(k,\tau)\propto\tau^4k.}
$$

This is the [Harrison-Zeldovich spectrum](../../../../../../harrison-peebles-zeldovich-spectrum.md). Scale invariance applies at horizon entry, not to the unprocessed density variance on a common late-time slice. In the notation $\delta_{\mathbf k}\propto k^{n/2}\tau^2$, it means **$n=1$**, with random Fourier coefficients supplying the ensemble statistics.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
