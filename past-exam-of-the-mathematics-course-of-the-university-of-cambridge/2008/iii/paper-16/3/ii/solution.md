<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Index the [functions](../../../../../../function-split.md) as $g_0,g_1,g_2,g_3$ and write $\Lambda=\mathbb E_{x,d}\prod_{j=0}^3g_j(x+jd)$. We first control $g_0$. Change variables to $y=x+3d$, average over $d$, and apply [Cauchy-Schwarz](../../../../../../cauchy-schwarz-inequality.md) in $y$, discarding the bounded factor $g_3(y)$. Expand the squared inner average with the second copy of $d$ written $d+h$, then put $x=y-3d$. This yields

$$
|\Lambda|^2\leq\mathbb E_{h,x,d}\Delta_{-3h}g_0(x)\,\Delta_{-2h}g_1(x+d)\,\Delta_{-h}g_2(x+2d).
$$

The right side is real and nonnegative because it arose as an average of squared absolute values. Next use $y=x+2d$ and apply [Cauchy-Schwarz](../../../../../../cauchy-schwarz-inequality.md) in $(h,y)$, discarding the bounded $g_2$ derivative. Expanding with a displacement $k$ in $d$ gives

$$
|\Lambda|^4\leq\mathbb E_{h,k,x,d}\Delta_{-2k}\Delta_{-3h}g_0(x)\,\Delta_{-k}\Delta_{-2h}g_1(x+d).
$$

Finally use $y=x+d$ and [Cauchy-Schwarz](../../../../../../cauchy-schwarz-inequality.md) in $(h,k,y)$, discarding the bounded $g_1$ double derivative. Expansion with displacement $r$ gives

$$
|\Lambda|^8\leq\mathbb E_{h,k,r,x}\Delta_{-r}\Delta_{-2k}\Delta_{-3h}g_0(x)=\mathbb E_{h,k}\left|\mathbb E_x\Delta_{-2k}\Delta_{-3h}g_0(x)\right|^2.
$$

All these changes of variables are bijections without any division in $G$.

Put $t_j=|G[j]|$, where $G[j]=\{z:jz=0\}$ is the [torsion subgroup killed by an integer](../../../../../../torsion-subgroup-killed-by-an-integer.md) $j$. The variables $2k$ and $3h$ are uniform on $2G$ and $3G$, whose indices are $t_2,t_3$. Since the last squared integrand is nonnegative, its restricted average is at most $t_2t_3$ times the unrestricted average over the two increments. By part (i), that unrestricted average is $\|g_0\|_{U^3}^8$. Hence $|\Lambda|\leq(t_2t_3)^{1/8}\|g_0\|_{U^3}$.

To control $g_1$, apply the same three eliminations in the order of slopes $3,0,2$. The surviving $g_1$ has increments $-2h,k,-r$. The last increment is uniform, and only the first is restricted to $2G$, so the resulting bound is $|\Lambda|\leq t_2^{1/8}\|g_1\|_{U^3}$. Reversing the [arithmetic progression](../../../../../../arithmetic-progression.md) by $(x,d)\mapsto(x+3d,-d)$ treats $g_3$ and $g_2$ respectively. This proves the [four-term progression bound with torsion factors](../../../../../../four-term-progression-bound-with-torsion-factors.md):

$$
\boxed{|\Lambda|\leq(t_2t_3)^{1/8}\min_i\|f_i\|_{U^3},\qquad\beta=(t_2t_3)^{1/8}\alpha.}
$$

For a fixed [finite group](../../../../../../finite-group.md), this positive constant tends to zero with $\alpha$. In $\mathbb Z_N$, $t_j=\gcd(j,N)$, so $\boxed{\beta=6^{1/8}\alpha\text{ suffices uniformly in }N}$. If multiplication by two and three are bijective, the sharper $\beta=\alpha$ holds.

A dependence on torsion is necessary if a bound uniform over all finite abelian groups is intended. In $G=\mathbb F_2^m$, choose independent random signs $f(x)$. A cube with eight distinct vertices has sign product of [expectation](../../../../../../expected-value.md) zero. Each of the twenty-eight possible collisions has [probability](../../../../../../probability.md) $1/|G|$, so the [expectation](../../../../../../expected-value.md) of $\|f\|_{U^3}^8$ is at most $28/|G|$. Some sign [function](../../../../../../function-split.md) therefore has [norm](../../../../../../norm.md) at most $(28/|G|)^{1/8}$. But with factors $(f,1,f,1)$, every [arithmetic progression](../../../../../../arithmetic-progression.md) is $(x,x+d,x,x+d)$ and its product is $f(x)^2=1$. Thus [unbounded torsion obstructs uniform control of four-term progressions](../../../../../../unbounded-torsion-obstructs-uniform-control-of-four-term-progressions.md). The stated fixed-group bound, and the uniform cyclic-group bound needed in part (iii), are unaffected.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
