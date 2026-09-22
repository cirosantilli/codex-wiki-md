<h1 id="35a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Set $k_B=1$. After the [Gaussian integral](../../../../../../gaussian-integral.md) over momenta, the [canonical partition function](../../../../../../canonical-partition-function.md) factors as

$$
Z=Z_{\rm kin}\frac1{N!}\int_{V^N}e^{-U(\mathbf x_1,\ldots,\mathbf x_N)/T}\,d^{3N}x,
$$

whereas the [ideal gas](../../../../../../ideal-gas.md) has $Z_{\rm ideal}=Z_{\rm kin}V^N/N!$. Hence

$$
\frac Z{Z_{\rm ideal}}
=\frac1{V^N}\int_{V^N}e^{-U/T}\,d^{3N}x
=1+\frac1{V^N}\int_{V^N}(e^{-U/T}-1)\,d^{3N}x.
$$

Using the [Helmholtz free energy](../../../../../../helmholtz-free-energy.md) $F=-T\log Z$ therefore gives

$$
\boxed{F=F_{\rm ideal}-T\log\left\{1+\frac1{V^N}\int_{V^N}(e^{-U/T}-1)\,d^{3N}x\right\}}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [35A](../../35a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
