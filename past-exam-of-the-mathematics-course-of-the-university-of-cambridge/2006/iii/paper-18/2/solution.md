<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Fix $p_0\in X$ on a connected [compact Riemann surface](../../../../../compact-riemann-surface.md), and construct its [Jacobian variety](../../../../../jacobian-variety.md) by periods as in the first solution. For a [divisor on an algebraic curve](../../../../../divisor-on-an-algebraic-curve.md) $E=\sum_p n_p p$ of degree zero, define

$$
\operatorname{AJ}(E)=\left[\omega\longmapsto\sum_p n_p\int_{p_0}^p\omega\right]\in\operatorname{Jac}(X).
$$

Changing the paths adds a [period lattice](../../../../../period-lattice.md) element; changing $p_0$ adds a common integral multiplied by $\sum n_p=0$. The [Abel theorem for divisors](../../../../../abel-theorem-for-divisors.md) says

$$
\boxed{\operatorname{AJ}(E)=0\quad\Longleftrightarrow\quad E=\operatorname{div}(f)\text{ for a nonzero meromorphic function }f.}
$$

Equivalently, effective [divisors on an algebraic curve](../../../../../divisor-on-an-algebraic-curve.md) of the same degree have the same Abelian sum exactly when they are equivalent under [linear equivalence of divisors](../../../../../linear-equivalence-of-divisors.md).

We need a meromorphic version of the [Riemann bilinear relations](../../../../../riemann-bilinear-relations-for-a-compact-surface.md). Let $\eta$ be a [differential of the third kind](../../../../../differential-of-the-third-kind.md), with [residues](../../../../../residue.md) $n_p$ at its simple poles, and let $\omega$ be a [holomorphic differential form](../../../../../holomorphic-differential-form.md). Choose representatives of the cycles and paths avoiding the poles in the same cut polygon, and let $F(p)=\int_{p_0}^p\omega$ there. Then

$$
\sum_i\left(A_i(\omega)B_i(\eta)-B_i(\omega)A_i(\eta)\right)=2\pi i\sum_p n_pF(p).
$$

Here the equality is an equality of the chosen complex numbers, before taking any quotient. To prove it, remove small disks about the poles. Since $d(F\eta)=\omega\wedge\eta=0$ on the remaining polygon, its boundary integral is zero. Pairing opposite outer edges gives the left side, just as in the first solution. The clockwise boundary about $p$ contributes $-2\pi i n_pF(p)$ by the [residue theorem](../../../../../residue-theorem.md). Moving these terms to the other side proves the formula and its sign.

Such an $\eta$ exists whenever $\sum n_p=0$. Here is the required existence argument. Let $S$ be the reduced support of $E$, and consider

$$
0\longrightarrow K_X\longrightarrow K_X(S)\xrightarrow{\operatorname{res}}\bigoplus_{p\in S}\mathbb C_p\longrightarrow0.
$$

Locally the last map takes $c\,dz/z$ to $c$. By [Serre duality](../../../../../serre-duality.md), the obstruction in $H^1(K_X)\cong\mathbb C$ is dual to restriction of constant functions, so it is the sum of the [residues](../../../../../residue.md). Thus the kernel of this sum is exactly the image of global meromorphic differentials. Alternatively, the [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) gives $h^0(K_X(S))-h^0(K_X)=|S|-1$, and the [residue theorem](../../../../../residue-theorem.md) identifies that image with the same codimension-one subspace. Subtracting a linear combination of the normalized [holomorphic differential forms](../../../../../holomorphic-differential-form.md) makes $A_i(\eta)=0$ for every $i$.

Suppose now that $\operatorname{AJ}(E)=0$. Let $u_i=\sum_p n_p\int_{p_0}^p\omega_i$ with the paths used above. There are integer columns $m,n$ such that $u=m+\tau n$. The normalized meromorphic bilinear formula gives $B_i(\eta)=2\pi i u_i$. Therefore

$$
\eta'=\eta-2\pi i\sum_j n_j\omega_j
$$

has $a$-periods $-2\pi i n_i$ and $b$-periods $2\pi i m_i$. Its integrals around the poles are also in $2\pi i\mathbb Z$. These cycles generate the homology of the punctured surface, so

$$
f(q)=\exp\left(\int_{q_*}^q\eta'\right)
$$

is a single-valued, nowhere-zero [holomorphic function](../../../../../holomorphic-function.md) away from the support of $E$. Near $p$, write $\eta'=n_p\,dz/z+h(z)\,dz$. Then $f=z^{n_p}\exp(H(z))$ times a nonzero constant, with $H'=h$. It extends meromorphically with order exactly $n_p$. Hence $\operatorname{div}(f)=E$.

Conversely, if $E=\operatorname{div}(f)$, take $\eta=df/f$. It has [residues](../../../../../residue.md) $n_p$ and every period lies in $2\pi i\mathbb Z$: continuation of a local logarithm of $f$ changes it by an integral multiple of $2\pi i$. Write $A_i(\eta)=2\pi i r_i$ and $B_i(\eta)=2\pi i s_i$. Applying the meromorphic bilinear formula to $\omega_i$ gives

$$
u_i=s_i-\sum_j\tau_{ij}r_j.
$$

Thus $u\in\Lambda$ and $\operatorname{AJ}(E)=0$, completing both directions without assuming the conclusion as a property of the [Jacobian variety](../../../../../jacobian-variety.md).

For completeness, the effective degree-$d$ version lives on the [symmetric product of a curve](../../../../../symmetric-product-of-a-curve.md) $X^{(d)}=X^d/\mathfrak S_d$. The sum of integrals on $X^d$ is invariant under the finite [symmetric group](../../../../../symmetric-group.md) and descends to the [Abelian sum map](../../../../../abel-map-of-an-algebraic-curve.md) $u_d$. The quotient is locally described by elementary symmetric coordinates, so repeated points are included. The proof above identifies its fibre over $u_d(D)$ with

$$
|D|=\mathbb P H^0(X,\mathcal O_X(D)).
$$

Explicitly, a nonzero [global section](../../../../../global-section.md) gives its effective zero [divisor](../../../../../divisor.md), and two sections give the same [divisor](../../../../../divisor.md) precisely when their quotient is constant. These maps are holomorphic in local symmetric coordinates. More intrinsically, a family of effective [divisors on an algebraic curve](../../../../../divisor-on-an-algebraic-curve.md) in this fixed class determines a line of sections of $\mathcal O_X(D)$, after locally trivializing any [line bundle](../../../../../line-bundle.md) pulled back from the parameter space. Conversely such a line of sections gives its family of zero [divisors on an algebraic curve](../../../../../divisor-on-an-algebraic-curve.md). These operations are inverse and unaffected by that trivialization, proving the identification with the [projective space](../../../../../projective-space-split.md) in families as well as on points.

Finally this description identifies the analytic [Jacobian variety](../../../../../jacobian-variety.md) with $\operatorname{Pic}^0(X)$. Every degree-zero [line bundle](../../../../../line-bundle.md) has a meromorphic section: after twisting by a sufficiently large effective [divisor](../../../../../divisor.md), the [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) supplies a nonzero [global section](../../../../../global-section.md). Its [divisor](../../../../../divisor.md) represents the original [line bundle](../../../../../line-bundle.md). The correspondence to the period quotient is well-defined and injective by the theorem. It is surjective because one may choose $g$ distinct points with independent evaluations of [holomorphic differential forms](../../../../../holomorphic-differential-form.md); the derivative of the sum of their Abel integrals is then an isomorphism. Hence the subgroup generated by point differences contains an open subset of the connected [complex torus](../../../../../complex-torus.md), and must be the whole group. Local integration coordinates, or the exponential sequence for $\mathcal O_X$, give the same holomorphic identification. This justifies the subsequent use of degree-$d$ [line bundles](../../../../../line-bundle.md) as points of a translate of the [Jacobian variety](../../../../../jacobian-variety.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
