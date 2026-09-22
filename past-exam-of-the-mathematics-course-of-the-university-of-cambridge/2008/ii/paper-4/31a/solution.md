<h1 id="31a/solution">Solution</h1>

↑ **Parent:** [31A](../31a.md)

Put $A=n^2-1/4$. Substitute $w=e^{sz}\sum_{k\geq0}c_kz^{\rho-k}$ into $w''+(1-A/z^2)w=0$. The leading coefficient gives $s^2+1=0$, and the next gives $2s\rho c_0=0$. Thus $s=\pm i$, $\rho=0$. The coefficient of $e^{sz}z^{-k-2}$ then gives

$$
\boxed{c_{k+1}=\frac{k(k+1)-A}{2s(k+1)}c_k,\qquad c_0\ne0.}
$$

In particular $c_1=sAc_0/2$ and $c_2=A(2-A)c_0/8$. The two [Bessel inverse-power expansions at infinity](../../../../../bessel-inverse-power-expansion-at-infinity.md) start as

$$
\boxed{w_\pm\sim C_\pm e^{\pm iz}\left(1\pm\frac{iA}{2z}+\frac{A(2-A)}{8z^2}+\cdots\right).}
$$

Their [independent](../../../../../independent-random-variables.md) leading oscillations give two [independent](../../../../../independent-random-variables.md) asymptotic solutions, represented by suitable multiples of $\sqrt zH_n^{(1)}(z)$ and $\sqrt zH_n^{(2)}(z)$ on the positive-real large-$z$ sector.

For the [Liouville–Green approximation](../../../../../wkb-approximation.md), $q=1-A/z^2$ gives

$$
q^{-1/4}=1+\frac A{4z^2}+O(z^{-4}),\qquad
\int^z\sqrt q\,d\zeta=z+\frac A{2z}+O(z^{-3}),
$$

where the integration constant is absorbed in the amplitude. Hence its two leading wave forms have first two terms

$$
\boxed{q^{-1/4}e^{\pm i\int^z\sqrt q}
=e^{\pm iz}\left(1\pm\frac{iA}{2z}+O(z^{-2})\right).}
$$

Expanding one order further gives the same $A(2-A)/(8z^2)$ as the formal recurrence.

The infinite sums must be interpreted as [asymptotic expansions](../../../../../asymptotic-expansion.md), not literal convergent inverse-power series. For integer $n$, $A$ never equals $k(k+1)$, so the recurrence never truncates, and $|c_{k+1}/c_k|\sim k/2$. Thus the inverse-power series diverges at every finite nonzero $z$. Exact Hankel solutions have these asymptotic series; the printed “solutions of the form” uses that customary asymptotic meaning.

## ↑ Ancestors (10)

1. [31A](../31a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
