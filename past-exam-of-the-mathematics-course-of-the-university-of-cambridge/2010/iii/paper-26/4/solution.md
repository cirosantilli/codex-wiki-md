<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

We use the [Dirichlet density](../../../../../dirichlet-density.md) form of the [Chebotarev density theorem](../../../../../chebotarev-density-theorem.md), the version directly proved by the permitted information at $s=1$. If $L/K$ is a finite [Galois extension](../../../../../finite-galois-extension.md) of [number fields](../../../../../number-field.md) with group $G$ and $C$ is a [conjugacy class](../../../../../conjugacy-class.md), let $S_C$ be the unramified [prime ideals](../../../../../prime-ideal.md) of $K$ whose [Frobenius conjugacy class](../../../../../frobenius-conjugacy-class.md) is $C$. Then

$$
\boxed{\delta(S_C):=\lim_{s\downarrow1}
\frac{\displaystyle\sum_{\mathfrak p\in S_C}(N\mathfrak p)^{-s}}
{\log(1/(s-1))}=\frac{|C|}{|G|}}.
$$

The same conclusion holds for a union of [conjugacy classes](../../../../../conjugacy-class.md), replacing $|C|$ by the size of that union. The denominator may equivalently be the sum over all primes of $K$. Here and below $s>1$ is real. This specifies the density being proved; an unweighted prime-counting asymptotic is a stronger formulation and is not being inferred merely from a limit at one.

First establish the necessary pole for a general base field. The [Dedekind zeta function as a permutation Artin L-function](../../../../../dedekind-zeta-function-as-a-permutation-artin-l-function.md) gives it using exactly the allowed assumptions. Take a finite normal closure $E$ of $K/\mathbb Q$, and let $W$ be the [permutation representation](../../../../../permutation-representation.md) on $\operatorname{Hom}_{\mathbb Q}(K,E)$. Its trivial constituent has multiplicity one: an invariant function on the transitive set of embeddings is constant. At a rational prime, a basis of $W^I$ consists of the sums over inertia orbits of embeddings. [Frobenius automorphism](../../../../../frobenius-automorphism.md) permutes these orbit sums. Within the decomposition-group orbit belonging to a prime $\mathfrak p$ of $K$, the resulting cycle has length $f_{\mathfrak p}$, because the residue embeddings are permuted cyclically by finite-field Frobenius. A cycle of length $f$ has determinant $\det(1-T\rho(\operatorname{Frob}))=1-T^f$. Consequently the [local factor of an Artin L-function](../../../../../local-factor-of-an-artin-l-function.md) gives

$$
L_{\mathbb Q}(W,s)=\prod_p\prod_{\mathfrak p\mid p}(1-p^{-f_{\mathfrak p}s})^{-1}
=\zeta_K(s),
$$

including at ramified primes. Decomposing $W=\mathbf1\oplus\bigoplus_{\psi\ne\mathbf1}m_\psi\psi$ gives

$$
\zeta_K(s)=\zeta(s)\prod_{\psi\ne\mathbf1}L_{\mathbb Q}(\psi,s)^{m_\psi}.
$$

All factors after $\zeta$ are holomorphic and nonzero at one by the allowed hypothesis. Thus $\zeta_K$ has a simple pole there and

$$
\log\zeta_K(s)=\log\frac1{s-1}+O(1).
$$

This argument also explains why the trivial relative [Artin L-function](../../../../../artin-l-function.md) is $\zeta_K$, rather than always the Riemann zeta function.

Now let $\chi$ be an [irreducible character](../../../../../irreducible-character.md) of $G$, of degree $d_\chi$. At an unramified prime the [Euler product](../../../../../euler-product.md) has local factor $\det(1-\rho_\chi(g_{\mathfrak p})(N\mathfrak p)^{-s})^{-1}$, where $g_{\mathfrak p}$ is a Frobenius representative. The [eigenvalues](../../../../../eigenvalue.md) of $\rho_\chi(g)$ are [roots of unity](../../../../../root-of-unity.md), since $g$ has finite order. Expanding the logarithm for $s>1$ therefore gives

$$
\log L_K(\chi,s)
=\sum_{\mathfrak p\ \mathrm{unramified}}\sum_{m\ge1}
\frac{\chi(g_{\mathfrak p}^m)}{m(N\mathfrak p)^{ms}}+R_\chi(s),
$$

where the finitely many ramified local factors contribute a function bounded as $s\downarrow1$. They are nonzero and finite near one because their [eigenvalues](../../../../../eigenvalue.md) have modulus one while $(N\mathfrak p)^{-1}<1$.

The terms $m\ge2$ are uniformly bounded. Indeed $|\chi(g)|\le d_\chi$, and for $N\mathfrak p\ge2$ and $s\ge1$,

$$
\sum_{m\ge2}\frac{(N\mathfrak p)^{-ms}}m
\le\sum_{m\ge2}(N\mathfrak p)^{-m}\le2(N\mathfrak p)^{-2}.
$$

There are at most $[K:\mathbb Q]$ primes of $K$ above each rational prime and each has norm at least that prime. Hence $\sum_{\mathfrak p}(N\mathfrak p)^{-2}<\infty$. Isolating $m=1$ proves the [character prime sums in the Chebotarev proof](../../../../../character-prime-sums-in-the-chebotarev-proof.md) identity

$$
\sum_{\mathfrak p\ \mathrm{unramified}}
\chi(g_{\mathfrak p})(N\mathfrak p)^{-s}
=\log L_K(\chi,s)+O(1).
$$

For nontrivial $\chi$, the allowed holomorphy and nonvanishing at one give a local [holomorphic logarithm](../../../../../holomorphic-logarithm.md) and a bounded right side. The logarithm specified by the Euler series differs from that local branch by a constant multiple of $2\pi i$ on the real interval near one, so it too is bounded. For the trivial character, the right side is $\log(1/(s-1))+O(1)$ by the pole of $\zeta_K$. Thus

$$
\sum_{\mathfrak p\ \mathrm{unramified}}
\chi(g_{\mathfrak p})(N\mathfrak p)^{-s}
=\begin{cases}\log(1/(s-1))+O(1),&\chi=\mathbf1,\\ O(1),&\chi\ne\mathbf1.\end{cases}
$$

Expand the conjugacy-class indicator by [character orthogonality](../../../../../character-orthogonality.md). For $c\in C$,

$$
\mathbf1_C(g)=\frac{|C|}{|G|}\sum_{\chi\in\widehat G}
\overline{\chi(c)}\,\chi(g).
$$

To see the coefficient, take its inner product with $\chi$: $|G|^{-1}\sum_{g\in C}\overline{\chi(g)}=|C|\overline{\chi(c)}/|G|$. The [irreducible characters](../../../../../irreducible-character.md) form an orthonormal basis of [class functions](../../../../../class-function.md), so this is the full expansion. Substituting the prime-sum estimates leaves only the trivial character's logarithmic term:

$$
\sum_{\mathfrak p\in S_C}(N\mathfrak p)^{-s}
=\frac{|C|}{|G|}\log\frac1{s-1}+O(1).
$$

Division by the diverging logarithm proves the theorem. The same trivial-character calculation shows that all primes of $K$ have density one; adding or removing finitely many primes does not change a [Dirichlet density](../../../../../dirichlet-density.md).

There is a necessary qualification for the final polynomial application: **the printed claim is false for degree one**. For example, $X$ is monic and irreducible in $\mathbb Z[X]$, yet has the root zero modulo every prime. We prove the intended assertion for degree $n\ge2$.

Let $L$ be the [splitting field](../../../../../splitting-field.md) of the monic [irreducible polynomial](../../../../../irreducible-polynomial.md) over $\mathbb Q$, and let $\Omega$ be its $n$ roots. The [Galois group](../../../../../galois-group.md) $G$ acts transitively on $\Omega$. There is a [derangement in a transitive group action](../../../../../derangement-in-a-transitive-group-action.md): count the pairs $(g,\alpha)$ satisfying $g\alpha=\alpha$. The [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md) gives

$$
\sum_{g\in G}|\operatorname{Fix}_\Omega(g)|
=\sum_{\alpha\in\Omega}|G_\alpha|=n\frac{|G|}{n}=|G|.
$$

If every $g$ fixed at least one root, the identity, which fixes $n\ge2$, would make this sum at least $|G|+n-1$, a contradiction. Therefore some $g$ fixes no root, and neither does any conjugate of $g$.

For completeness, relate this group action to reduction without assuming the desired splitting result. All roots are [algebraic integers](../../../../../algebraic-integer.md), since the polynomial is monic. Exclude the finitely many primes ramifying in $L$ or dividing the nonzero [polynomial discriminant](../../../../../polynomial-discriminant.md). At a prime $\mathfrak q$ over any remaining $p$, the roots reduce to distinct elements of $k_{\mathfrak q}$ and give all roots of the reduced polynomial. [Arithmetic Frobenius](../../../../../frobenius-automorphism.md) permutes them by $b\mapsto b^p$. A reduced root belongs to $\mathbb F_p$ exactly when it is fixed by this map. Because reduction is injective on the original root set, this happens exactly when the Frobenius permutation fixes an original root. This proves the [Frobenius permutation and roots modulo a prime](../../../../../frobenius-permutation-and-roots-modulo-a-prime.md) criterion.

The [Chebotarev density theorem](../../../../../chebotarev-density-theorem.md) assigns the [conjugacy class](../../../../../conjugacy-class.md) of our fixed-point-free $g$ the positive [Dirichlet density](../../../../../dirichlet-density.md) $|C_g|/|G|$. All but finitely many of these primes have rootless reduction, so there are infinitely many. More precisely, applying the same argument to the union of all fixed-point-free classes gives

$$
\boxed{\delta\{p:f\bmod p\text{ has no root in }\mathbb F_p\}
=\frac{|\{g\in G:\operatorname{Fix}_\Omega(g)=\varnothing\}|}{|G|}>0
\quad(n\ge2).}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
