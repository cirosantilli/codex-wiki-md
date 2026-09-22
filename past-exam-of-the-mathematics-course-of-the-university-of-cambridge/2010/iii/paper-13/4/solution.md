<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [canonical bundle](../../../../../canonical-bundle.md) is $K_M=\bigwedge^m(T^{1,0}M)^*$, the [holomorphic line bundle](../../../../../holomorphic-line-bundle.md) of holomorphic top forms on a complex $m$-manifold. For an embedded complex submanifold $V$ of dimension $n$, the holomorphic [normal bundle](../../../../../normal-bundle.md) is the quotient

$$
0\longrightarrow T^{1,0}V\longrightarrow T^{1,0}M|_V\longrightarrow N_{V/M}\longrightarrow0.
$$

Taking determinants and duals gives [adjunction for a smooth submanifold](../../../../../adjunction-for-a-smooth-submanifold.md):

$$
\boxed{K_V\cong K_M|_V\otimes\det N_{V/M}.}
$$

For a closed smooth hypersurface, $[V]=\mathcal O_M(V)$ is its [divisor line bundle](../../../../../divisor-line-bundle.md), equipped with a holomorphic section whose zero divisor is $V$ with multiplicity one. If $f_\alpha$ locally defines $V$, local meromorphic generators $1/f_\alpha$ transform by the holomorphic units $f_\alpha/f_\beta$. The stated normal-bundle relation is

$$
\boxed{[V]|_V\cong N_{V/M},\qquad K_V\cong(K_M\otimes[V])|_V.}
$$

Equivalently the conormal is $\mathcal O_M(-V)|_V$. The closed-divisor interpretation is needed to define $[V]$; an arbitrary nonclosed local submanifold does not define that global divisor bundle.

For a holomorphic subbundle $F\subset E$, define $D_Fs=\pi D_Es$ on sections of $F$, with $\pi$ acting on the bundle factor of a bundle-valued form. It obeys the [Leibniz rule](../../../../../leibniz-rule.md). Since $F$ is holomorphic, $D_E^{0,1}s=\bar\partial_Es$ lies in $F$, so $D_F^{0,1}=\bar\partial_F$. For $s,t\in F$, their inner products with the normal components of $D_Es,D_Et$ vanish; hence projecting preserves [metric compatibility](../../../../../metric-compatibility.md). The uniqueness proved for the [Chern connection](../../../../../chern-connection.md) identifies

$$
\boxed{D_F=\pi\circ D_E|_F.}
$$

This is the [projected Chern connection](../../../../../projected-chern-connection.md).

Choose the adapted smooth unitary frame and retain Question 2's input-index convention. The [connection matrix](../../../../../connection-one-form.md) is skew-Hermitian. Its upper-left block is $\theta_1$ for $D_F$; writing the lower-left block as $-A$ forces the upper-right block to be $\overline A^t$:

$$
\boxed{\theta_E=\begin{pmatrix}\theta_1&\overline A^t\\-A&\theta_2\end{pmatrix}.}
$$

Holomorphicity of $F$ makes the normal part of $D_E^{0,1}s$ vanish, so $B=\overline A^t$ has type $(1,0)$, and $A$ has type $(0,1)$. The matrix $B$ represents the [second fundamental form of a holomorphic subbundle](../../../../../second-fundamental-form-of-a-holomorphic-subbundle.md) in this input-index convention. These types would appear in the opposite blocks with coefficient-column indices; they must not be swapped while retaining the printed minus-sign Cartan equation.

Take the upper-left block of the [Cartan curvature equation with input indices](../../../../../cartan-curvature-equation-with-input-indices.md). It is

$$
(\Theta_E)_{11}=d\theta_1-\theta_1\wedge\theta_1+\overline A^t\wedge A=\Theta_F+\overline A^t\wedge A.
$$

Therefore the [curvature formula for a holomorphic subbundle](../../../../../curvature-formula-for-a-holomorphic-subbundle.md) is

$$
\boxed{\Theta_F=(\Theta_E)_{11}-\overline A^t\wedge A=(\Theta_E)_{11}-B\wedge\overline B^t.}
$$

The sign and the order of the factors both follow from the displayed block multiplication.

Now let $M$ be a [complex torus](../../../../../complex-torus.md) and $V$ a closed smooth hypersurface. The torus has a translation-invariant flat [Kähler metric](../../../../../kahler-metric.md), and $T^{1,0}M$ and $K_M$ are holomorphically trivial. Give $E=T^{1,0}M|_V$ its flat metric and apply the preceding formula to $F=T^{1,0}V$. Since $\Theta_E=0$,

$$
\Theta_{TV}=-B\wedge\overline B^t,\qquad\Theta_{K_V}=-\operatorname{tr}\Theta_{TV}=\operatorname{tr}(B\wedge\overline B^t).
$$

For a $(1,0)$ tangent vector $X$, the latter coefficient is $\operatorname{tr}(B(X)B(X)^\dagger)\geq0$, so $i\Theta_{K_V}$ is a semipositive real $(1,1)$ form. Thus $K_V$ is a [semipositive holomorphic line bundle](../../../../../semipositive-holomorphic-line-bundle.md). This proves the [semipositive canonical bundle of a submanifold of a complex torus](../../../../../semipositive-canonical-bundle-of-a-submanifold-of-a-complex-torus.md) assertion directly from curvature. By [adjunction for a smooth submanifold](../../../../../adjunction-for-a-smooth-submanifold.md), $K_V\cong[V]|_V$.

Restrict a positive metric on $L$ to $V$. The tensor-product metric on

$$
P_a=(L\otimes[V]^{\otimes a})|_V
$$

has curvature $i\Theta_{L|_V}+a\,i\Theta_{K_V}$, which is positive for every nonnegative integer $a$. Hence

$$
\boxed{(L\otimes[V]^{\otimes a})|_V\text{ is a positive holomorphic line bundle for every }a\in\mathbb Z_{\geq0}.}
$$

The integer condition is implicit in a tensor power. No assertion of strict positivity of $[V]|_V$ is required.

For vanishing, write $E_a=L\otimes[V]^{\otimes a}$. The allowed [Kodaira vanishing theorem](../../../../../kodaira-vanishing-theorem.md) says that on a compact [Kähler manifold](../../../../../kahler-manifold.md) $X$, $H^i(X,K_X\otimes P)=0$ for $i>0$ when $P$ is a [positive holomorphic line bundle](../../../../../positive-holomorphic-line-bundle.md). Since $K_M$ is trivial, its application on the torus gives $H^i(M,E_0)=H^i(M,L)=0$ for $i>0$.

For every $a\geq1$, the divisor section gives the exact sequence

$$
0\longrightarrow E_{a-1}\longrightarrow E_a\longrightarrow i_*(E_a|_V)\longrightarrow0,
$$

where $i:V\hookrightarrow M$. Crucially,

$$
E_a|_V\cong K_V\otimes P_{a-1},
$$

and $P_{a-1}$ is positive by the proved restriction statement. The induced [Kähler metric](../../../../../kahler-metric.md) makes $V$ compact Kähler, so [Kodaira vanishing theorem](../../../../../kodaira-vanishing-theorem.md) on $V$ gives $H^i(V,E_a|_V)=0$ for all $i>0$. In the [long exact sequence in sheaf cohomology](../../../../../long-exact-sequence-in-sheaf-cohomology.md), the segment

$$
H^i(M,E_{a-1})\longrightarrow H^i(M,E_a)\longrightarrow H^i(V,E_a|_V)
$$

then has zero outside terms by induction. Therefore

$$
\boxed{H^i(M,L\otimes[V]^{\otimes a})=0\qquad(i>0,\ a\in\mathbb Z_{\geq0}).}
$$

This proves [vanishing for divisor twists on a complex torus](../../../../../vanishing-for-divisor-twists-on-a-complex-torus.md) using restriction positivity and the divisor exact sequence, rather than presuming ambient positivity of every divisor twist.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
