<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The zero-prescription claim requires a [closed discrete subset](../../../../../closed-discrete-subset.md), meaning no accumulation in $\Omega$. If “discrete” means only that each listed point is isolated, it is false: $\{1/n:n\geq1\}\subset\mathbb C$ is a [discrete subset](../../../../../discrete-subset.md), but any [holomorphic function](../../../../../holomorphic-function.md) vanishing there is identically zero by the [identity theorem for holomorphic functions](../../../../../identity-theorem.md), and then has additional zeros. In the usual zero-set interpretation, discreteness includes local finiteness. We prove the claim with this necessary interpretation.

First choose an increasing [compact exhaustion](../../../../../compact-exhaustion.md) $K_j$ of $\Omega$ by relatively filled sets: every component of $\widehat{\mathbb C}\setminus K_j$ meets $\widehat{\mathbb C}\setminus\Omega$. Such an exhaustion is obtained by exhausting with finite unions of small closed squares lying in $\Omega$, then adding all complementary components relatively compact in $\Omega$. The filled sets remain compact in $\Omega$: a complementary component containing a point within distance $\operatorname{dist}(K_j,\mathbb C\setminus\Omega)$ of the complement could join that complement through a ball disjoint from $K_j$, and hence would not be filled. Their boundedness follows by using a disk containing the initial compact. Nesting can be ensured by enlarging each stage first. This is also the geometric description of the [holomorphic convex hull](../../../../../holomorphic-convex-hull.md) proved below.

A finite prescribed set is realized by a finite product of linear factors. For an infinite [closed discrete subset](../../../../../closed-discrete-subset.md), enumerate the distinct points as $a_n$. Every compact contains only finitely many of them, so there are indices $j(n)\to\infty$ with $a_n\notin K_{j(n)}$. Finitely many initial factors can be handled without an approximation requirement. For the remaining factors, let $U_n$ be the complementary component containing $a_n$. It also contains a point $c_n\notin\Omega$ or infinity. Join $a_n$ to $c_n$ by an arc in that component, or to infinity by a ray-like arc. Define

$$
p_n(z)=\frac{z-a_n}{z-c_n}\quad(c_n\ne\infty),
\qquad p_n(z)=z-a_n\quad(c_n=\infty).
$$

Each $p_n$ is a [holomorphic function](../../../../../holomorphic-function.md) on $\Omega$, has exactly one [simple zero](../../../../../simple-zero.md), at $a_n$, and no other zeros there.

The arc is disjoint from $K_{j(n)}$, and $p_n$ has a [holomorphic logarithm](../../../../../holomorphic-logarithm.md) $L_n$ near that compact. To justify the logarithm, any closed curve avoiding the arc has equal [winding numbers](../../../../../winding-number.md) about its finite endpoints, so the integral of $p_n'/p_n$ around it is zero. For a ray to infinity the winding number about $a_n$ is zero. A primitive of $p_n'/p_n$, adjusted by a constant on each component, supplies the logarithm.

The [Runge theorem](../../../../../runge-s-theorem.md) proved in Question 4 approximates $L_n$ uniformly on $K_{j(n)}$ by $h_n\in\mathcal O(\Omega)$: all needed finite poles can be chosen outside $\Omega$ because every complementary component meets its complement. Choose the error small enough that

$$
F_n=p_n e^{-h_n},\qquad \sup_{K_{j(n)}}|F_n-1|<2^{-n}.
$$

Each $F_n$ still has exactly the [simple zero](../../../../../simple-zero.md) $a_n$. On every fixed compact, all sufficiently late factors satisfy the summable bound above. Hence their [infinite product](../../../../../infinite-product.md) converges locally uniformly. It has a nonzero tail because, once $|F_n-1|<1/2$, its logarithmic tails satisfy $|\log F_n|\leq2|F_n-1|$ and converge absolutely. Thus multiplying by the finitely many earlier factors gives **a holomorphic function with precisely the prescribed zeros, and no additional zeros**. Repeating a factor to any prescribed finite positive multiplicity gives the corresponding multiplicity version. This is [prescribed zeros in a plane domain via Runge approximation](../../../../../prescribed-zeros-in-a-plane-domain-via-runge-approximation.md), not an invocation of the existence theorem being asked for.

For the specified [infinite product](../../../../../infinite-product.md), put $a_k=q^{-2k-1}$. On any compact annulus $0<r\leq|z|\leq R$,

$$
\sum_{k\geq0}\bigl(|a_kz|+|a_kz^{-1}|\bigr)
\leq(R+r^{-1})\frac{|q|^{-1}}{1-|q|^{-2}}<\infty.
$$

The logarithmic-tail estimate therefore proves locally uniform convergence on $\mathbb C^*$ and nonvanishing wherever no individual factor vanishes. At a zero of one factor, the product is zero and the remaining product converges to a nonzero value. Consequently

$$
\boxed{\text{The product is defined and converges for every }z\ne0;
\quad Z(\sigma)=\{q^{2k+1},q^{-2k-1}:k\geq0\}.}
$$

All these [zeros](../../../../../zero-of-a-function.md) are simple and distinct: their moduli distinguish the two strings and their indices. At $z=0$ the reciprocal factors are undefined, so the given expression has no convergence value there. The infinite sequence of zeros tending to zero also rules out continuation across that point as a [holomorphic function](../../../../../holomorphic-function.md).

Set $P(z)=\prod_{k\geq1}(1-q^{-2k}z)(1-q^{-2k}z^{-1})$. Absolute local convergence allows reindexing:

$$
\sigma(qz)=(1-z)P(z),\qquad
\sigma(q^{-1}z)=(1-z^{-1})P(z).
$$

Since $1-z=-z(1-z^{-1})$, **$\sigma(qz)=-z\sigma(q^{-1}z)$ for every $z\ne0$**. No division by a vanishing factor is involved, so the identity also holds at all the zeros.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
