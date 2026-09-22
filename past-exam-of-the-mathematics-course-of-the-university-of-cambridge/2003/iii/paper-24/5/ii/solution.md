<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Logarithmically differentiate the convergent product of the [modular discriminant](../../../../../../modular-discriminant.md). On compact subsets of $\mathbb H$, [absolute convergence](../../../../../../absolute-convergence.md) permits termwise differentiation and rearrangement of the resulting divisor sums:

$$
\frac1{2\pi i}\frac{\Delta'(\tau)}{\Delta(\tau)}=1-24\sum_{m\geq1}\frac{mq^m}{1-q^m}=1-24\sum_{n\geq1}\sigma_1(n)q^n=E_2(\tau).
$$

The division is valid because $\Delta$ has no interior zeros. Its weight-twelve inversion law is $\Delta(-1/\tau)=\tau^{12}\Delta(\tau)$. Taking a logarithmic derivative, including the derivative $1/\tau^2$ of $-1/\tau$, yields

$$
\frac1{\tau^2}\frac{\Delta'(-1/\tau)}{\Delta(-1/\tau)}=\frac{12}\tau+\frac{\Delta'(\tau)}{\Delta(\tau)}.
$$

Thus the [Eisenstein series of weight two](../../../../../../eisenstein-series-of-weight-two.md) has the anomalous transformation

$$
\boxed{E_2(-1/\tau)=\tau^2E_2(\tau)+\frac{6\tau}{\pi i}.}
$$

Let $y=\operatorname{Im}\tau$. Under inversion, $y$ becomes $y/|\tau|^2$. Using $\tau^2-|\tau|^2=2iy\tau$, the anomalous term cancels:

$$
E_2^*(-1/\tau)=\tau^2E_2(\tau)+\frac{6\tau}{\pi i}-\frac{3|\tau|^2}{\pi y}=\tau^2\left(E_2(\tau)-\frac3{\pi y}\right)=\tau^2E_2^*(\tau).
$$

The Fourier expansion gives $E_2(\tau+1)=E_2(\tau)$, and translation leaves $y$ unchanged. Since translation and inversion generate the projective [modular group](../../../../../../modular-group.md) and weight two is unchanged by $-I$, the [almost holomorphic weight-two Eisenstein series](../../../../../../almost-holomorphic-weight-two-eisenstein-series.md) satisfies

$$
\boxed{E_2^*(\gamma\tau)=(c\tau+d)^2E_2^*(\tau)\qquad\gamma\in SL_2(\mathbb Z).}
$$

It is modular in the transformation sense, but is not a holomorphic [modular form](../../../../../../modular-form.md). Substituting $\operatorname{Im}(\gamma\tau)=y/|c\tau+d|^2$ into this law also gives the useful full-group anomaly

$$
E_2(\gamma\tau)=(c\tau+d)^2E_2(\tau)+\frac{6c(c\tau+d)}{\pi i}.
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
