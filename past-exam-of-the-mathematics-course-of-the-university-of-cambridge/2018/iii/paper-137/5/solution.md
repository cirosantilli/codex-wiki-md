<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [modular form](../../../../../modular-form.md) of integer weight $k$ for a finite-index subgroup $\Gamma\leq SL_2(\mathbb Z)$ is a [holomorphic function](../../../../../holomorphic-function.md) on the [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md) satisfying $f|_k\gamma=f$ for $\gamma\in\Gamma$ and [holomorphic](../../../../../complex-differentiability-at-a-point.md) at every [cusp of a modular group](../../../../../cusp-of-a-modular-group.md). Explicitly, for each $\sigma\in SL_2(\mathbb Z)$ choose a positive integer $h_\sigma$ with $\sigma T^{h_\sigma}\sigma^{-1}\in\Gamma$. Then $f|_k\sigma$ is periodic with period $h_\sigma$, and its expansion in $q_{h_\sigma}=e^{2\pi iz/h_\sigma}$ must have no negative powers. Equivalently it must be bounded as $\operatorname{Im}z\to\infty$, uniformly in one period. This definition applies to noncongruence subgroups too. If $-I\in\Gamma$, nonzero forms require even weight.

Put $d=[SL_2(\mathbb Z):\Gamma]$ and let $f\ne0$. Form the product over left cosets

$$
F(z)=\prod_{\gamma\in\Gamma\backslash SL_2(\mathbb Z)}(f|_k\gamma)(z).
$$

Changing a representative does not affect a factor. Right multiplication permutes the cosets, so the product is a nonzero level-one [modular form](../../../../../modular-form.md) of weight $kd$. It is [holomorphic](../../../../../complex-differentiability-at-a-point.md) on the upper half-plane and at infinity, since every factor is bounded there by cusp holomorphy.

Let $h$ be the least positive integer with $T^h\in\Gamma$, and write $f=\sum_{n\geq0}b_nq_h^n$. If $r$ is its first nonzero index, the $h$ distinct cosets $\Gamma T^j$, $0\leq j<h$, give the factors $f(z+j)$. Their product has leading term a nonzero constant times $e^{2\pi irz}=q^r$. All remaining factors are bounded at infinity. Hence $F(z)=O(e^{-2\pi r\operatorname{Im}z})$, so its level-one order satisfies $v_\infty(F)\geq r$. Notice that using just the single factor $f$ would only give $r/h$; the entire translation orbit is needed.

The permitted [valence formula for the modular group](../../../../../valence-formula-for-the-modular-group.md) bounds $v_\infty(F)\leq kd/12$, because all its other weighted zero orders are nonnegative. Thus $r\leq kd/12$. With $R=\lfloor kd/12\rfloor$, the map $f\mapsto(b_0,\ldots,b_R)$ is injective: a nonzero form in its kernel would have $r\geq R+1$. This proves the [dimension bound for modular forms on a finite-index subgroup](../../../../../dimension-bound-for-modular-forms-on-a-finite-index-subgroup.md):

$$
\boxed{\dim M_k(\Gamma)\leq\lfloor kd/12\rfloor+1\leq1+kd/12
\quad(k\geq0).}
$$

For the dilation assertion, the original PDF states $N_1D\mid N$, a product-divisibility condition, rather than the TeX's chain $N_1\mid D\mid N$. Use the PDF condition. Put $A=\operatorname{diag}(D,1)$. If $\gamma=\begin{pmatrix}a&b\\c&d\end{pmatrix}\in\Gamma_0(N)$, then

$$
A\gamma A^{-1}=\begin{pmatrix}a&Db\\c/D&d\end{pmatrix}\in\Gamma_0(N_1),
$$

since $N_1D\mid c$. Therefore, for $g(z)=f(Dz)$, either direct substitution or the [slash operator for modular forms](../../../../../slash-operator-for-modular-forms.md) gives $g|_k\gamma=g$. It is [holomorphic](../../../../../complex-differentiability-at-a-point.md) on the upper half-plane.

To verify every cusp, take $\sigma\in SL_2(\mathbb Z)$ and choose $\tau\in SL_2(\mathbb Z)$ taking infinity to the rational cusp $A\sigma\infty$. Then $B=\tau^{-1}A\sigma$ is rational upper triangular, with positive ratio of its two diagonal entries. Consequently

$$
(f|_k A)|_k\sigma=(f|_k\tau)|_k B
$$

is a nonzero constant factor times $f|_k\tau$ evaluated at an affine map $z\mapsto uz+v$ with $u>0$. The imaginary part tends to infinity, where $f|_k\tau$ is bounded. Thus $g|_k\sigma$ is bounded too. Together with its periodicity this proves cusp holomorphy by the [Riemann removable singularity theorem](../../../../../riemann-removable-singularity-theorem.md). Hence the [oldform by argument dilation](../../../../../oldform-by-argument-dilation.md) satisfies

$$
\boxed{f\in M_k(\Gamma_0(N_1)),\ N_1D\mid N
\ \Longrightarrow\ f(Dz)\in M_k(\Gamma_0(N)).}
$$

Finally $\Gamma_0(3)$ has index four: reduction modulo three gives a transitive $SL_2(\mathbb F_3)$ action on the four points of $\mathbb P^1(\mathbb F_3)$, and $\Gamma_0(3)$ is the inverse image of the stabilizer of infinity. Reduction is surjective, since elementary determinant-one matrices generate $SL_2(\mathbb F_3)$ and lift integrally. The dimension bound gives $\dim M_4(\Gamma_0(3))\leq2$.

The normalized [Eisenstein series](../../../../../eisenstein-series.md) $E_4(z)$ and the oldform $E_4(3z)$ both belong to this space. Their [Fourier expansion of a normalized Eisenstein series](../../../../../fourier-expansion-of-a-normalized-eisenstein-series.md) starts as

$$
E_4(z)=1+240q+O(q^2),\qquad E_4(3z)=1+240q^3+O(q^6).
$$

A linear relation between them has zero constant term only if its two scalars sum to zero; its $q$ coefficient then forces both scalars to vanish. They are independent, proving the [weight-four modular forms on Gamma 0 3](../../../../../weight-four-modular-forms-on-gamma-0-3.md) description

$$
\boxed{\dim M_4(\Gamma_0(3))=2,\qquad
\{E_4(z),E_4(3z)\}\text{ is a basis}.}
$$

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 137](../../paper-137-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
