<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [infinite products](../../../../../../infinite-product.md), a nonzero limiting product requires that its factors tend to one. A useful sufficient condition is

$$
\sum_j|u_j|<\infty,\qquad 1+u_j\ne0.
$$

After finitely many factors, $|u_j|<1/2$ and the principal [holomorphic logarithm](../../../../../../holomorphic-logarithm.md) satisfies $|\log(1+u_j)|\leq2|u_j|$. Therefore the sum of logarithms converges, and exponentiating it gives a finite nonzero product. The same argument on compact sets proves [infinite product convergence from logarithmic tails](../../../../../../infinite-product-convergence-from-logarithmic-tails.md): a locally uniformly absolutely convergent tail of [holomorphic](../../../../../../complex-differentiability-at-a-point.md) logarithms gives a [holomorphic](../../../../../../complex-differentiability-at-a-point.md) nonvanishing tail product. Finite factors then determine all zeros and their orders.

The [Weierstrass elementary factors](../../../../../../weierstrass-elementary-factor.md) are

$$
E_p(w)=(1-w)\exp\left(w+\frac{w^2}{2}+\cdots+\frac{w^p}{p}\right),\quad
E_0(w)=1-w.
$$

For $|w|<1$,

$$
\log E_p(w)=-\sum_{\nu=p+1}^{\infty}\frac{w^\nu}{\nu},
\qquad
|\log E_p(w)|\leq2|w|^{p+1}\quad(|w|\leq1/2).
$$

Their only zero is a simple zero at $w=1$.

Work with [entire functions](../../../../../../entire-function.md) on $\mathbb C$. As usual for prescribed exact zero orders, the distinct zero locations must have consistent multiplicities. The literal statement allows repeated locations with conflicting orders; that cannot be true, for example if the same point is prescribed order one and order two. Remove consistent repetitions rather than adding their orders, and separate a possible zero at the origin.

List the distinct nonzero locations as $a_j$, with prescribed orders $n_j$, and write $m$ for the prescribed order at zero, or zero if the origin is not prescribed. Choose $p_j$ large enough that

$$
n_j2^{-p_j}\leq2^{-j}.
$$

Then the [Weierstrass factorization theorem](../../../../../../weierstrass-factorization-theorem.md) construction is

$$
\boxed{F(z)=z^m\prod_j E_{p_j}(z/a_j)^{n_j}.}
$$

On every compact set, $|z/a_j|\leq1/2$ for all sufficiently large $j$ because $|a_j|\to\infty$. Its logarithmic tail is bounded by

$$
\sum_j n_j|\log E_{p_j}(z/a_j)|\leq\sum_j n_j2^{-p_j}
\leq\sum_j2^{-j}.
$$

Thus the product converges locally uniformly, is entire, and has exactly the specified zeros with exactly their orders. At a prescribed zero, only its own finite factor vanishes; all other finite factors and the tail product are nonzero.

Without escape to infinity the conclusion fails in general. Distinct proposed zeros $1/j$ accumulate at zero. The [identity theorem](../../../../../../identity-theorem.md) would force an [entire function](../../../../../../entire-function.md) with those zeros to vanish identically, which does not have precisely the prescribed isolated zeros. A finite zero set can of course be realized by a polynomial.

For [entire functions with the same zero divisor](../../../../../../entire-functions-with-the-same-zero-divisor.md), the quotient $q=f/g$ extends through every common zero by cancelling equal local powers. It is entire and nowhere zero. Hence $q'/q$ is entire and has a primitive on the [simply connected](../../../../../../simply-connected-space.md) plane. Choose $h(0)$ with $e^{h(0)}=q(0)$ and put

$$
h(z)=h(0)+\int_0^z\frac{q'(\zeta)}{q(\zeta)}\,d\zeta.
$$

The derivative of $qe^{-h}$ vanishes, and its value at zero is one. Therefore

$$
\boxed{f=e^h g.}
$$

If also $f=e^k g$, then $e^{h-k}=1$ everywhere. The continuous difference $h-k$ takes values in the discrete set $2\pi i\mathbb Z$ and so is constant on the [connected](../../../../../../connected-space.md) plane:

$$
\boxed{h-k=2\pi i\ell\quad\text{for one fixed }\ell\in\mathbb Z.}
$$

The whole-plane hypothesis matters: a zero-free [holomorphic](../../../../../../complex-differentiability-at-a-point.md) quotient on a multiply [connected](../../../../../../connected-space.md) domain need not possess a global [holomorphic logarithm](../../../../../../holomorphic-logarithm.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
