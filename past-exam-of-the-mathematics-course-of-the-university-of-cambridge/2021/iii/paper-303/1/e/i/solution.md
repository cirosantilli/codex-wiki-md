<h1 id="1/e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

This is the [Blume–Capel model](../../../../../../../blume-capel-model.md). In the [mean-field approximation](../../../../../../../mean-field-approximation.md), write $m=\langle\sigma_i\rangle$ and replace

$$
\sigma_i\sigma_j\simeq m\sigma_i+m\sigma_j-m^2.
$$

Because every site has [coordination number](../../../../../../../coordination-number-of-a-lattice.md) $q$, the resulting energy is

$$
E_{\rm MF}=\frac12NJqm^2+\sum_i\left[g\sigma_i^2-(Jqm+B)\sigma_i\right].
$$

The one-site [partition function](../../../../../../../canonical-partition-function.md) is therefore

$$
Z_1=\sum_{\sigma=-1}^{1}e^{-\beta[g\sigma^2-(Jqm+B)\sigma]}
=1+2e^{-\beta g}\cosh\!\left(\beta(Jqm+B)\right).
$$

With $\kappa=e^{-\beta g}$, the mean-field partition function is $Z_{\rm MF}=e^{-\beta NJqm^2/2}Z_1^N$. Taking $F=-T\log Z_{\rm MF}$ gives

$$
\boxed{\frac FN=\frac12Jqm^2-T\log\!\left[1+2\kappa\cosh\!\left(\beta(Jqm+B)\right)\right]}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [E](../../e.md)
3. [1](../../../1.md)
4. [Paper 303](../../../../paper-303-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
