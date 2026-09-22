<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a symmetric matrix $B$ with $Y=\operatorname{Im}B$ positive definite, the [Riemann theta function](../../../../../riemann-theta-function.md) is

$$
\boxed{\theta(z,B)=\sum_{n\in\mathbb Z^g}\exp\bigl(\pi i n^tBn+2\pi i n^tz\bigr).}
$$

On any [compact](../../../../../compact-space.md) set of $z$, the absolute value of the summand is bounded by $\exp(-c|n|^2+C|n|)$ for some $c>0$, so the series and all its derivatives converge uniformly there. It is therefore entire. Its constant [Fourier coefficient](../../../../../fourier-coefficient.md) in $\operatorname{Re}z$ is $1$, so it is not identically zero. Reindexing $n$ gives its parity and automorphy laws:

$$
\theta(-z,B)=\theta(z,B),\qquad
\theta(z+m+Bn,B)=e^{-\pi i n^tBn-2\pi i n^tz}\theta(z,B),\quad m,n\in\mathbb Z^g.
$$

Although the [theta function](../../../../../theta-function.md) is not itself a function on $J=\mathbb C^g/\Lambda$, these factors define a [holomorphic line bundle](../../../../../holomorphic-line-bundle.md) on $J$, and its zeros define a [divisor](../../../../../divisor.md) $\Theta$ there.

For the period matrix of $X$, the [Riemann vanishing theorem](../../../../../riemann-vanishing-theorem.md) asserts that a fixed class $\kappa\in J$, the [vector of Riemann constants](../../../../../vector-of-riemann-constants.md) in the convention used here, satisfies

$$
\boxed{\Theta=W_{g-1}-\kappa.}
$$

We prove both its support statement and its reduced [divisor](../../../../../divisor.md) structure. This will make the multiplicity calculation in Solution 5 independent of any assumed multiplicity theorem.

The essential contour calculation is the [theta pullback zero-divisor identity](../../../../../theta-pullback-zero-divisor-identity.md). Put $f_z(p)=\theta(u(p)-z,B)$, regarding this as a local expression for a section on $X$. If it is not identically zero, let $D_z$ be its zero [divisor](../../../../../divisor.md). We claim

$$
\deg D_z=g,\qquad u_g(D_z)=z+\kappa.
$$

Use the cut polygon from Solution 1 and choose cuts avoiding the zeros. There $\alpha_z=d_p\log f_z$ is a [meromorphic](../../../../../meromorphic-function.md) differential whose [residues](../../../../../residue.md) are the zero multiplicities. Under continuation by an $a_j$ period, $u$ changes by the integer vector $e_j$, so $\alpha_z$ is unchanged. Under a $b_j$ period, $u$ changes by $Be_j$, so automorphy gives $\alpha_z\mapsto\alpha_z-2\pi i\omega_j$. Pairing opposite boundary sides therefore gives

$$
2\pi i\deg D_z=\int_{\partial P}\alpha_z
=2\pi i\sum_j\int_{a_j}\omega_j=2\pi ig.
$$

For example, the two $a_j$ sides, traversed with opposite orientations and separated by a $b_j$ translation, contribute $\int_{a_j}(\alpha_z-(\alpha_z-2\pi i\omega_j))$. This fixes the sign of the count.

For the first moment of the zeros, the [residue theorem](../../../../../residue-theorem.md) on the polygon gives, component by component,

$$
\sum_q\operatorname{ord}_q(f_z)\,u_k(q)=\frac{1}{2\pi i}\int_{\partial P}u_k\alpha_z.
$$

This is interpreted modulo the [period lattice](../../../../../period-lattice.md), with the lifts to the polygon fixed. Vary $z$ without letting zeros cross the cuts, and put $h=\delta\log f_z$. The coordinate $u_k$ does not vary, so integration by parts gives

$$
\delta\!\left(\sum_q\operatorname{ord}_q(f_z)u_k(q)\right)
=-\frac{1}{2\pi i}\int_{\partial P}\omega_k h.
$$

There is no endpoint term: the closed polygon boundary returns both the Abel integral and $h$ to their starting values. Across an $a_j$ translation $h$ is unchanged, while across a $b_j$ translation it changes by $2\pi i\delta z_j$. Pairing the boundary edges consequently gives $\int_{\partial P}\omega_k h=-2\pi i\sum_j\delta z_j\int_{a_j}\omega_k=-2\pi i\delta z_k$. Thus $\delta u_g(D_z)=\delta z$, and $u_g(D_z)-z$ is constant. The calculation uses weighted zeros, so their collisions cause no problem. The parameters where $f_z$ is identically zero form a proper analytic subset: they are given by the vanishing of all its local Taylor coefficients, and parameters outside $\Theta$ are not in it. Its complement in the connected [complex manifold](../../../../../complex-manifold.md) $J$ is connected, so the constant is one class $\kappa$. This proves the pullback identity globally, with continuation of the zero [divisors](../../../../../divisor.md) where necessary.

We must account for the parameters with identically zero pullback, rather than discard them. No [irreducible](../../../../../irreducible-representation.md) component $C$ of $\Theta$ can consist entirely of such parameters. Otherwise parity would imply $C-u(p)\subset\Theta$ for every $p\in X$. The image of $C\times X$ under subtraction is [irreducible](../../../../../irreducible-representation.md), is contained in $\Theta$, and contains $C$ when $p=p_0$. Since $C$ is an [irreducible](../../../../../irreducible-representation.md) component of the [hypersurface](../../../../../hypersurface.md), that image must be $C$. Hence $C-u(p)=C$ for all $p$. The surjectivity of the large-degree [Abelian sum map](../../../../../abel-map-of-an-algebraic-curve.md), proved in Solution 3, says that these translations generate all of $J$. This would make the nonempty proper subset $C$ invariant under every translation, which is impossible.

A generic point $z$ of each component of $\Theta$ therefore has nonzero pullback. Since $\theta(-z)=\theta(z)=0$, its zero [divisor](../../../../../divisor.md) contains $p_0$. Write $D_z=p_0+D'$, with $D'$ effective of degree $g-1$. The pullback identity gives $u_{g-1}(D')=z+\kappa$. Each component of $\Theta$ is consequently contained in $W_{g-1}-\kappa$. By Solution 3 the latter is [irreducible](../../../../../irreducible-representation.md) of dimension $g-1$, so any such component equals it. The zero locus is nonempty for $g>0$: any parameter with nonzero pullback has $g$ pullback zeros. We have proved equality of supports, in both directions.

Finally the automorphy factors make the [First Chern class](../../../../../first-chern-class.md) of the theta [line bundle](../../../../../line-bundle.md) primitive. On the two-torus spanned by $a_i,b_j$, the logarithm of the $b_j$ factor changes by $-2\pi i\delta_{ij}$ after the $a_i$ translation; equivalently the transition for local frames has opposite winding. Thus $c_1(a_i,b_j)=\delta_{ij}$, while $c_1(a_i,a_j)=c_1(b_i,b_j)=0$. In particular some integral pairing equals $1$. As its support is the single [irreducible](../../../../../irreducible-representation.md) [hypersurface](../../../../../hypersurface.md) $W_{g-1}-\kappa$, the zero [divisor](../../../../../divisor.md) is $m(W_{g-1}-\kappa)$ for a positive integer $m$. Its integral [First Chern class](../../../../../first-chern-class.md) would then be divisible by $m$. Primitivity forces $m=1$, proving the displayed equality as reduced [divisors](../../../../../divisor.md).

The sign convention is $\kappa=u_g(D_z)-z$, so the translate is $W_{g-1}-\kappa$; a convention naming $-\kappa$ the Riemann constant reverses that displayed sign. For $g=1$, $\kappa=(1+B)/2$ modulo periods and the zero locus is the corresponding single point. For $g=0$, the empty-lattice theta series is $1$, its zero locus is empty, and the degree-$-1$ effective locus is empty; no negative symmetric product is required.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
