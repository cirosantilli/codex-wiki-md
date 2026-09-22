<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

In character theory, a [p-elementary group](../../../../../p-elementary-group.md) is a finite group isomorphic to $P\times C$, where $P$ is a $p$-group and $C$ is cyclic of order coprime to $p$. Either factor may be trivial. An [elementary group](../../../../../elementary-group.md) is p-elementary for at least one prime $p$; it need not be an elementary [abelian group](../../../../../abelian-group.md).

A [generalised character](../../../../../virtual-character.md) means an integer linear combination of irreducible complex characters. [Brauer's characterisation of characters](../../../../../brauer-s-characterization-of-characters.md) states that a complex [class function](../../../../../class-function.md) $f$ on a finite group $G$ is a [generalised character](../../../../../virtual-character.md) if and only if $f_E$ is a [generalised character](../../../../../virtual-character.md) for every elementary subgroup $E\leq G$. Equivalently,

$$
\boxed{f\in\mathbb Z\operatorname{Irr}(G)\iff\langle f_E,\alpha\rangle_E\in\mathbb Z\text{ for every elementary }E\leq G\text{ and }\alpha\in\operatorname{Irr}(E).}
$$

An ordinary character additionally requires nonnegative coefficients in its global irreducible decomposition. We use the virtual-character criterion just stated.

For the extension construction, set $d=\theta(1)$. The [determinant character](../../../../../determinant-character.md) $\det\theta$ is linear. Since its extension $\mu$ has the same value $1$ at the identity, $\mu$ is also a [linear character](../../../../../linear-character.md). For any $g\in G$, the subgroup $J_g=N\langle g\rangle$ has cyclic quotient $J_g/N$, hence a solvable quotient. The invariant character $\theta$ has degree coprime to $[J_g:N]$, since this index divides $[G:N]$, and $\mu_{J_g}$ extends its determinant. The permitted [coprime-degree determinant extension theorem](../../../../../coprime-degree-determinant-extension-theorem.md) therefore gives a unique character $\chi_g\in\operatorname{Irr}(J_g)$ with

$$
(\chi_g)_N=\theta,\qquad\det\chi_g=\mu_{J_g}.
$$

Define a function on $G$ by $f(g)=\chi_g(g)$. We next verify that these individually defined values form a compatible [class function](../../../../../class-function.md).

If $x\in G$, conjugation carries $J_g$ to $J_{xgx^{-1}}$. Transporting $\chi_g$ by this conjugation gives a character extending $\theta$, because $\theta$ is $G$-invariant, and with determinant $\mu$ restricted to the conjugate subgroup, because $\mu$ is a [class function](../../../../../class-function.md). Uniqueness identifies the transported character with $\chi_{xgx^{-1}}$. Consequently $f(xgx^{-1})=f(g)$.

Now take an elementary subgroup $E\leq G$ and let $J=NE$. A finite $p$-group is solvable, a cyclic group is solvable, and a direct product of [solvable groups](../../../../../solvable-group.md) is solvable. Thus $E$ is solvable, and so is $J/N\cong E/(E\cap N)$. Again the index $[J:N]$ divides $[G:N]$, so the same extension theorem gives $\chi_J\in\operatorname{Irr}(J)$ extending $\theta$ with determinant $\mu_J$.

For $g\in E$, we have $J_g\leq J$. The restriction $(\chi_J)_{J_g}$ is irreducible: an [invariant subspace](../../../../../invariant-subspace.md) for $J_g$ would be invariant for $N$, whose restriction already affords the irreducible $\theta$. Its determinant is $\mu_{J_g}$. By uniqueness on $J_g$, it equals $\chi_g$. Therefore

$$
f_E=(\chi_J)_E,
$$

an ordinary character and hence a [generalised character](../../../../../virtual-character.md) of $E$. [Brauer's characterisation of characters](../../../../../brauer-s-characterization-of-characters.md) now makes $f$ a [generalised character](../../../../../virtual-character.md) of $G$. If $n\in N$, then $J_n=N$ and $\chi_n=\theta$, so $f(n)=\theta(n)$. We have proved, by [gluing determinant-normalized character extensions](../../../../../gluing-determinant-normalized-character-extensions.md),

$$
\boxed{\chi:=f\text{ is a generalised character of }G,\qquad\chi_N=\theta.}
$$

Only the intermediate quotients $J_g/N$ and $NE/N$ were required to be solvable; no solvability assumption on $G/N$ has been added.

For the prime-set assertion, let $E=P\times C$ be p-elementary, and split the cyclic group as $C=C_\pi\times C_{\pi'}$, where each factor has the indicated prime divisors in its order. If $p\in\pi$, put $E_\pi=P\times C_\pi$ and $E_{\pi'}=C_{\pi'}$. If $p\notin\pi$, put $E_\pi=C_\pi$ and $E_{\pi'}=P\times C_{\pi'}$. In both cases the factors commute, have trivial intersection and have orders with disjoint prime spectra. This proves the [prime-set decomposition of elementary groups](../../../../../prime-set-decomposition-of-elementary-groups.md)

$$
\boxed{E=E_\pi\times E_{\pi'},\qquad E_\pi\text{ a }\pi\text{-group},\quad E_{\pi'}\text{ a }\pi'\text{-group}.}
$$

Here a [pi-group](../../../../../pi-group.md) has order divisible only by primes in $\pi$, and a [pi-element](../../../../../pi-element.md) has such an element order; the identity qualifies for both complementary prime sets.

Finally, suppose $K$ satisfies the given element-order condition. The sets $A,B$ are unions of [conjugacy classes](../../../../../conjugacy-class.md) and are disjoint, because membership in both would force every prime divisor of the element order into $\pi\cap\pi'=\varnothing$, hence force order $1$. Let $E\leq K$ be elementary and use $E=E_\pi\times E_{\pi'}$. If both factors were nontrivial, choose $a\ne1$ in the first and $b\ne1$ in the second. They commute and have coprime orders, so $ab$ has order $|a||b|$, containing primes from both $\pi$ and $\pi'$. It would belong to neither $A$ nor $B$ nor $\{1\}$, contrary to the hypothesis. Thus every elementary subgroup is entirely a [pi-group](../../../../../pi-group.md) or entirely a complementary-prime group.

Write $m=|K|_\pi$ and $r=|K|_{\pi'}$ for the two prime parts of $|K|$, so $|K|=mr$ and $\gcd(m,r)=1$. The [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) supplies an integer $D$ satisfying

$$
D\equiv1\pmod m,\qquad D\equiv0\pmod r.
$$

Define the [class function](../../../../../class-function.md)

$$
f(1)=D,\qquad f(a)=1\ (a\in A),\qquad f(b)=0\ (b\in B).
$$

For an elementary $\pi$-subgroup $E$, its order divides $m$. Let $\rho_E$ be the character of its [regular representation](../../../../../regular-representation.md), equal to $|E|$ at $1$ and zero elsewhere. Then

$$
f_E=1_E+\frac{D-1}{|E|}\rho_E,
$$

with integral coefficient because $D\equiv1\pmod{|E|}$. For an elementary $\pi'$-subgroup, its order divides $r$, and

$$
f_E=\frac{D}{|E|}\rho_E
$$

again has integral coefficient. The trivial subgroup satisfies either formula. Every elementary restriction is therefore a [generalised character](../../../../../virtual-character.md). A second application of [Brauer's characterisation of characters](../../../../../brauer-s-characterization-of-characters.md) proves

$$
\boxed{\xi:=f\text{ is a generalised character of }K,\qquad\xi(a)=1\ (a\in A),\quad\xi(b)=0\ (b\in B).}
$$

The freely chosen identity value, fixed by the two congruences, makes the restrictions integral. This construction also covers the cases $\pi=\varnothing$, $\pi'=\varnothing$, or $K=\{1\}$, using modulus-one congruences where appropriate.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
