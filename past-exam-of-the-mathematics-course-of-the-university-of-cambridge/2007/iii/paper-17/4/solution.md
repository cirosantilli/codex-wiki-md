<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The dense [algebraic torus](../../../../../algebraic-torus.md) has coordinate ring $k[M]$, a [Laurent polynomial ring](../../../../../laurent-polynomial-ring.md) and hence a [unique factorization domain](../../../../../unique-factorization-domain.md). Its [divisor class group](../../../../../divisor-class-group.md) is therefore zero. Restrict an arbitrary [Weil divisor](../../../../../weil-divisor.md) $D$ to the [algebraic torus](../../../../../algebraic-torus.md) and choose a [rational function on an algebraic variety](../../../../../rational-function-on-an-algebraic-variety.md) $f$ whose divisor there is $D|_T$. Then $D-\operatorname{div}(f)$ is supported on the [algebraic torus](../../../../../algebraic-torus.md) boundary. The prime divisors in that boundary are precisely the $F_j$ corresponding to the [toric rays](../../../../../ray-of-a-fan.md), by the [torus orbit-cone correspondence](../../../../../orbit-cone-correspondence.md). Consequently

$$
\boxed{D\sim\sum_{j=1}^d a_jF_j\quad\text{for some }a_j\in\mathbb Z.}
$$

Since the variety is smooth, every [Weil divisor](../../../../../weil-divisor.md) is Cartier. This gives invariant representatives for all divisor classes, without assuming that the original divisor was invariant.

Now use such a representative. The associated vector space is

$$
L(D)=\{f\in k(X)^*: \operatorname{div}(f)+D\ge0\}\cup\{0\}=H^0(X,\mathcal O_X(D)).
$$

The [principal divisor on a toric variety](../../../../../principal-divisor-on-a-toric-variety.md) formula gives $\operatorname{div}(\chi^m)=\sum_j\langle m,e_j\rangle F_j$. Define the [lattice polytope of a toric divisor](../../../../../lattice-polytope-of-a-toric-divisor.md)

$$
P_D=\{m\in M_{\mathbb R}:\langle m,e_j\rangle\ge-a_j\text{ for every }j\}.
$$

For a maximal [toric cone](../../../../../cone-in-toric-geometry.md) $\sigma$, its basic [toric ray](../../../../../ray-of-a-fan.md) vectors are a basis of $N$, so there is a unique integral $m_\sigma$ with $\langle m_\sigma,e_j\rangle=-a_j$ on its [toric rays](../../../../../ray-of-a-fan.md). The [algebraic torus character](../../../../../algebraic-torus-character.md) $\chi^{m_\sigma}$ is a local frame for $\mathcal O(D)$ on $U_\sigma$. Every global section restricts on the [algebraic torus](../../../../../algebraic-torus.md) to a finite [Laurent polynomial](../../../../../laurent-polynomial.md) $\sum_m c_m\chi^m$. Relative to this frame, regularity on $U_\sigma$ means $\sum_m c_m\chi^{m-m_\sigma}\in k[\sigma^\vee\cap M]$. Since distinct [algebraic torus characters](../../../../../algebraic-torus-character.md) are independent, this holds exactly when each exponent with nonzero coefficient satisfies the inequalities for the [toric rays](../../../../../ray-of-a-fan.md) of $\sigma$. Taking all charts proves

$$
\boxed{L(D)=\bigoplus_{m\in P_D\cap M}k\chi^m.}
$$

Completeness makes $P_D$ bounded when nonempty: a nonzero recession vector would be nonnegative on every [toric ray](../../../../../ray-of-a-fan.md) of a complete [toric fan](../../../../../fan-in-toric-geometry.md), and therefore on all of $N_{\mathbb R}$, which is impossible. The displayed space is consequently finite-dimensional.

At the torus-fixed point $p_\sigma$ in the smooth chart $U_\sigma\cong\mathbb A^n$, a section $\chi^m$ has local [monomial](../../../../../monomial.md) $\chi^{m-m_\sigma}$. Its value is nonzero exactly when this [monomial](../../../../../monomial.md) is constant, namely when $m=m_\sigma$. Thus if the [complete linear system of a divisor](../../../../../complete-linear-system-of-a-divisor.md) has no base point, some section is nonzero at $p_\sigma$, forcing $m_\sigma\in P_D$. Conversely, if $m_\sigma\in P_D$ for every maximal [toric cone](../../../../../cone-in-toric-geometry.md), its [algebraic torus character](../../../../../algebraic-torus-character.md) is a global section whose local expression on $U_\sigma$ is one. It therefore vanishes nowhere on that whole chart, and these charts cover $X$. This proves the [toric basepoint-free criterion](../../../../../toric-basepoint-free-criterion.md):

$$
\boxed{|D|\text{ is basepoint-free}\ \Longleftrightarrow\ \forall\sigma\in\Sigma(n),\ \langle m_\sigma,e_j\rangle\ge-a_j\text{ for all }j,\text{ with equality on }\sigma.}
$$

The analogous [toric ampleness criterion](../../../../../toric-ampleness-criterion.md), stated without proof, replaces the inequalities off $\sigma$ by strict ones:

$$
\boxed{D\text{ is ample}\ \Longleftrightarrow\ \forall\sigma\in\Sigma(n),\ \langle m_\sigma,e_j\rangle=-a_j\text{ on }\sigma,\quad\langle m_\sigma,e_j\rangle>-a_j\text{ off }\sigma.}
$$

Equivalently, the [normal fan of a polytope](../../../../../normal-fan-of-a-polytope.md) $P_D$ is exactly $\Sigma$.

For the final [fan subdivision](../../../../../fan-subdivision.md), take $n\ge2$ so that $\tilde e$ is a new [toric ray](../../../../../ray-of-a-fan.md), as the construction requires. The vectors $e_1,\ldots,e_n$ are a lattice basis, so their sum is primitive. Replacing any one basis vector by this sum gives another basis. Thus the [star subdivision](../../../../../star-subdivision.md) gives a smooth [toric blowup at a torus-fixed point](../../../../../toric-blowup-at-a-torus-fixed-point.md) $\pi:X_{\Sigma'}\to X_\Sigma$, with [algebraic exceptional divisor](../../../../../algebraic-exceptional-divisor.md) $E=\tilde F$. On the old chart, a local equation of $D$ is $\chi^{-m_\sigma}$, whose order on the new [toric ray](../../../../../ray-of-a-fan.md) is $-\langle m_\sigma,\tilde e\rangle=\sum_{i=1}^n a_i=a$. All old [toric ray](../../../../../ray-of-a-fan.md) coefficients are unchanged. Therefore

$$
\boxed{D'=\pi^*D.}
$$

We prove ampleness of $D_c=cD'-E$ directly by inequalities, giving the [ample divisor after blowing up a torus-fixed point](../../../../../ample-divisor-after-blowing-up-a-torus-fixed-point.md) result.

Let $u_1,\ldots,u_n$ be the basis of $M$ dual to $e_1,\ldots,e_n$. On the new maximal [toric cone](../../../../../cone-in-toric-geometry.md) $\sigma_i$, which omits $e_i$, the required local [algebraic torus character](../../../../../algebraic-torus-character.md) is

$$
m_{i,c}=cm_\sigma+u_i.
$$

Indeed its pairings on $e_j$, $j\ne i$, are $-ca_j$, while its pairing on $\tilde e$ is $-ca+1$, exactly the negative of the new coefficient $ca-1$. Its inequality on the omitted old [toric ray](../../../../../ray-of-a-fan.md) has strict gap one:

$$
\langle m_{i,c},e_i\rangle+ca_i=1.
$$

For any [toric ray](../../../../../ray-of-a-fan.md) $e_j$ outside the original [toric cone](../../../../../cone-in-toric-geometry.md), put $\delta_j=\langle m_\sigma,e_j\rangle+a_j$. The original ampleness gives positive integers $\delta_j$, and the new strict gaps are

$$
\langle m_{i,c},e_j\rangle+ca_j=c\delta_j+\langle u_i,e_j\rangle>0
$$

for all sufficiently large $c$.

For any unchanged maximal [toric cone](../../../../../cone-in-toric-geometry.md) $\eta\ne\sigma$, the local [algebraic torus character](../../../../../algebraic-torus-character.md) is $cm_\eta$. All strict inequalities on old [toric rays](../../../../../ray-of-a-fan.md) follow from those for $D$. Its inequality on the new [toric ray](../../../../../ray-of-a-fan.md) has gap

$$
\langle cm_\eta,\tilde e\rangle+ca-1=c\epsilon_\eta-1,\qquad\epsilon_\eta=\sum_{i=1}^n(\langle m_\eta,e_i\rangle+a_i).
$$

Each summand is nonnegative, and at least one is positive because $\eta\ne\sigma$ cannot contain all its [toric rays](../../../../../ray-of-a-fan.md). Hence $\epsilon_\eta$ is a positive integer, making this gap positive for $c\ge2$. There are only finitely many remaining inequalities. For example, any integer satisfying

$$
c>\max\left\{1,\ \max_{\substack{1\le i\le n\\j>n}}\frac{-\langle u_i,e_j\rangle}{\delta_j}\right\}
$$

works, with the inner maximum omitted when its index set is empty. The [toric ampleness criterion](../../../../../toric-ampleness-criterion.md) now gives

$$
\boxed{cD'-\tilde F\text{ is ample for every sufficiently large integer }c.}
$$

The new-ray assumption is essential to the printed construction. In dimension one, $\tilde e=e_1$ and the [fan subdivision](../../../../../fan-subdivision.md) is unchanged, so the two purported distinct divisors coincide. If the displayed definition of $D'$ is applied literally on $\mathbb P^1$ with coefficients $a_1=-2$, $a_2=3$, then $D$ has degree one but $D'$ has degree $-1$, contradicting the conclusion. The argument above applies to the intended blowup in dimension at least two.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
