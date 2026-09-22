<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The product defining the [modular discriminant](../../../../../../modular-discriminant.md) converges locally uniformly for $|q|<1$ and has integral [Fourier coefficients](../../../../../../fourier-coefficient.md). Its [logarithmic derivative](../../../../../../logarithmic-derivative.md) is

$$
D\log\left(q\prod_{r\geq1}(1-q^r)^{24}\right)
=1-24\sum_{r\geq1}\frac{rq^r}{1-q^r}
=1-24\sum_{n\geq1}\sigma_1(n)q^n=E_2.
$$

Therefore $D\Delta=E_2\Delta$. Comparing the coefficient of $q^n$ gives $n\tau(n)=\tau(n)-24\sum_{j=1}^{n-1}\sigma_1(j)\tau(n-j)$, or

$$
\boxed{(1-n)\tau(n)=24\sum_{j=1}^{n-1}\sigma_1(j)\tau(n-j).}
$$

This also fixes the initial value $\tau(1)=1$.

For the [Ramanujan tau congruence modulo five](../../../../../../ramanujan-tau-congruence-modulo-five.md), first justify the link between this product and $E_4,E_6$. Question 1 constructs $\Delta_0=(E_4^3-E_6^2)/1728\in S_{12}$ with first coefficient one. Its [Serre derivative](../../../../../../serre-derivative.md) is in $S_{14}$, which vanishes by the [valence formula for the modular group](../../../../../../valence-formula-for-the-modular-group.md): a nonzero such [cusp form](../../../../../../cusp-form.md) would contribute at least $1+1/2>14/12$, since it vanishes at infinity and at $i$. Hence $D\Delta_0=E_2\Delta_0$. The product and $\Delta_0$ have the same [differential equation](../../../../../../differential-equation-split.md) and leading coefficient. Equivalently their quotient has derivative zero near $q=0$ and limit one; the [identity theorem](../../../../../../identity-theorem.md) gives

$$
1728\Delta=E_4^3-E_6^2.
$$

Also $D_6E_6\in M_8=\mathbb C E_4^2$. Its constant coefficient is $-1/2$, so the [Serre derivative](../../../../../../serre-derivative.md) gives $2DE_6=E_2E_6-E_4^2$.

Work now in the [formal power series](../../../../../../formal-power-series.md) ring $\mathbb F_5[[q]]$. The integral expansions give $E_4\equiv1$ and $E_2\equiv E_6\pmod5$, because $d^5\equiv d\pmod5$, $-24\equiv-504\equiv1$, and $240\equiv0$. The two identities reduce to

$$
3\Delta\equiv1-E_6^2,\qquad 2DE_6\equiv E_6^2-1\pmod5.
$$

Thus $3\Delta\equiv-2DE_6\equiv3DE_6$, and division by the nonzero element $3$ gives $\Delta\equiv DE_6$. Since the coefficient of $q^n$ in $DE_6$ is $-504n\sigma_5(n)$, we conclude

$$
\boxed{\tau(n)\equiv n\sigma_5(n)\pmod5\quad(n\geq1).}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
