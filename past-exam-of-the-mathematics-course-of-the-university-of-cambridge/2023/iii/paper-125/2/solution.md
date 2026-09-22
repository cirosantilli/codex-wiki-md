<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Hasse theorem for elliptic curves](../../../../../hasse-s-theorem-on-elliptic-curves.md) states that for $E/\mathbb F_q$,

$$
\left|\#E(\mathbb F_q)-(q+1)\right|\leq2\sqrt q.
$$

Let $\pi$ be the [Frobenius isogeny of an elliptic curve](../../../../../frobenius-isogeny-of-an-elliptic-curve.md). Its fixed points are exactly $E(\mathbb F_q)$, and $1-\pi$ is separable because its differential is the identity. Therefore

$$
\#E(\mathbb F_q)=\#\ker(1-\pi)=\deg(1-\pi).
$$

For every endomorphism $\alpha$, the [dual isogeny](../../../../../dual-isogeny.md) gives $\alpha\widehat\alpha=[\deg\alpha]$, and the degree satisfies the parallelogram law

$$
\deg(\alpha+\beta)+\deg(\alpha-\beta)=2\deg\alpha+2\deg\beta.
$$

Consequently, if $a=1+q-\deg(1-\pi)$ is the [trace](../../../../../trace-of-an-elliptic-curve-endomorphism.md) of $\pi$, then

$$
\deg([m]-[n]\pi)=m^2-amn+qn^2.
$$

This is nonnegative for every pair of integers $m,n$. By approximating the minimizing real ratio $m/n=a/2$, the quadratic polynomial can be nonnegative for all rational ratios only if its discriminant is nonpositive. Thus $a^2\leq4q$, and the displayed point-count identity proves Hasse's theorem.

An explicit example with nonisomorphic groups occurs over $\mathbb F_{43}$. Put

$$
E_1:y^2=x^3+2x+4,
\qquad
E_2:y^2=x^3+20.
$$

On $E_1$, the point $(30,19)$ has order seven and its nonzero cyclic subgroup has $x$-coordinates $30,31,40$. [Vélu formulas](../../../../../velu-s-formulas.md) give the quotient coefficients

$$
v=6\sum x_i^2+6A=9,
\qquad
w=10\sum x_i^3+6A\sum x_i+12B=10
\pmod {43},
$$

so the degree-seven quotient is

$$
A'=A-5v=0,
\qquad B'=B-7w=20,
$$

which is $E_2$. Direct quadratic-residue counts give $\#E_1(\mathbb F_{43})=\#E_2(\mathbb F_{43})=49$. The points killed by seven on $E_1$ are only the displayed kernel and $O$, while $(1,8)$ and $(3,2)$ are independent seven-torsion points on $E_2$. Hence

$$
E_1(\mathbb F_{43})\cong\mathbb Z/49\mathbb Z,
\qquad
E_2(\mathbb F_{43})\cong(\mathbb Z/7\mathbb Z)^2.
$$

Finally, let $p<43$ and suppose two curves are linked by an isogeny of degree seven. The isogeny and its dual induce inverse isomorphisms on every prime-to-seven primary subgroup, so nonisomorphic rational point groups would require $49$ to divide their common order. Since this order is less than $57$ by Hasse, one group would then be cyclic of order $49$ and the other would contain all of $E[7]$. The [Weil pairing](../../../../../weil-pairing.md) on rational seven-torsion forces $\mu_7\subset\mathbb F_p$, hence $p\equiv1\pmod7$ unless $p=7$. The only prime below $43$ congruent to one modulo seven is $29$, but Hasse gives $\#E(\mathbb F_{29})<49$; for $p=7$ the same inequality is immediate. No such pair exists below $43$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 125](../../paper-125-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
