<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

From part (a), $\Theta F=E_2F$. Its product has integer coefficients and begins with $q$, so write $F=\sum_{n\geq1}\tau(n)q^n$, with $\tau(1)=1$. Comparing the coefficient of $q^n$ gives

$$
n\tau(n)=\tau(n)-24\sum_{\ell=1}^{n-1}\sigma_1(\ell)\tau(n-\ell),
$$

which rearranges to

$$
\boxed{(1-n)\tau(n)=24\sum_{\ell=1}^{n-1}\sigma_1(\ell)\tau(n-\ell).}
$$

This is a recurrence for the [Ramanujan tau function](../../../../../../ramanujan-tau-function.md); for example it gives $\tau(2)=-24$ and $\tau(3)=252$.

For the congruence, use the normalized Eisenstein expansions

$$
E_4=1+240\sum_{n\geq1}\sigma_3(n)q^n,\qquad
E_6=1-504\sum_{n\geq1}\sigma_5(n)q^n.
$$

The [modular form](../../../../../../modular-form.md) $E_4^3-E_6^2$ is a [cusp form](../../../../../../cusp-form.md) of weight twelve, and its leading coefficient is $720-(-1008)=1728$. Since $S_{12}$ is one-dimensional and $F$ starts with $q$,

$$
E_4^3-E_6^2=1728F.
$$

Also $D_6E_6$ is a weight-eight form, with constant coefficient $-1/2$. Since $M_8$ is one-dimensional and $E_4^2$ has constant coefficient one, $D_6E_6=-E_4^2/2$, or

$$
2\Theta E_6=E_2E_6-E_4^2.
$$

These identities have rational coefficients whose only displayed denominators are prime to five, so coefficientwise reduction modulo five is legitimate. We have $E_4\equiv1$. Furthermore $d^5\equiv d\pmod5$ gives $\sigma_5(n)\equiv\sigma_1(n)$, while $-504\equiv-24\equiv1$, so $E_6\equiv E_2$. Therefore

$$
F\equiv\frac{1-E_6^2}{3}=\frac{E_6^2-1}{2}\equiv\Theta E_6\pmod5.
$$

The equality in the middle is in $\mathbb F_5$, where $-1/3=1/2$. Comparing coefficients in $\Theta E_6=-504\sum_{n\geq1}n\sigma_5(n)q^n$ gives

$$
\boxed{\tau(n)\equiv n\sigma_5(n)\pmod5.}
$$

This proves the [Ramanujan tau congruence modulo five](../../../../../../ramanujan-tau-congruence-modulo-five.md) from the given small-dimensional modular-form spaces, without assuming that congruence as a theorem.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
