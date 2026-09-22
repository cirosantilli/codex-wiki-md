<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [modulus of a number field](../../../../../../modulus-of-a-number-field.md) is $\mathfrak m=\mathfrak m_0\mathfrak m_\infty$, with $\mathfrak m_0$ a nonzero integral [ideal](../../../../../../ideal.md) and $\mathfrak m_\infty$ a subset of the real places. Let $I_{\mathfrak m}$ be the [group](../../../../../../group-split.md) of [fractional ideals](../../../../../../fractional-ideal.md) prime to $\mathfrak m_0$, and let $P_{\mathfrak m}$ consist of principal [ideals](../../../../../../ideal.md) $(a)$ with $a\equiv1$ at each prime power in $\mathfrak m_0$ and $a>0$ at each selected real place. The [ray class group](../../../../../../ray-class-group.md) is

$$
\operatorname{Cl}_{\mathfrak m}(K)=I_{\mathfrak m}/P_{\mathfrak m}.
$$

The [ray class field](../../../../../../ray-class-field.md) $K_{\mathfrak m}$ is the finite [abelian extension](../../../../../../abelian-extension.md) for which the [Artin map](../../../../../../artin-reciprocity-law.md) has [kernel](../../../../../../kernel-of-a-linear-map.md) $P_{\mathfrak m}$ and induces an isomorphism $\operatorname{Cl}_{\mathfrak m}(K)\cong\operatorname{Gal}(K_{\mathfrak m}/K)$. Equivalently it is the maximal [abelian extension](../../../../../../abelian-extension.md) whose conductor divides $\mathfrak m$.

To compute its order use the [ray class exact sequence](../../../../../../ray-class-exact-sequence.md), including signatures:

$$
\mathcal O_K^\times\longrightarrow (\mathcal O_K/\mathfrak m_0)^\times\times\{\pm1\}^{|\mathfrak m_\infty|}\longrightarrow\operatorname{Cl}_{\mathfrak m}(K)\longrightarrow\operatorname{Cl}(K)\longrightarrow1.
$$

The middle map lifts a residue and sign tuple to an element of $K$ by [weak approximation theorem](../../../../../../weak-approximation-for-inequivalent-absolute-values.md), then takes its principal [ideal](../../../../../../ideal.md) as a ray class. Different lifts differ by a principal ray factor. Its [kernel](../../../../../../kernel-of-a-linear-map.md) consists exactly of tuples represented by global units. Every ordinary [ideal class](../../../../../../ideal-class.md) has a representative prime to the finite modulus, again by [weak approximation theorem](../../../../../../weak-approximation-for-inequivalent-absolute-values.md); this gives surjectivity of the last map. If $U_{\mathfrak m}$ denotes the [ray units](../../../../../../ray-unit.md), the kernel of the unit map is $U_{\mathfrak m}$. The [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md) and counting units in each prime-power quotient give the [ray class number formula](../../../../../../ray-class-number-formula.md)

$$
\boxed{|\operatorname{Cl}_{\mathfrak m}(K)|=\frac{h_K\,2^{|\mathfrak m_\infty|}\,\Phi_K(\mathfrak m_0)}{[\mathcal O_K^\times:U_{\mathfrak m}]},\qquad \Phi_K(\mathfrak m_0)=N\mathfrak m_0\prod_{\mathfrak p\mid\mathfrak m_0}\left(1-\frac1{N\mathfrak p}\right).}
$$

First take $K=\mathbb Q(\sqrt{-3})$. Its [ring of integers](../../../../../../ring-of-integers.md) is $\mathbb Z[\omega]$, where $\omega=(-1+\sqrt{-3})/2$ and $\omega^2+\omega+1=0$. The [Minkowski bound for ideal classes](../../../../../../minkowski-s-bound.md) is $(2/\pi)\sqrt3<2$, so every [ideal class](../../../../../../ideal-class.md) has a representative of norm one and $h_K=1$. Its units are the six [roots of unity](../../../../../../root-of-unity.md). Modulo seven, the polynomial $X^2+X+1$ has distinct roots $2,4$, and therefore

$$
\mathcal O_K/(7)\cong\mathbb F_7\times\mathbb F_7,\qquad \omega\mapsto(2,4).
$$

The [unit group](../../../../../../unit-group.md) of this quotient has order $36$. The unit $1+\omega$ maps to $(3,5)$, which has order six; consequently unit reduction is injective and $U_{(7)}=\{1\}$. The [ray class number formula](../../../../../../ray-class-number-formula.md) gives $36/6=6$.

We also identify the quotient explicitly. Conjugation interchanges the two factors, so the residue [norm](../../../../../../norm.md) is $(x,y)\mapsto xy$. Its [kernel](../../../../../../kernel-of-a-linear-map.md) has order six and equals the image of the six units, since $3\cdot5=1\pmod7$. Hence

$$
\operatorname{Cl}_{(7)}(K)\cong\mathbb F_7^\times\cong C_6.
$$

The field $M=K(\zeta_7)=\mathbb Q(\zeta_{21})$ has degree six over $K$, since the degrees over $\mathbb Q$ are twelve and two. It is [unramified](../../../../../../unramified-extension.md) outside seven by the cyclotomic computation and the base-change argument above. At primes over seven, $K$ has completion $\mathbb Q_7$, and $M/K$ is the tame degree-six cyclotomic extension; its conductor exponent is one. Its relative arithmetic [Artin symbol](../../../../../../artin-symbol.md) at an [ideal](../../../../../../ideal.md) $\mathfrak a$ prime to seven acts by

$$
\zeta_7\longmapsto\zeta_7^{N\mathfrak a\bmod7}.
$$

If $\mathfrak a=(a)$ with $a\equiv1\pmod{7\mathcal O_K}$, then $N_{K/\mathbb Q}(a)\equiv1\pmod7$. Thus the [Artin map](../../../../../../artin-reciprocity-law.md) kills the principal ray subgroup. It factors through the order-six [ray class group](../../../../../../ray-class-group.md); the residue [norm](../../../../../../norm.md) quotient computed above shows that it is onto the degree-six [Galois group](../../../../../../galois-group.md), so the fields coincide. This proves the explicit [ray class field of Q of square root minus three modulo seven](../../../../../../ray-class-field-of-q-of-square-root-minus-three-modulo-seven.md):

$$
\boxed{K_{(7)}=K(\zeta_7)=\mathbb Q(\zeta_{21}),\qquad[K_{(7)}:K]=6.}
$$

Now take $K=\mathbb Q(\sqrt{-6})$, and write $s=\sqrt{-6}$. Its [ring of integers](../../../../../../ring-of-integers.md) is $\mathbb Z[s]$, its [discriminant](../../../../../../discriminant.md) is $-24$, and its units are $\pm1$. The quotient by $(s)$ is

$$
\mathbb Z[s]/(s)\cong\mathbb Z/6\mathbb Z,
$$

whose two units are both images of $\pm1$. The [ray class exact sequence](../../../../../../ray-class-exact-sequence.md) therefore gives $\operatorname{Cl}_{(s)}(K)\cong\operatorname{Cl}(K)$.

For its [class number](../../../../../../class-number.md), the [Minkowski bound for ideal classes](../../../../../../minkowski-s-bound.md) is $(2/\pi)\sqrt{24}<4$, so each [ideal class](../../../../../../ideal-class.md) contains an integral [ideal](../../../../../../ideal.md) of norm at most three. The primes of norms two and three are

$$
\mathfrak p_2=(2,s),\qquad\mathfrak p_3=(3,s),\qquad\mathfrak p_2^2=(2),\quad\mathfrak p_3^2=(3),\quad\mathfrak p_2\mathfrak p_3=(s).
$$

These are the only nontrivial possibilities within the bound, and their [ideal classes](../../../../../../ideal-class.md) coincide and have order at most two. The [ideal](../../../../../../ideal.md) $\mathfrak p_2$ is not principal: its being principal would give an integer solution to $x^2+6y^2=2$, which is impossible. Thus $h_K=2$, the [ideal class group](../../../../../../ideal-class-group.md) is $C_2$, and the ray field is the [Hilbert class field](../../../../../../hilbert-class-field.md).

We verify its actual identity rather than stopping at the degree. Put

$$
H=K(\sqrt2)=\mathbb Q(\sqrt2,\sqrt{-3}),\qquad b=\frac{1+\sqrt{-3}}2.
$$

The two quadratic fields $\mathbb Q(\sqrt2)$ and $\mathbb Q(\sqrt{-3})$ are distinct, so $[H:\mathbb Q]=4$ and $[H:K]=2$. The integral elements $1,\sqrt2,b,\sqrt2b$ are a rational [basis](../../../../../../basis.md). Their trace matrix is the [Kronecker product](../../../../../../kronecker-product.md) of the two quadratic trace matrices, with [discriminants](../../../../../../discriminant.md) $8$ and $-3$. Its [determinant](../../../../../../determinant.md) is therefore $8^2(-3)^2=576$. The [discriminant-index formula for an integral lattice](../../../../../../discriminant-index-formula-for-an-integral-lattice.md) shows that the field [discriminant](../../../../../../discriminant.md) divides $576$. On the other hand the relative [discriminant ideal](../../../../../../discriminant-ideal.md) formula gives

$$
|D_H|=|D_K|^{[H:K]}N_{K/\mathbb Q}(\mathfrak d_{H/K})=576\,N_{K/\mathbb Q}(\mathfrak d_{H/K}).
$$

The norm on the right is a positive integer, so equality is forced. Thus the relative [discriminant ideal](../../../../../../discriminant-ideal.md) is the unit ideal, and $H/K$ is [unramified](../../../../../../unramified-extension.md) at every finite prime. There are no real places of $K$. The extension is quadratic and therefore [Abelian](../../../../../../abelian-group.md); its degree equals $h_K$, identifying it with the [Hilbert class field of Q of square root minus six](../../../../../../hilbert-class-field-of-q-of-square-root-minus-six.md). Hence the [ray class field of Q of square root minus six modulo square root minus six](../../../../../../ray-class-field-of-q-of-square-root-minus-six-modulo-square-root-minus-six.md) is

$$
\boxed{K_{(\sqrt{-6})}=K(\sqrt2)=\mathbb Q(\sqrt2,\sqrt{-3}),\qquad[K_{(\sqrt{-6})}:K]=2.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
