<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a circular [binary star](../../../../../binary-star.md), the relative orbit has speed $v=\sqrt{GM/a}$. Its orbital [angular momentum](../../../../../angular-momentum.md) is therefore

$$
\boxed{J_{\rm orb}=\mu av=\mu\sqrt{GMa}},
\qquad
M=M_1+M_2,
\qquad
\mu=\frac{M_1M_2}{M}.
$$

Logarithmic differentiation, using $\dot\mu/\mu=\dot M_1/M_1+\dot M_2/M_2-\dot M/M$, gives

$$
\boxed{\frac{\dot a}{a}=2\frac{\dot J_{\rm orb}}{J_{\rm orb}}
-2\frac{\dot M_1}{M_1}-2\frac{\dot M_2}{M_2}
+\frac{\dot M}{M}}.
$$

For [conservative binary mass transfer](../../../../../conservative-binary-mass-transfer.md), $\dot M=0$, $\dot J_{\rm orb}=0$, and $\dot M_2=-\dot M_1$. Hence

$$
\boxed{\frac{\dot a}{a}=-2\dot M_1
\left(\frac1{M_1}-\frac1{M_2}\right)}.
$$

Since a donor has $\dot M_1<0$, the orbit widens for $M_1<M_2$ and shrinks for $M_1>M_2$.

Write the [Roche lobe](../../../../../roche-lobe.md) radius as $R_L=aF(q)$, where

$$
F(q)=0.49\frac{q^{2/3}}
{0.6q^{2/3}+\ln(1+q^{1/3})}.
$$

Then

$$
\boxed{f(q)=\frac{d\ln F}{d\ln q}
=\frac23-
\frac{0.4q^{2/3}+q^{1/3}/[3(1+q^{1/3})]}
{0.6q^{2/3}+\ln(1+q^{1/3})}}.
$$

Conservative transfer has $d\ln q/d\ln M_1=1+q$, so

$$
\boxed{\frac{d\ln R_L}{d\ln M_1}
=\frac{d\ln a}{d\ln M_1}+(1+q)f(q)},
\qquad
\frac{d\ln a}{d\ln M_1}=2(q-1).
$$

The donor response $R_1\propto M_1^{-n}$ has $\zeta_*=d\ln R_1/d\ln M_1=-n$, whereas

$$
\zeta_L=2(q-1)+(1+q)f(q).
$$

After $d\ln M_1<0$, overflow decreases only if $\zeta_*>\zeta_L$. The [dynamical stability of binary mass transfer](../../../../../dynamical-stability-of-binary-mass-transfer.md) criterion is thus

$$
\boxed{n<n_{\rm crit}(q)},
\qquad
\boxed{n_{\rm crit}(q)=2(1-q)-(1+q)f(q)}.
$$

For $q>1$, both terms make $n_{\rm crit}<0$, which is incompatible with $n>0$. Transfer from the more massive donor is therefore dynamically unstable: mass loss shrinks its Roche lobe while the donor expands. The resulting runaway commonly produces a [common envelope](../../../../../common-envelope.md), followed by envelope ejection into a tighter binary or by a stellar merger.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 317](../../paper-317-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
