<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $N=(q^d-1)/(q-1)$, so $N>1$ and $N\equiv1$ in the characteristic. For a nonzero root $x$, division by $x$ gives

$$
x^{q^d-1}+x^{q-1}+t=0.
$$

The projective point $\mathbb F_qx$ is therefore represented by $s=x^{q-1}$, satisfying

$$
P_t(s)=s^N+s+t=0.
$$

Two nonzero roots give the same $s$ exactly when their ratio lies in $\mathbb F_q^\times$. Thus the $N$ projective points are precisely the roots of $P_t$. The [polynomial](../../../../../../polynomial-split.md) $s^N+s+t$ is irreducible in $\mathbb F_q[s,t]$, since it is linear in $t$ and its quotient ring is $\mathbb F_q[s]$. [Gauss's lemma](../../../../../../gauss-s-lemma-riemannian-geometry.md) makes it irreducible over $\mathbb F_q(t)$, so the action on projective points is transitive.

Fix one such coordinate $s$, so $t=-s^N-s$. The other coordinates satisfy

$$
R(Y,s)=\frac{Y^N-s^N}{Y-s}+1=0.
$$

We prove its irreducibility even over $\overline{\mathbb F}_q(s)$. Make the birational change $z=Y/s$, $h=1/s$. Multiplication by $h^{N-1}$ transforms the equation into

$$
h^{N-1}+B(z)=0,\qquad B(z)=\frac{z^N-1}{z-1}.
$$

Choose a nontrivial $N$th [root of unity](../../../../../../root-of-unity.md) $\zeta$ over the [algebraic closure](../../../../../../algebraic-closure.md). Since the characteristic does not divide $N$, $B$ has a simple zero at $\zeta$. Viewed as a [polynomial](../../../../../../polynomial-split.md) in $h$ over $\overline{\mathbb F}_q[z]$, $h^{N-1}+B(z)$ is Eisenstein at the prime $z-\zeta$: the leading coefficient is one, every intermediate coefficient is zero, and the constant term is divisible by that prime exactly once. It is therefore irreducible.

The birational substitution preserves irreducibility after inverting $s$ or $h$. No factor supported solely on $s=0$ is lost, because $R(Y,0)=Y^{N-1}+1$ is nonzero. [Gauss's lemma](../../../../../../gauss-s-lemma-riemannian-geometry.md) then proves that $R(Y,s)$ is irreducible over $\overline{\mathbb F}_q(s)$ and hence over $\mathbb F_q(s)$. Its roots are distinct: a repeated root would have $Y^{N-1}+1=0$ as well as $Y^N+Y+t=0$, forcing $t=0$, impossible generically.

The stabilizer of the chosen projective point is $\operatorname{Gal}(E/\mathbb F_q(s))$, and the irreducibility of $R$ makes it transitive on all the remaining projective points. This proves [projective transitivity of a trinomial linearized polynomial](../../../../../../projective-transitivity-of-a-trinomial-linearized-polynomial.md), namely two-transitivity on the one-dimensional subspaces. The supplied group-theoretic result now applies to the linear subgroup from part (a), giving

$$
\boxed{\operatorname{Gal}(X^{q^d}+X^q+tX,\mathbb F_q(t))\ \supseteq\ SL(d,q).}
$$

The Eisenstein argument remains valid even though $N-1$ is divisible by the characteristic; it concerns irreducibility in $h$, not separability of that projection. Separability of the projective [polynomial](../../../../../../polynomial-split.md) has been checked independently.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
