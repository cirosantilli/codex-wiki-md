<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

**[Herbrand quotient](../../../../../herbrand-quotient.md) and local norm indices.** Let $G=\langle\sigma\rangle$ have order $n$. For an additive $G$-module $M$, put $D=\sigma-1$ and $N=1+\sigma+\cdots+\sigma^{n-1}$. The relevant [Tate cohomology of a cyclic group](../../../../../tate-cohomology-of-a-cyclic-group.md) groups are

$$
\widehat H^0(G,M)=M^G/NM,\qquad \widehat H^{-1}(G,M)=\ker N/DM.
$$

If both groups are finite, their size ratio is the [Herbrand quotient](../../../../../herbrand-quotient.md)

$$
h_G(M)=\frac{\#\widehat H^0(G,M)}{\#\widehat H^{-1}(G,M)}.
$$

Multiplicative modules use products for $N$ and $D(m)=\sigma(m)/m$. A finite module has quotient one: $\#\ker N=\#M/\#NM$, while $\#DM=\#M/\#M^G$, and the two cohomology orders are equal. The six-term periodic cohomology sequence shows $h(B)=h(A)h(C)$ for a short exact sequence $0\to A\to B\to C\to0$ when these groups are finite. Thus the quotient is unchanged by finite-index changes of lattices. For the trivial $G$-module $\mathbb Z$, the zeroth group is $\mathbb Z/n\mathbb Z$ and the negative first group is zero, so $h_G(\mathbb Z)=n$.

Now let $L/K$ be a cyclic extension of [p-adic fields](../../../../../p-adic-field.md) of degree $n$. For a sufficiently deep [principal unit](../../../../../principal-unit.md) subgroup $U_L^r=1+\mathfrak m_L^r$, the [p-adic logarithm](../../../../../p-adic-logarithm.md) is a $G$-equivariant isomorphism with the additive [p-adic lattice](../../../../../integral-lattice-in-a-p-adic-vector-space.md) $\mathfrak m_L^r$; it suffices to take $r>v_L(p)/(p-1)$. The [normal basis theorem](../../../../../normal-basis-theorem.md) makes $L$ a regular $K[G]$-module. Consequently $\mathfrak m_L^r$, as a $\mathbb Z_p[G]$-lattice, is commensurable with a direct sum of $[K:\mathbb Q_p]$ copies of $\mathbb Z_p[G]$. These regular lattices have zero Tate groups: its invariants are the multiples of the sum of the basis elements, every such element is a norm, and vectors with coefficient sum zero are images of $D$. Commensurability and the finite-module calculation give $h_G(U_L^r)=1$. Since $U_L/U_L^r$ is finite, $h_G(U_L)=1$. These comparisons also establish finiteness of the Tate groups concerned.

The valuation exact sequence $1\to U_L\to L^\times\to\mathbb Z\to0$ now gives $h_G(L^\times)=n$. [Hilbert theorem 90](../../../../../hilbert-s-theorem-90.md) makes $\widehat H^{-1}(G,L^\times)$ trivial. One can prove the cyclic statement directly: for $a$ of norm one set $A_0=1$, $A_i=a\sigma(a)\cdots\sigma^{i-1}(a)$ and choose $c$ for which $b=\sum_i A_i\sigma^i(c)\ne0$. Such a $c$ exists by linear independence of distinct field automorphisms. Then $\sigma(b)=b/a$, so $a=b/\sigma(b)$ is a coboundary. Therefore **the local cyclic norm index is**

$$
\boxed{[K^\times:N_{L/K}L^\times]=[L:K]=n.}
$$

This is the central use of the [Herbrand quotient](../../../../../herbrand-quotient.md): it calculates a norm index without first constructing the local reciprocity map.

Let $e,f$ be the [ramification index](../../../../../ramification-index.md) and [residue degree](../../../../../residue-degree.md). With normalized integer valuations, $v_K(Nx)=f v_L(x)$. A norm is a unit exactly when its preimage is a unit, and the norm valuations fill $f\mathbb Z$. Hence there is an exact sequence

$$
1\to\mathcal O_K^\times/N\mathcal O_L^\times\to K^\times/NL^\times\to\mathbb Z/f\mathbb Z\to0.
$$

**The unit norm index is $\boxed{[\mathcal O_K^\times:N\mathcal O_L^\times]=e}$.** In an unramified extension all units are norms and the obstruction is the valuation modulo $n$; in a totally ramified cyclic extension the entire index comes from units. The norm subgroup is open: on deep [principal units](../../../../../principal-unit.md), logarithm carries the norm to the [field trace](../../../../../field-trace.md), and the trace of a full [p-adic lattice](../../../../../integral-lattice-in-a-p-adic-vector-space.md) contains a sufficiently deep [p-adic lattice](../../../../../integral-lattice-in-a-p-adic-vector-space.md) in $K$.

**[Hilbert norm residue symbol](../../../../../hilbert-norm-residue-symbol.md) and the local-to-global principle.** More generally, for a local field $F$ containing $\mu_m$, fix the local reciprocity map $\operatorname{rec}_F$ with uniformizers acting as arithmetic Frobenius on unramified extensions. The [Hilbert norm residue symbol](../../../../../hilbert-norm-residue-symbol.md) is

$$
(a,b)_{F,m}=\frac{\operatorname{rec}_F(b)(a^{1/m})}{a^{1/m}}\in\mu_m.
$$

This is independent of the chosen root, is bilinear, and has value one exactly when $b$ is a norm from $F(a^{1/m})$. These are standard consequences of [Local Artin reciprocity](../../../../../local-artin-reciprocity.md). The case $m=2$, for which the values are signs, is the one directly governing [quadratic forms](../../../../../quadratic-form.md). The [quadratic Hilbert symbol](../../../../../quadratic-hilbert-symbol.md) at a place $v$ is defined for $a,b\in K_v^\times$ by

$$
(a,b)_v=\begin{cases}1,&b\in N_{K_v(\sqrt a)/K_v}(K_v(\sqrt a)^\times),\\-1,&\text{otherwise},\end{cases}
$$

with value one for all $b$ when $a$ is a square. Equivalently it is one precisely when $z^2=ax^2+by^2$ has a nonzero solution over $K_v$. For nonsquare $a$, a solution has $y\ne0$ and gives $b=(z/y)^2-a(x/y)^2$; the converse follows from the same norm identity. When $a$ is square the conic is already isotropic. Symmetry follows from this conic criterion. The local cyclic norm index gives a norm subgroup of index two; its sign character is multiplicative in $b$, and symmetry gives multiplicativity in $a$. Thus the symbol is a nondegenerate bilinear pairing on the [square-class group of a field](../../../../../square-class-group-of-a-field.md), since every nonsquare $a$ gives a nontrivial norm character. Also $(a,-a)_v=1$, because $N(\sqrt a)=-a$, and $(a,a)_v=(a,-1)_v$.

For an odd-residue-characteristic [p-adic field](../../../../../p-adic-field.md) with residue size $q$, write $a=\pi^r u$, $b=\pi^s w$, and let $\chi$ be the quadratic character of the residue units. Then

$$
\boxed{(a,b)=(-1)^{rs(q-1)/2}\chi(\overline u)^s\chi(\overline w)^r.}
$$

The unramified [quadratic extension](../../../../../quadratic-extension.md) has every unit as a norm and only even norm valuations; in a ramified [quadratic extension](../../../../../quadratic-extension.md) the norm of a unit has square residue. The preceding unit norm index is two, so the square-residue condition in the ramified case is also sufficient. These facts, together with $N(\sqrt\pi)=-\pi$, determine the formula on the generators $u,\pi$ of the [square-class group](../../../../../square-class-group-of-a-field.md). At a real place the symbol is negative exactly when both arguments are negative, and at a complex place it is always one. For $\mathbb Q_2$, with $u,w$ odd units, the dyadic formula is

$$
(a,b)_2=(-1)^{\frac{u-1}{2}\frac{w-1}{2}+r\frac{w^2-1}{8}+s\frac{u^2-1}{8}}.
$$

Only residue classes modulo eight and the parities of $r,s$ enter; other dyadic fields retain the norm definition.

The [Hilbert reciprocity law](../../../../../hilbert-reciprocity-law.md) states $\prod_v(a,b)_v=1$ for $a,b\in K^\times$. Only finitely many factors can be nontrivial: outside the places above two, the Archimedean places, and the finite places where $a$ or $b$ is not a unit, the odd-residue formula gives one. For $K=\mathbb Q$ this product formula is a formulation of [quadratic reciprocity](../../../../../quadratic-reciprocity.md), including its supplementary laws. It forces local norm obstructions to occur with compatible parity. It is a necessary compatibility law, not by itself a substitute for the following local-to-global theorem.

The [Hasse-Minkowski theorem](../../../../../hasse-minkowski-theorem.md) states that a nondegenerate [quadratic form](../../../../../quadratic-form.md) over a [number field](../../../../../number-field.md) has a nonzero isotropic vector if and only if it does over every completion. Equivalently, two nondegenerate [quadratic forms](../../../../../quadratic-form.md) are isometric globally if and only if they are isometric at every place. The forward directions are immediate; the reverse directions are the substantive global theorem. Over non-Archimedean completions, local isometry classes are determined by dimension, determinant square class and the [Hasse invariant of a quadratic form](../../../../../hasse-invariant-of-a-quadratic-form.md)

$$
\epsilon_v(\langle a_1,\ldots,a_m\rangle)=\prod_{i<j}(a_i,a_j)_v.
$$

At real places one uses signature, and at complex places dimension suffices. Reciprocity gives $\prod_v\epsilon_v(q)=1$ for a globally diagonalized form. These invariants make the theorem practically usable: local square classes and norm characters replace an unrestricted search for rational solutions. In particular every [quadratic form](../../../../../quadratic-form.md) of dimension at least five over a [p-adic field](../../../../../p-adic-field.md) is isotropic; for such a form over a [number field](../../../../../number-field.md) the only isotropy obstructions are definite signatures at real places.

As a concrete application, take nonsquare $a\in K^\times$. Then $b$ is a global norm from $K(\sqrt a)$ if and only if $(a,b)_v=1$ at every place. The local conditions make the ternary form $\langle1,-a,-b\rangle$ isotropic everywhere. [Hasse-Minkowski theorem](../../../../../hasse-minkowski-theorem.md) gives a global solution of $z^2-a x^2=b y^2$; since $a$ is nonsquare, $y$ cannot be zero, and division by $y$ gives the global norm. For example $-1$ fails to be a norm from $\mathbb Q(i)$ already at the real place. **Thus the [quadratic Hilbert symbol](../../../../../quadratic-hilbert-symbol.md) detects local norm solvability, while the [Hasse-Minkowski theorem](../../../../../hasse-minkowski-theorem.md) turns solvability at all places into a global quadratic solution.** The reciprocity and local-to-global theorems in this essay are stated as standard results; the norm interpretation, bilinearity and application are derived above.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
