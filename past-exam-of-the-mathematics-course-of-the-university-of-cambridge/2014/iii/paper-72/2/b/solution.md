<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the incident [acoustic plane wave](../../../../../../acoustic-plane-wave.md), set $q_0=k\sin\theta$ and $\beta_0=k\cos\theta>0$. The flat reflected field and total field are

$$
\psi_s^{[0]}=-e^{iq_0x+i\beta_0z},\qquad \psi^{[0]}=e^{iq_0x}(e^{-i\beta_0z}-e^{i\beta_0z}).
$$

Therefore $\partial_z\psi^{[0]}(x,0)=-2i\beta_0e^{iq_0x}$ and the [first-order rough-surface scattered field](../../../../../../first-order-rough-surface-scattered-field.md) is

$$
\psi_s^{[1]}(x,z)=\frac{2i\beta_0}{2\pi}\int\widehat h(q-q_0)e^{iqx+i\beta(q)z}dq.
$$

It is linear in the height. Since $\langle h(x)\rangle=0$, its mean vanishes, with the expectation interpreted through finite windows or stationary spectral distributions when needed. Hence

$$
\boxed{\langle\psi_s(x,z)\rangle_{\text{through first order}}=-e^{ik(x\sin\theta+z\cos\theta)}.}
$$

**The coherent first-order reflection is the flat-surface reflection.** If the field symbol is instead used only for the rough correction, its first-order mean is zero. [Stationarity](../../../../../../stationary-process.md) ensures the coherent reflection retains the incident horizontal wavenumber, but zero mean height already explains the vanishing linear correction. The nonzero [root mean square](../../../../../../root-mean-square.md) height does not enter this mean at first order; it does enter the fluctuating reflected field and its intensity.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
