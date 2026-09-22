<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $u,v,w$ be the consecutive primitive [toric ray](../../../../../ray-of-a-fan.md) vectors around the compact invariant curve $F=F_v$. Smoothness gives oriented determinants $\det(u,v)=\det(v,w)=1$, hence $u+w=bv$ for an integer $b$. Choose an [algebraic torus character](../../../../../algebraic-torus-character.md) $m$ with $\langle m,u\rangle=0$ and $\langle m,v\rangle=1$. The [principal divisor on a toric variety](../../../../../principal-divisor-on-a-toric-variety.md) has coefficient one at $F$, coefficient $b$ at $F_w$, and zero at $F_u$. The other invariant curves do not meet $F$, while each adjacent one meets it transversely once. Intersecting this [principal divisor](../../../../../principal-divisor-on-an-algebraic-curve.md) with the proper curve $F$ gives $0=F^2+b$. This proves the [self-intersection formula for a toric surface divisor](../../../../../self-intersection-formula-for-a-toric-surface-divisor.md) even when the ambient surface is not complete.

If $F^2=-1$, then $b=1$ and $v=u+w$. The vectors $u,w$ form a lattice basis since $\det(u,w)=1$, and their [toric cone](../../../../../cone-in-toric-geometry.md) is the union of the two [toric cones](../../../../../cone-in-toric-geometry.md) adjacent to $v$. Deleting $v$ is consequently a smooth [toric fan](../../../../../fan-in-toric-geometry.md) coarsening. Its inverse is precisely the [toric blowup at a torus-fixed point](../../../../../toric-blowup-at-a-torus-fixed-point.md), obtained by inserting the sum of the two primitive basis vectors. Conversely, that insertion gives $u+w=v$, and hence [algebraic self-intersection](../../../../../self-intersection-of-an-algebraic-curve.md) $-1$. Thus the [toric contraction of a minus-one curve](../../../../../toric-contraction-of-a-minus-one-curve.md) satisfies

$$
\boxed{F\text{ contracts torically to a smooth point}\ \Longleftrightarrow\ F^2=-1.}
$$

For the cyclic quotient description, first take a strongly convex [toric cone](../../../../../cone-in-toric-geometry.md) of dimension two. Write its primitive boundary vectors as $a,b$ and put $N_0=\mathbb Za+\mathbb Zb$, $r=[N:N_0]$. Since $a$ is primitive, extend it to a basis of $N$ and write $b=ua+rc$ with $\gcd(u,r)=1$. Thus $N/N_0$ is cyclic of order $r$. In the lattice $N_0$, the [toric cone](../../../../../cone-in-toric-geometry.md) is smooth and its [toric variety](../../../../../toric-variety.md) is $\mathbb A^2$. Passing to the larger lattice $N$ takes the finite quotient whose invariant [monomials](../../../../../monomial.md) are precisely those in the smaller dual lattice $M=N^*\subset N_0^*$. Relative to the two boundary coordinates, $c=(b-ua)/r$, so a generator acts with weights $(-u,1)$ modulo $r$. Replacing that generator by a suitable power makes the first weight one and the second some $q$ with $0<q<r$ and $\gcd(q,r)=1$. Therefore, for the singular case,

$$
\boxed{U_\sigma\cong\mathbb A^2/\mu_r,\qquad\zeta\cdot(x,y)=(\zeta x,\zeta^q y).}
$$

The [cyclic quotient surface singularity](../../../../../cyclic-quotient-surface-singularity.md) can equivalently be described by the first-quadrant [toric cone](../../../../../cone-in-toric-geometry.md) in

$$
L=\mathbb Z^2+\mathbb Z\frac{(1,q)}r,\qquad L^*=\{(i,j)\in\mathbb Z^2:i+qj\equiv0\pmod r\}.
$$

Indeed its coordinate ring is $k[x^iy^j:i,j\ge0,\ i+qj\equiv0\pmod r]=k[x,y]^{\mu_r}$. Characteristic zero ensures the stated ordinary finite-group quotient interpretation.

The restriction to singular [toric cones](../../../../../cone-in-toric-geometry.md) of dimension two is necessary for $r>1$. A smooth [toric cone](../../../../../cone-in-toric-geometry.md) has $r=1$ and gives $\mathbb A^2$ with the trivial quotient. A [toric cone](../../../../../cone-in-toric-geometry.md) of dimension one gives $\mathbb A^1\times k^*$, and the zero [toric cone](../../../../../cone-in-toric-geometry.md) gives $(k^*)^2$. These latter surfaces cannot be a quotient of the displayed kind, since they have nonconstant invertible [regular functions](../../../../../regular-function.md), whereas $k[x,y]^{\mu_r}$ has only constant units. Thus the blanket affine-surface wording requires these separate cases.

For the singular case, compute the [negative continued fraction](../../../../../negative-continued-fraction.md) by the ceiling form of the [Euclidean algorithm](../../../../../euclidean-algorithm.md). Start with $a_0=r$, $a_1=q$, and, while $a_i>0$, set

$$
b_i=\left\lceil\frac{a_{i-1}}{a_i}\right\rceil,\qquad a_{i+1}=b_ia_i-a_{i-1}.
$$

Then $0\le a_{i+1}<a_i$, so the process terminates at $a_{s+1}=0$. The gcd is unchanged at each step, hence $a_s=1$. Since $a_{i-1}>a_i>0$, every $b_i\ge2$. Rearranging the recurrence gives

$$
\boxed{\frac rq=[b_1,\ldots,b_s]^-=b_1-\frac1{b_2-\dfrac1{\cdots-1/b_s}}.}
$$

Now define lattice vectors

$$
v_0=(0,1),\qquad v_1=\frac{(1,q)}r,\qquad v_{i+1}=b_iv_i-v_{i-1}.
$$

To verify this [Hirzebruch–Jung resolution](../../../../../hirzebruch-jung-resolution.md) algorithm, write $v_i=(p_i,a_i)/r$ with $p_0=0$, $p_1=1$ and $p_{i+1}=b_ip_i-p_{i-1}$. Induction gives $a_i\equiv qp_i\pmod r$, so $v_i\in L$. It also gives $p_i a_{i+1}-a_i p_{i+1}=-r$. Thus every adjacent pair has absolute determinant $1/r$, the covolume of $L$, and is a basis of $L$. The $p_i$ increase strictly, while the $a_i$ decrease to zero, so these [toric rays](../../../../../ray-of-a-fan.md) occur in order inside the first quadrant. At termination, $a_s=1$ and the determinant identity gives $p_{s+1}=r$, hence $v_{s+1}=(1,0)$. All boundary and inserted vectors are primitive because they occur in lattice bases.

Subdivide the quadrant by $v_1,\ldots,v_s$. Every resulting [toric cone](../../../../../cone-in-toric-geometry.md) is smooth by the [smoothness criterion for a toric variety](../../../../../smoothness-criterion-for-a-toric-variety.md), and the [fan subdivision](../../../../../fan-subdivision.md) gives a proper birational [toric morphism](../../../../../toric-morphism.md), hence a resolution. Each interior [toric ray](../../../../../ray-of-a-fan.md) has a complete one-dimensional star, so its [exceptional curve of a surface resolution](../../../../../exceptional-curve-of-a-surface-resolution.md) is $\mathbb P^1$. The recurrence yields

$$
\boxed{F_i^2=-b_i\le-2,\qquad F_i\cdot F_{i+1}=1,\qquad F_i\cdot F_j=0\ (|i-j|>1).}
$$

This proves minimality: no [exceptional curve of a surface resolution](../../../../../exceptional-curve-of-a-surface-resolution.md) can be contracted to a smooth point by the [Castelnuovo contraction criterion](../../../../../castelnuovo-contraction-criterion.md). There is also a direct [toric fan](../../../../../fan-in-toric-geometry.md) check. For fixed $i$, the determinants of $v_i$ with $v_{i+h}$, measured in units of the lattice covolume, satisfy the same recurrence with coefficients at least two and initial values zero and one. They are at least $h$. Omitting any intervening [toric ray](../../../../../ray-of-a-fan.md) therefore leaves a [toric cone](../../../../../cone-in-toric-geometry.md) of determinant at least two, so no nontrivial coarsening is smooth. Thus this is the [minimal resolution of a cyclic quotient surface singularity](../../../../../hirzebruch-jung-resolution.md).

If all exceptional [algebraic self-intersections](../../../../../self-intersection-of-an-algebraic-curve.md) are $-2$, all $b_i=2$ and induction gives $[2,\ldots,2]^-= (s+1)/s$. Since $r,q$ are coprime, this forces $r=s+1$, $q=s$. Conversely $r/(r-1)$ has exactly $r-1$ coefficients equal to two. Therefore

$$
\boxed{F_i^2=-2\text{ for every exceptional curve}\ \Longleftrightarrow\ q=r-1.}
$$

For the final [toric fan](../../../../../fan-in-toric-geometry.md), the minimal smooth [fan subdivision](../../../../../fan-subdivision.md) of the [toric cone](../../../../../cone-in-toric-geometry.md) from $(0,1)$ to $(r,1)$ inserts the [toric rays](../../../../../ray-of-a-fan.md) $(j,1)$ for $1\le j<r$. Adjacent determinants have absolute value one, and $(j-1,1)+(j+1,1)=2(j,1)$, so its inserted curves have [algebraic self-intersection](../../../../../self-intersection-of-an-algebraic-curve.md) $-2$ and it is the minimal [fan subdivision](../../../../../fan-subdivision.md) just described. The second original [toric cone](../../../../../cone-in-toric-geometry.md), from $(r,1)$ to $(1,0)$, is already smooth.

Write $v_j=(j,1)$ and $e=(1,0)$. In the resolved [toric fan](../../../../../fan-in-toric-geometry.md), the rightmost interior [toric ray](../../../../../ray-of-a-fan.md) obeys $v_{r-1}+e=v_r$, so its curve has [algebraic self-intersection](../../../../../self-intersection-of-an-algebraic-curve.md) $-1$ and can be blown down to a smooth point. After deleting it, the same relation $v_{r-2}+e=v_{r-1}$ applies to the new rightmost interior [toric ray](../../../../../ray-of-a-fan.md). Continue deleting $v_r,v_{r-1},\ldots,v_1$ in that order. Each deletion is the inverse of a [toric blowup at a torus-fixed point](../../../../../toric-blowup-at-a-torus-fixed-point.md). The last [toric fan](../../../../../fan-in-toric-geometry.md) has only the quadrant [toric cone](../../../../../cone-in-toric-geometry.md) and defines $\mathbb A^2$. Consequently

$$
\boxed{X_{\Sigma'}\longrightarrow\mathbb A^2\text{ is the composite of exactly }r\text{ smooth-point toric blowdowns}.}
$$

All maps induce the identity on the dense [algebraic torus](../../../../../algebraic-torus.md), so this composite is the same morphism as $X_{\Sigma'}\to X_\Sigma\to\mathbb A^2$. The intermediate smooth [toric fans](../../../../../fan-in-toric-geometry.md) need not include the singular [toric fan](../../../../../fan-in-toric-geometry.md) $\Sigma$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
