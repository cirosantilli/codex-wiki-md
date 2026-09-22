<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply the [Serre derivative](../../../../../../serre-derivative.md) in weight twelve to the [modular discriminant](../../../../../../modular-discriminant.md). The preceding result makes $D_{12}\Delta=D\Delta-E_2\Delta$ a weight-fourteen [cusp form](../../../../../../cusp-form.md). The [vanishing of weight-fourteen level-one cusp forms](../../../../../../vanishing-of-weight-fourteen-level-one-cusp-forms.md) follows directly from the [valence formula for the modular group](../../../../../../valence-formula-for-the-modular-group.md): a nonzero such form has order at infinity at least one, and $f(i)=i^{14}f(i)=-f(i)$ forces order at $i$ at least one. Thus its weighted number of zeros would be at least $1+1/2>14/12$, a contradiction. Therefore $D\Delta=E_2\Delta$.

Compare the [Fourier coefficients](../../../../../../fourier-coefficient.md) at positive indices using $\Delta=\sum_{n\geq1}\tau(n)q^n$ and $E_2=1-24\sum_{r\geq1}\sigma_1(r)q^r$. This gives $n\tau(n)=\tau(n)-24\sum_{r=1}^{n-1}\sigma_1(r)\tau(n-r)$. For the [Ramanujan tau function](../../../../../../ramanujan-tau-function.md), the concise recurrence is

$$
\boxed{(1-n)\tau(n)=24\sum_{r=1}^{n-1}\sigma_1(r)\tau(n-r)\qquad(n\geq1).}
$$

At $n=1$ the sum is empty and both sides are zero; normalization supplies $\tau(1)=1$. For instance the next coefficient is $\tau(2)=-24$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 137](../../../paper-137-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
